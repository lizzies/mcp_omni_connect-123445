# Local Tools System

While MCP servers provide a wide range of integration, you often need to give your agent access to internal business logic, custom APIs, or specialized Python code. The **Local Tools System** allows you to register any Python function as a tool.

## Using the `ToolRegistry`

The `ToolRegistry` is the central manager for local tools.

```python
from omnicoreagent import OmniCoreAgent, ToolRegistry

# 1. Create a registry
tools = ToolRegistry()

# 2. Register a tool using a decorator
@tools.register_tool("get_stock_price")
def get_stock_price(ticker: str) -> str:
    """
    Get the current stock price for a ticker.
    Args:
        ticker: The stock ticker symbol (e.g., AAPL).
    """
    # Your custom logic here
    return f"Stock price for {ticker}: $150.00"

# 3. Pass the registry to the agent
agent = OmniCoreAgent(
    ...
    local_tools=tools
)
```

---

## Tool Requirements

For a function to work as a tool, it must meet these criteria:

1. **Docstrings**: The function *must* have a clear docstring. This is how the LLM understands when and how to use the tool.
2. **Type Hints**: Arguments should have type hints to help the agent generate the correct input schema.
3. **Return Value**: The function should return a string or a JSON-serializable object that the agent can read as an observation.

---

## Advanced Usage

### Accessing Tool Info

You can query the registry for all registered tools and their schemas.

```python
available_tools = tools.get_available_tools()
for tool in available_tools:
    print(f"Tool: {tool.name}")
    print(f"Description: {tool.description}")
```

### Integration with MCP

Local tools and MCP tools coexist seamlessly. The agent can use a local tool to process data and then pass it to an MCP tool (e.g., fetch a stock price locally and save it to a remote database via MCP).

---

## Best Practices

- **Atomic Tools**: Keep tools small and focused on a single task.
- **Clear Descriptions**: Spend time on the tool's docstring. Use descriptions like "Fetch the latest production logs for a specific service ID" instead of "Get logs".
- **Error Handling**: Catch exceptions within your tools and return a helpful error message to the agent so it can decide how to proceed.

```python
@tools.register_tool("fetch_data")
def fetch_data(id: int):
    try:
        # fetch logic
        return data
    except Exception as e:
        return f"Error fetching data: {str(e)}. Please check the ID and try again."
```
