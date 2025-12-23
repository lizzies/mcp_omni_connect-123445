# Memory Tool Backend (Working Memory)

The **Memory Tool Backend** provides your agent with a persistent, file-based local workspace. Unlike conversation history (which stores what was *said*), this backend is for what the agent *does* — creating files, saving plans, and managing data during long-running tasks.

## Configuration

Enable the local file-based memory in the agent configuration:

```python
agent_config = {
    "memory_tool_backend": "local"  # Enable file-based workspace
}

agent = OmniCoreAgent(
    ...
    agent_config=agent_config
)
```

---

## How It Works

1. **Storage**: Files are stored in a `./memories/` directory in your project root.
2. **Persistence**: These files persist across agent restarts and re-initializations.
3. **Security**: Built-in path traversal protection ensures the agent can only access the designated memory directory.
4. **Safety**: Thread-safe file locking allows multiple agent steps or sub-agents to access the workspace safely.

---

## Workspace Tools

When enabled, the agent automatically gains access to these management tools:

| Tool | Action |
|------|--------|
| `memory_view` | List files and directories in the workspace. |
| `memory_create_update` | Create new files or overwrite existing ones. |
| `memory_str_replace` | Find and replace text within a file (ideal for code edits). |
| `memory_insert` | Insert text at exact line numbers. |
| `memory_delete` | Remove files or directories. |
| `memory_rename` | Rename or move files within the workspace. |
| `memory_clear_all` | Wipe the entire workspace (use with caution!). |

---

## Use Cases

### 🛠️ Code Generation
An agent can write a plan to a `TODO.md` file, then incrementally write code files, run tests, and update its progress in the plan.

### 📊 Data Processing
Store intermediate results between complex transformation steps. If a process takes several minutes, the agent can resume from the last saved state.

### 📋 Multi-step Planning
For extremely complex tasks, the agent can "externalize" its reasoning by writing out a detailed multi-step plan that it updates as it completes each component.

### 💾 Context Extension
When a task involves more information than fits in the LLM's context window, the agent can save important notes to files and retrieve them only when needed using `memory_view`.

---

## Best Practices

- **Structured Files**: Encourage the agent to use structured formats (JSON, Markdown) for its internal files to make retrieval easier.
- **Incremental Edits**: Use `memory_str_replace` or `memory_insert` instead of overwriting large files to save tokens and maintain precision.
- **Directory Organization**: For complex projects, tell the agent to create subdirectories within `./memories/` to keep its workspace clean.
