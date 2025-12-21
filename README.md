# 🚀 OmniCoreAgent - Production-Ready AI Agent Framework

> **A powerful Python framework for building autonomous AI agents that think, reason, and execute complex tasks. Production-ready agents that use tools, manage memory, coordinate workflows, and handle real-world business logic.**

## 🎯 TL;DR (30 Seconds)

**OmniCoreAgent** = Build AI agents that:
- 🤖 **Think and reason** (not just chatbots)
- 🛠️ **Use tools** (APIs, databases, files)
- 🧠 **Remember context** (across conversations)
- 🔄 **Orchestrate workflows** (multi-agent systems)
- 🚀 **Run in production** (monitoring, scaling, reliability)
- 🔌 **Plug & Play** (switch memory/event backends at runtime—Redis ↔ MongoDB ↔ PostgreSQL ↔ in-memory)

**Perfect for**: Developers building AI assistants, automation systems, or multi-agent applications.

**Get Started**: `pip install omnicoreagent` → Set `LLM_API_KEY` → Build your first agent in 30 seconds.

[![PyPI Downloads](https://static.pepy.tech/badge/omnicoreagent)](https://pepy.tech/projects/omnicoreagent)
[![Python Version](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Tests](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/omnirexflora-labs/omnicoreagent/actions)
[![PyPI version](https://badge.fury.io/py/omnicoreagent.svg)](https://badge.fury.io/py/omnicoreagent)
[![Last Commit](https://img.shields.io/github/last-commit/omnirexflora-labs/omnicoreagent)](https://github.com/omnirexflora-labs/omnicoreagent/commits/main)
[![Open Issues](https://img.shields.io/github/issues/omnirexflora-labs/omnicoreagent)](https://github.com/omnirexflora-labs/omnicoreagent/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/omnirexflora-labs/omnicoreagent)](https://github.com/omnirexflora-labs/omnicoreagent/pulls)

<p align="center">
  <img src="assets/IMG_5292.jpeg" alt="OmniCoreAgent Logo" width="300"/>
</p>

## 📋 Table of Contents

### 🚀 **Getting Started**
- [🎯 TL;DR (30 Seconds)](#-tldr-30-seconds)
- [⚡ Quick Start (1 Minute)](#-quick-start-1-minute)
- [🌟 What is OmniCoreAgent?](#-what-is-omnicoreagent)
- [🎯 What Problem Does OmniCoreAgent Solve?](#-what-problem-does-omnicoreagent-solve)
- [📚 Glossary](#-glossary-for-non-technical-readers)
- [🏗️ Architecture Overview](#️-architecture-overview)
- [📦 Installation & Setup](#-installation--setup)

### 🎯 **Core Features**
- [🤖 OmniAgent - The Heart of the Framework](#1--omniagent---the-heart-of-the-framework)
- [🧠 Multi-Tier Memory System](#2--multi-tier-memory-system)
- [📡 Event System](#3--event-system)
- [🛠️ Local Tools System](#4--local-tools-system)
- [💾 Memory Tool Backend](#5--memory-tool-backend)
- [🚁 Background Agents](#6--background-agents)
- [🔄 Workflow Agents](#7--workflow-agents)
- [🧠 Advanced Tool Use](#8--advanced-tool-use)
- [📊 Production Observability](#9--production-observability)
- [🌐 Universal Model Support](#10--universal-model-support)
- [🔌 Built-in MCP Client](#11--built-in-mcp-client)

### 📖 **Advanced Topics**
- [🎯 Production Examples](#-production-examples)
- [🚀 Advanced Features](#-advanced-features)
- [⚙️ Configuration Guide](#-configuration-reference)
- [🧠 Vector Database Setup](#-vector-database-integration)
- [📊 Opik Tracing Setup](#-opik-tracing)

### 🛠️ **Development & Support**
- [🧪 Testing](#-testing)
- [🔍 Troubleshooting](#-troubleshooting)
- [🤝 Contributing](#-contributing)
- [📖 Documentation](#-documentation)
- [🌟 Why OmniCoreAgent?](#-why-omnicoreagent)


---

## 🌟 What is OmniCoreAgent?

**OmniCoreAgent** is a powerful, production-ready Python framework for building autonomous AI agents that think, reason, and execute complex tasks. It provides a sophisticated yet intuitive architecture for AI agents that go beyond chatbots—agents that use tools, manage memory, coordinate workflows, and handle real-world business logic.

## 🎯 What Problem Does OmniCoreAgent Solve?

### Before OmniCoreAgent

Building production-ready AI agents was challenging:
- ❌ **Complex Setup**: Requires integrating multiple libraries (LLM, memory, tools, orchestration)
- ❌ **Difficult Orchestration**: Complex code to coordinate multiple agents
- ❌ **No Production Infrastructure**: Missing monitoring, observability, error handling
- ❌ **Vendor Lock-in**: Hard to switch between AI providers
- ❌ **Tool Integration Complexity**: Difficult to connect agents to external services

### With OmniCoreAgent

Build production-ready agents in minutes:
- ✅ **Simple API**: `OmniAgent(...)` and you're done
- ✅ **Built-in Persistance storage**: Redis, PostgreSQL, Mysql, MongoDB, SQLite—**switch at runtime!**
- ✅ **Plug & Play**: Switch memory and event backends at runtime (Redis ↔ MongoDB ↔ PostgreSQL ↔ Mysql ↔ SQLite ↔ in-memory)
- ✅ **Workflow Orchestration**: Sequential, Parallel, and Router agents out of the box
- ✅ **Production-Ready**: Monitoring, observability, error handling built-in
- ✅ **Model Agnostic**: Switch between OpenAI, Anthropic, Groq, Ollama, and 100+ models
- ✅ **Easy Tool Integration**: Connect to MCP servers or register Python functions as tools

### Core Philosophy

OmniCoreAgent is designed for **production applications**, not experiments. It's a complete framework that handles everything from memory management and tool orchestration to background automation and real-time event streaming. Build agents that plan multi-step workflows, use tools to gather information, validate results, and adapt their approach based on outcomes.

### Key Differentiators

- **🏗️ Complete Agent Framework**: Full framework with built-in infrastructure—not just a library
- **🧠 Multi-Tier Memory System**: In-memory, Redis, PostgreSQL, MySQL, SQLite, MongoDB—**switch at runtime!**
- **📡 Real-Time Event System**: Event router with in-memory and Redis Streams backends—**switch at runtime!**
- **🛠️ Local Tools System**: Register any Python function as an AI tool with simple decorators
- **🚁 Background Agents**: Autonomous task execution with intelligent scheduling
- **🔄 Workflow Orchestration**: Sequential, Parallel, and Router agents for complex multi-agent systems
- **💾 Memory Tool Backend**: Persistent agent working memory for long-running tasks
- **📊 Production Observability**: Opik tracing, metrics, and comprehensive monitoring
- **🌐 Universal Model Support**: Model-agnostic through LiteLLM—use any LLM provider
- **🔌 Built-in MCP Client**: Seamless integration with Model Context Protocol servers—connect to filesystems, databases, APIs, and more

---

## ⚡ Quick Start (1 Minute)

### Prerequisites Checklist

Before you begin, make sure you have:
- [ ] **Python 3.10+** installed (check with `python --version`)
- [ ] **LLM API Key** from OpenAI, Anthropic, or Groq
- [ ] **Terminal/Command prompt** ready

### Step 1: Install (10 seconds)

```bash
# Using uv (recommended)
uv add omnicoreagent

# Or with pip
pip install omnicoreagent
```

### Step 2: Set API Key (10 seconds)

```bash
# Create .env file in your project directory
echo "LLM_API_KEY=your_openai_api_key_here" > .env

# Or manually create .env file with:
# LLM_API_KEY=sk-your-actual-api-key-here
```

> **💡 Tip**: Get your API key from [OpenAI](https://platform.openai.com/api-keys), [Anthropic](https://console.anthropic.com/), or [Groq](https://console.groq.com/)

### Step 3: Create Your First Agent (30 seconds)

Create a file `my_first_agent.py`:

```python
import asyncio
from omnicoreagent import OmniAgent

async def main():
    # Create your agent
    agent = OmniAgent(
        name="my_agent",
        system_instruction="You are a helpful assistant.",
        model_config={"provider": "openai", "model": "gpt-4o"}
    )
    
    # Run your agent
    result = await agent.run("Hello, world!")
    print(result['response'])
    
    # Clean up
    await agent.cleanup()

if __name__ == "__main__":
    asyncio.run(main())
```

Run it:
```bash
python my_first_agent.py
```

**✅ Success!** You just built an AI agent with:
- ✅ Session management
- ✅ Memory persistence
- ✅ Event streaming
- ✅ Tool orchestration
- ✅ Error handling
- ✅ Production-ready infrastructure

### 🚨 Common First Errors & Fixes

| **Error** | **Fix** |
|-----------|---------|
| `Invalid API key` | Check `.env` file: `LLM_API_KEY=sk-...` (no quotes, no spaces) |
| `ModuleNotFoundError: omnicoreagent` | Run: `pip install omnicoreagent` |
| `RuntimeError: Event loop is closed` | Make sure you use `asyncio.run(main())` |
| `AttributeError: 'coroutine' object has no attribute 'response'` | Make sure you `await agent.run()` |

### Next Steps

- 📖 **Learn More**: See [Core Features](#-core-features) for advanced capabilities
- 🎯 **See Examples**: Check [Examples](#-examples) for real-world use cases
- 🚀 **Production Ready**: See [Production Examples](#-production-examples) for full setups

---

## 🏗️ Architecture Overview

OmniCoreAgent is built on a modular, production-ready architecture:

```
OmniCoreAgent Framework
├── 🤖 Core Agent System
│   ├── OmniAgent (Main Agent Class)
│   ├── ReactAgent (Reasoning Engine)
│   ├── Tool Orchestration
│   └── Session Management
│
├── 🧠 Memory System (Multi-Backend)
│   ├── InMemoryStore (Fast Development)
│   ├── RedisMemoryStore (Production Persistence)
│   ├── DatabaseMemory (PostgreSQL/MySQL/SQLite)
│   ├── MongoDBMemory (Document Storage)
│   └── Memory Management (Working Memory)
│
├── 📡 Event System
│   ├── InMemoryEventStore (Development)
│   ├── RedisStreamEventStore (Production)
│   └── Real-Time Event Streaming
│
├── 🛠️ Tool System
│   ├── Local Tools Registry (Python Functions)
│   ├── MCP Tools Integration (Built-in Client)
│   ├── Advance Tool Use
│   └── Memory Tool Backend (Persistent Working Memory)
│
├── 🚁 Background Agent System
│   ├── Background Agent Manager
│   ├── Task Registry
│   ├── APScheduler Backend
│   └── Lifecycle Management
│
├── 🔄 Workflow Agents
│   ├── SequentialAgent (Step-by-step chaining)
│   ├── ParallelAgent (Concurrent execution)
│   └── RouterAgent (Intelligent routing)
│
└── 🔌 Built-in MCP Client
    ├── Model Context Protocol server support
    ├── Multiple transport protocols (stdio, Streamable_HTTP, SSE)
    └── Seamless tool integration
```

---

## 📚 Glossary (For Non-Technical Readers)

Understanding key terms helps you get the most out of OmniCoreAgent:

- **AI Agent**: A program that can think, make decisions, and use tools (like APIs or databases) to complete tasks autonomously. Unlike simple chatbots, agents can plan multi-step workflows and adapt based on results.

- **LLM (Large Language Model)**: The "brain" of your agent. Examples include GPT-4, Claude, Gemini. These models understand language and can reason about tasks.

- **Tool**: A function your agent can call to perform actions. Examples: "get weather", "send email", "query database", "read file". Tools extend what your agent can do beyond just talking.

- **Memory**: How your agent remembers past conversations and context. OmniCoreAgent supports multiple memory backends (in-memory, Redis, databases) for different use cases.

- **Session**: A single conversation with your agent. Sessions help maintain context and separate different user interactions.

- **MCP (Model Context Protocol)**: A standard protocol for connecting AI agents to external tools and services. OmniCoreAgent has built-in MCP client support.

- **Background Agent**: An agent that runs automatically on a schedule, without human interaction. Perfect for monitoring, periodic tasks, or automation.

- **Workflow Agent**: A system that coordinates multiple agents to work together. Examples: Sequential (one after another), Parallel (at the same time), Router (intelligent routing).

- **Observability**: Tools and metrics that help you monitor, debug, and optimize your agents in production. Includes tracing, logging, and performance metrics.

---

## 🎯 Core Features

### 1. 🤖 OmniAgent - The Heart of the Framework

**OmniAgent** is the main class that powers everything. It's a sophisticated agent with enterprise-grade capabilities:

#### Common Workflows

**Basic Agent**:
```python
agent = OmniAgent(
    name="assistant",
    system_instruction="You are a helpful assistant.",
    model_config={"provider": "openai", "model": "gpt-4o"}
)
result = await agent.run("What is Python?")
```

**Agent with Custom Tools**:
```python
from omnicoreagent import OmniAgent, ToolRegistry

tools = ToolRegistry()
@tools.register_tool("get_weather")
def get_weather(city: str) -> str:
    return f"Weather in {city}: Sunny, 25°C"

agent = OmniAgent(
    name="weather_agent",
    system_instruction="You help with weather information.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    local_tools=tools
)
```

**Production Agent with Memory & Events**:
```python
from omnicoreagent import OmniAgent, MemoryRouter, EventRouter

agent = OmniAgent(
    name="production_agent",
    system_instruction="You are a production agent.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    memory_router=MemoryRouter("redis"),
    event_router=EventRouter("redis_stream"),
    agent_config={
        "max_steps": 20,
        "memory_tool_backend": "local"
    }
)
```

#### Key Methods

```python
from omnicoreagent import OmniAgent

agent = OmniAgent(
    name="my_agent",
    system_instruction="You are a helpful assistant.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    local_tools=tool_registry,  # Your custom tools
    mcp_tools=[...],  # MCP server connections
    memory_router=MemoryRouter("redis"),
    event_router=EventRouter("redis_stream"),
    agent_config={
        "max_steps": 15,
        "tool_call_timeout": 30,
        "memory_results_limit": 5,
        "enable_advanced_tool_use": True,
        "memory_tool_backend": "local"
    }
)

# Core Methods
await agent.run(query)                          # Execute agent task (session_id auto-generated)
await agent.run(query, session_id="user_123")   # Execute with specific session_id for context
await agent.connect_mcp_servers()                # Connect to MCP servers
await agent.list_all_available_tools()           # Get all tools (MCP + local)
await agent.get_session_history(session_id)      # Retrieve conversation history
await agent.clear_session_history(session_id)     # Clear history (session_id optional, clears all if None)
await agent.stream_events(session_id)           # Stream real-time events
await agent.get_events(session_id)               # Get event history
agent.get_memory_store_type()                    # Get current memory backend
agent.get_event_store_type()                    # Get current event backend
agent.switch_event_store("redis_stream")         # Switch event backend at runtime (in_memory ↔ redis_stream)
agent.swith_memory_store("redis")                # Switch memory backend at runtime (redis, mongodb, database, in_memory)
agent.swith_memory_store("mongodb")              # Switch to MongoDB
agent.swith_memory_store("database")             # Switch to PostgreSQL/MySQL/SQLite
agent.swith_memory_store("in_memory")            # Switch to in-memory
await agent.cleanup()                            # Clean up resources
```

#### Agent Configuration

```python
agent_config = {
    # Execution Limits
    "max_steps": 15,                    # Maximum reasoning steps
    "tool_call_timeout": 30,            # Tool execution timeout (seconds)
    "request_limit": 0,                 # 0 = unlimited, >0 for limits
    "total_tokens_limit": 0,            # 0 = unlimited, >0 for token cap
    
    # Memory Configuration
    "memory_config": {
        "mode": "sliding_window",       # or "token_budget"
        "value": 10000                  # Window size or token limit
    },
    
    
    # Advanced Tool Use
    "enable_advanced_tool_use": True,  # Enable advanced tool use
    
    
    # Memory Tool Backend for filesystem persistance storage
    "memory_tool_backend": "local"       # "local", or None
}
```

---

### 2. 🧠 Multi-Tier Memory System

OmniCoreAgent provides **5 memory backends** with intelligent routing and **runtime switching**—truly plug and play!

#### 🎯 Runtime Switching (Plug & Play)

**The Beauty of OmniCoreAgent**: Switch memory backends at runtime without restarting or losing data. Start with Redis, switch to MongoDB, then to PostgreSQL—all on the fly!

```python
from omnicoreagent import OmniAgent, MemoryRouter

# Start with Redis
agent = OmniAgent(
    name="my_agent",
    memory_router=MemoryRouter("redis"),
    model_config={"provider": "openai", "model": "gpt-4o"}
)

# Use Redis for a while...
result = await agent.run("Store this information")

# Switch to MongoDB at runtime - no restart needed!
agent.swith_memory_store("mongodb")
result = await agent.run("Now using MongoDB backend")

# Switch to PostgreSQL
agent.swith_memory_store("database")  # Uses DATABASE_URL env var

# Switch to in-memory for testing
agent.swith_memory_store("in_memory")

# Switch back to Redis
agent.swith_memory_store("redis")
```

**Use Cases**:
- **Development → Production**: Start with `in_memory`, switch to `redis` when ready
- **Migration**: Switch from one backend to another without downtime
- **Testing**: Quickly switch between backends for testing
- **Cost Optimization**: Use cheaper backends for development, premium for production
- **A/B Testing**: Test different backends with the same agent

#### Memory Router

```python
from omnicoreagent import MemoryRouter

# In-Memory (Fast Development)
memory = MemoryRouter("in_memory")

# Redis (Production Persistence)
memory = MemoryRouter("redis")  # Uses REDIS_URL env var

# Database (PostgreSQL/MySQL/SQLite)
memory = MemoryRouter("database")  # Uses DATABASE_URL env var
# Supports: postgresql://, mysql://, sqlite://

# MongoDB (Document Storage)
memory = MemoryRouter("mongodb")  # Uses MONGODB_URI env var

# Runtime Switching - Works with any backend!
memory.swith_memory_store("redis")      # Switch to Redis
memory.swith_memory_store("mongodb")    # Switch to MongoDB
memory.swith_memory_store("database")   # Switch to PostgreSQL/MySQL/SQLite
memory.swith_memory_store("in_memory")  # Switch to in-memory
```

#### Memory Strategies

```python
# Sliding Window - Keep last N messages
memory.set_memory_config(mode="sliding_window", value=100)

# Token Budget - Keep under token limit
memory.set_memory_config(mode="token_budget", value=5000)
```


**Memory Types:**
- **Working Memory**: Active task state (via Memory Tool Backend)

**What You Get:**
- **Long-term Memory**: Persistent storage across sessions
- **Multi-session Context**: Remember information across different conversations
- **Automatic Summarization**: Intelligent memory compression for efficiency

---

### 3. 📡 Event System

Real-time event streaming for monitoring and debugging with **runtime switching**—plug and play!

#### 🎯 Runtime Switching (Plug & Play)

**The Beauty of OmniCoreAgent**: Switch event router at runtime. Start with `in_memory` for development, switch to `redis_stream` for production—all without restarting!

```python
from omnicoreagent import OmniAgent, EventRouter

# Start with in-memory events (fast for development)
agent = OmniAgent(
    name="my_agent",
    event_router=EventRouter("in_memory"),
    model_config={"provider": "openai", "model": "gpt-4o"}
)

# Use in-memory for development...
result = await agent.run("Test query")

# Switch to Redis Streams at runtime for production persistence!
agent.switch_event_store("redis_stream")
result = await agent.run("Now events are persisted in Redis")

# Switch back to in-memory if needed
agent.switch_event_store("in_memory")
```

**Use Cases**:
- **Development → Production**: Start with `in_memory`, switch to `redis_stream` when deploying
- **Testing**: Quickly switch between backends for testing
- **Performance Tuning**: Use in-memory for speed, Redis for persistence
- **Cost Management**: Use in-memory for development, Redis for production

#### Event Backends

```python
from omnicoreagent import EventRouter

# In-Memory Events (Development - Fast)
events = EventRouter("in_memory")

# Redis Streams (Production - Persistent)
events = EventRouter("redis_stream")  # Uses REDIS_URL env var

# Runtime Switching - Works seamlessly!
events.switch_event_store("redis_stream")  # Switch to Redis Streams
events.switch_event_store("in_memory")     # Switch back to in-memory
```

#### Event Types

```python
# Event Types Available:
# - user_message
# - agent_message
# - tool_call_started
# - tool_call_result
# - tool_call_error
# - final_answer
# - agent_thought
# - background_task_started
# - background_task_completed
# - background_task_error
```

#### Usage Examples

```python
# Stream events in real-time
async for event in agent.stream_events(session_id):
    print(f"{event.type}: {event.payload}")

# Get event history
history = await agent.get_events(session_id)

# Switch event backend and continue streaming
agent.switch_event_store("redis_stream")
async for event in agent.stream_events(session_id):
    print(f"Persisted: {event.type}")
```

---

### 4. 🛠️ Local Tools System

Register any Python function as an AI tool:

```python
from omnicoreagent import ToolRegistry

tool_registry = ToolRegistry()

@tool_registry.register_tool("calculate_area")
def calculate_area(length: float, width: float) -> str:
    """Calculate the area of a rectangle."""
    area = length * width
    return f"Area: {area} square units"

@tool_registry.register_tool(
    name="analyze_data",
    description="Analyze data and return insights",
    inputSchema={
        "type": "object",
        "properties": {
            "data": {"type": "string", "description": "Data to analyze"}
        },
        "required": ["data"]
    }
)
def analyze_data(data: str) -> str:
    """Analyze data and return insights."""
    return f"Analysis: {len(data)} characters processed"

# Use with OmniAgent
agent = OmniAgent(
    name="my_agent",
    system_instruction="You are a helpful assistant.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    local_tools=tool_registry  # Your custom tools!
)
```

**The agent automatically:**
- ✅ Discovers all registered tools
- ✅ Generates tool schemas
- ✅ Handles tool execution
- ✅ Manages errors gracefully
- ✅ Combines with MCP tools seamlessly

---

### 5. 💾 Memory Tool Backend

Persistent working memory for long-running tasks. **When to use**: Enable this when your agent needs to save intermediate work, track progress across multiple steps, or resume tasks after interruption.

```python
agent_config = {
    "memory_tool_backend": "local"  # Enable persistent memory
}

# Agent automatically gets access to memory_* tools:
# - memory_view: Inspect memory contents
# - memory_create_update: Create/append/overwrite files
# - memory_str_replace: Replace strings in files
# - memory_insert: Insert text at specific line
# - memory_delete: Delete files
# - memory_rename: Rename/move files
# - memory_clear_all: Clear all memory

# Files stored in ./memories/ directory
# Safe, concurrent access with file locks
# Path traversal protection
```

**Use Cases:**
- **Long-running workflows**: Save progress as agent works through complex tasks
- **Resumable tasks**: Agent can continue where it left off after interruption
- **Progress tracking**: Monitor multi-step processes
- **Intermediate state storage**: Store data between agent reasoning steps
- **Multi-step planning**: Agent can plan, save plan, execute, and update

**Example**: A code generation agent can save its plan, write code incrementally, and resume if interrupted.

---

### 6. 🚁 Background Agents

Autonomous agents that run independently:

```python
from omnicoreagent import (
    OmniAgent,
    BackgroundAgentService,
    MemoryRouter,
    EventRouter,
    ToolRegistry
)

# Initialize background service
memory_router = MemoryRouter("redis")
event_router = EventRouter("redis_stream")
bg_service = BackgroundAgentService(memory_router, event_router)
bg_service.start_manager()

# Create tool registry
tool_registry = ToolRegistry()

@tool_registry.register_tool("monitor_system")
def monitor_system() -> str:
    """Monitor system resources."""
    import psutil
    return f"CPU: {psutil.cpu_percent()}%, Memory: {psutil.virtual_memory().percent}%"

# Create background agent
agent_config = {
    "agent_id": "system_monitor",
    "system_instruction": "You are a system monitoring agent.",
    "model_config": {
        "provider": "openai",
        "model": "gpt-4o-mini",
        "temperature": 0.3
    },
    "agent_config": {
        "max_steps": 10,
        "tool_call_timeout": 60
    },
    "interval": 300,  # Run every 5 minutes
    "task_config": {
        "query": "Monitor system resources and alert if CPU > 80%",
        "schedule": "every 5 minutes",
        "interval": 300,
        "max_retries": 2,
        "retry_delay": 30
    },
    "local_tools": tool_registry
}

result = await bg_service.create(agent_config)

# Agent Management
bg_service.start_agent("system_monitor")
bg_service.pause_agent("system_monitor")
bg_service.resume_agent("system_monitor")
bg_service.stop_agent("system_monitor")
bg_service.remove_task("system_monitor")

# Status Monitoring
status = bg_service.get_agent_status("system_monitor")
agents = bg_service.list()  # List all agents
```

**Features:**
- ✅ Flexible scheduling (interval-based, cron support planned)
- ✅ Lifecycle management (create, pause, resume, delete)
- ✅ Health monitoring
- ✅ Automatic retries
- ✅ Event broadcasting
- ✅ Full OmniAgent capabilities

---

### 7. 🔄 Workflow Agents

Orchestrate multiple agents for complex tasks:

#### SequentialAgent

Chain agents step-by-step:

```python
from omnicoreagent import OmniAgent, SequentialAgent

# Create agents
agent1 = OmniAgent(name="analyzer", ...)
agent2 = OmniAgent(name="processor", ...)
agent3 = OmniAgent(name="reporter", ...)

# Chain them
seq_agent = SequentialAgent(sub_agents=[agent1, agent2, agent3])
await seq_agent.initialize()

result = await seq_agent.run(
    initial_task="Analyze this data and generate a report"
)
# Output from agent1 → input to agent2 → input to agent3
```

#### ParallelAgent

Run agents concurrently:

```python
from omnicoreagent import ParallelAgent

par_agent = ParallelAgent(sub_agents=[agent1, agent2, agent3])
await par_agent.initialize()

results = await par_agent.run(
    agent_tasks={
        "analyzer": "Analyze the data",
        "processor": "Process the results",
        "reporter": None  # Uses system instruction
    }
)
# All agents run simultaneously
```

#### RouterAgent

Intelligent task routing:

```python
from omnicoreagent import RouterAgent

router = RouterAgent(
    sub_agents=[code_agent, data_agent, research_agent],
    model_config={"provider": "openai", "model": "gpt-4o"},
    agent_config={"max_steps": 10},
    memory_router=MemoryRouter("redis"),
    event_router=EventRouter("redis_stream")
)

await router.initialize()
result = await router.run(task="Find and summarize recent AI research")
# RouterAgent analyzes task and routes to best agent
```

---

### 8. 🧠 Advanced Tool Use

Automatically discover and retrieve relevant tools using semantic search. **The Problem**: When you have hundreds of tools, manually selecting which ones to use is impossible. **The Solution**: OmniCoreAgent automatically finds the right tools based on what the agent needs to do.

**Before (Manual Tool Selection)**:
```python
# ❌ You have to manually specify which tools to use
# ❌ Doesn't scale with 100+ tools
# ❌ Agent might miss relevant tools
tools = [tool1, tool2, tool3]  # Limited selection
```

**After (Semantic Tool Knowledge Base)**:
```python
# ✅ Agent automatically finds relevant tools
# ✅ Scales to unlimited tools
# ✅ Context-aware selection
agent_config = {
    "enable_advanced_tool_use": True,
    
}


```

**How It Works:**
1. All tools are automatically embedded into a vector database
2. When agent needs tools, it searches semantically (by meaning)
3. Returns most relevant tools for the current task
4. Falls back to keyword search if semantic search finds nothing

**Benefits:**
- ✅ **Scales to unlimited tools**: Works with 10 or 10,000 tools
- ✅ **Context-aware tool selection**: Finds tools based on task meaning
- ✅ **No manual registry management**: Automatic tool discovery
- ✅ **Automatic tool indexing**: New tools are automatically available

---

### 9. 📊 Production Observability

#### Opik Tracing & Observability Setup

**Monitor and optimize your AI agents with production-grade observability:**

**🚀 Quick Setup:**

1. **Sign up for Opik** (Free & Open Source):
   - Visit: **[https://www.comet.com/signup?from=llm](https://www.comet.com/signup?from=llm)**
   - Create your account and get your API key and workspace name

2. **Add to your `.env` file:**
   ```bash
   OPIK_API_KEY=your_opik_api_key_here
   OPIK_WORKSPACE=your_opik_workspace_name
   ```

**✨ What You Get Automatically:**

Once configured, OmniCoreAgent automatically tracks:
- **🔥 LLM Call Performance**: Execution time, token usage, response quality
- **🛠️ Tool Execution Traces**: Which tools were used and how long they took
- **🧠 Memory Operations**: memory retrieval performance
- **🤖 Agent Workflow**: Complete trace of multi-step agent reasoning
- **📊 System Bottlenecks**: Identify exactly where time is spent

**📈 Benefits:**
- **Performance Optimization**: See which LLM calls or tools are slow
- **Cost Monitoring**: Track token usage and API costs
- **Debugging**: Understand agent decision-making processes
- **Production Monitoring**: Real-time observability for deployed agents
- **Zero Code Changes**: Works automatically with existing agents

**🔍 Example: What You'll See**

```
Agent Execution Trace:
├── agent_execution: 4.6s
│   ├── tools_registry_retrieval: 0.02s ✅
│   ├── memory_retrieval_step: 0.08s ✅
│   ├── llm_call: 4.5s ⚠️ (bottleneck identified!)
│   ├── response_parsing: 0.01s ✅
│   └── action_execution: 0.03s ✅
```

**💡 Pro Tip**: Opik is completely optional. If you don't set the credentials, OmniCoreAgent works normally without tracing.

#### Metrics & Monitoring

OmniCoreAgent provides built-in metrics collection for production monitoring:

```python
# Metrics are automatically collected when using production examples
# See examples/devops_copilot_agent/ for Prometheus integration
# See examples/deep_code_agent/ for comprehensive monitoring

# Key Metrics Tracked:
# - Request count and latency
# - Token usage per request
# - Tool execution time
# - Memory operations
# - Error rates
# - Agent step counts
```

**Production Examples Include**:
- **Prometheus-compatible endpoints**: `/metrics` endpoint for scraping
- **Real-time performance tracking**: Monitor agent performance live
- **Custom metrics**: Add your own business metrics
- **Alerting**: Set up alerts based on metrics

See [Production Examples](#-production-examples) for complete implementations.

---

## 🎯 Production Examples

### 1. DevOps Copilot Agent

A production-ready DevOps assistant with:
- ✅ Safe bash command execution
- ✅ Rate limiting
- ✅ Audit logging
- ✅ Prometheus metrics
- ✅ Health checks
- ✅ Redis persistence

**Location:** `examples/devops_copilot_agent/`

**How to Run**:
```bash
cd examples/devops_copilot_agent
# Follow the README in that directory for setup instructions
```

**Prerequisites**:
- Redis running (for persistence)
- LLM API key configured
- Docker (for deployment)

**Features**:
- Configuration management
- Observability (metrics, logging, audit)
- Security (rate limiting, command filtering)
- Health checks
- Docker deployment

### 2. Deep Code Agent

An advanced coding agent with:
- ✅ Sandbox code execution
- ✅ Memory tool backend
- ✅ Session workspaces
- ✅ Code analysis tools
- ✅ Test execution
- ✅ Production observability

**Location:** `examples/deep_code_agent/`

**How to Run**:
```bash
cd examples/deep_code_agent
# Follow the README in that directory for setup instructions
```

**Prerequisites**:
- LLM API key configured
- Optional: Vector database for enhanced memory

**Features**:
- Secure sandbox execution
- Persistent working memory
- Code generation and testing
- Full observability stack

---

### 10. 🌐 Universal Model Support

OmniCoreAgent is **model-agnostic by design** through LiteLLM integration. Use OpenAI, Anthropic Claude, Google Gemini, Ollama, or any LLM provider. Switch models without changing agent code. Your logic stays consistent regardless of the underlying model.

#### Multi-Provider LLM Support

OmniCoreAgent uses **LiteLLM** for unified access to 100+ models:

```python
model_config = {
    # OpenAI
    "provider": "openai",
    "model": "gpt-4o",
    
    # Anthropic
    "provider": "anthropic",
    "model": "claude-3-5-sonnet-20241022",
    
    # Groq (Ultra-fast)
    "provider": "groq",
    "model": "llama-3.1-8b-instant",
    
    # Azure OpenAI
    "provider": "azureopenai",
    "model": "gpt-4",
    "azure_endpoint": "https://your-resource.openai.azure.com",
    
    # Ollama (Local)
    "provider": "ollama",
    "model": "llama3.1:8b",
    "ollama_host": "http://localhost:11434",
    
    # OpenRouter (200+ models)
    "provider": "openrouter",
    "model": "anthropic/claude-3.5-sonnet"
}
```

**Supported Providers:**
- OpenAI (GPT-4, GPT-3.5, etc.)
- Anthropic (Claude 3.5 Sonnet, Claude 3 Haiku, etc.)
- Google (Gemini Pro, Gemini Flash)
- Groq (Llama, Mixtral, Gemma)
- DeepSeek (DeepSeek-V3, DeepSeek-Coder)
- Mistral
- Azure OpenAI
- OpenRouter (200+ models)
- Ollama (local models)

**Why This Matters:**
- **Cost Optimization**: Use cheaper models for simple tasks, powerful models for complex reasoning
- **Flexibility**: Switch providers without code changes
- **Consistency**: Same agent logic works across all providers
- **Future-Proof**: New models automatically supported through LiteLLM

---

### 11. 🔌 Built-in MCP Client

OmniCoreAgent includes **built-in support for Model Context Protocol (MCP) servers**, allowing your agents to seamlessly connect to external tools and services without additional setup. This is a core feature that enables your agents to interact with filesystems, databases, APIs, and any MCP-compatible service.

#### Quick Integration

```python
agent = OmniAgent(
    name="my_agent",
    system_instruction="You are a helpful assistant.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    mcp_tools=[
        # stdio Transport - Local MCP servers
        {
            "name": "filesystem",
            "transport_type": "stdio",
            "command": "npx",
            "args": ["-y", "@modelcontextprotocol/server-filesystem", "/home"]
        },
        # HTTP Transport - Remote MCP servers
        {
            "name": "github",
            "transport_type": "streamable_http",
            "url": "http://localhost:8080/mcp",
            "headers": {"Authorization": "Bearer your-token"}
        }
    ]
)

await agent.connect_mcp_servers()  # Connect to all servers
tools = await agent.list_all_available_tools()  # Get all tools (MCP + local)
```

#### Supported Transports

- **stdio**: Direct process communication (local MCP servers)
- **sse**: Server-Sent Events (HTTP-based streaming)
- **streamable_http**: HTTP with streaming support
- **docker**: Container-based servers
- **npx**: NPX package execution

#### Authentication Methods

- **OAuth 2.0**: Automatic callback server (starts on `localhost:3000`)
- **Bearer Tokens**: Simple token-based authentication
- **Custom Headers**: Flexible header configuration

#### Key Benefits

- ✅ **No Additional Setup**: Built directly into OmniAgent
- ✅ **Seamless Integration**: MCP tools work alongside local tools
- ✅ **Multiple Transports**: Support for stdio, HTTP, SSE, Docker, NPX
- ✅ **Automatic Discovery**: All MCP tools automatically available to agent
- ✅ **Unified Tool Access**: Use `list_all_available_tools()` to see MCP + local tools
- ✅ **Production Ready**: Handles connection errors, retries, and cleanup

#### Example: Agent with Filesystem Access

```python
agent = OmniAgent(
    name="file_agent",
    system_instruction="You can read and write files.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    mcp_tools=[{
        "name": "filesystem",
        "transport_type": "stdio",
        "command": "npx",
        "args": ["-y", "@modelcontextprotocol/server-filesystem", "/home/user"]
    }]
)

await agent.connect_mcp_servers()
result = await agent.run("List all Python files in the current directory")
# Agent can now use filesystem tools from MCP server
```

#### Example: Agent with Multiple MCP Servers

```python
agent = OmniAgent(
    name="multi_tool_agent",
    system_instruction="You have access to filesystem and GitHub.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    mcp_tools=[
        {
            "name": "filesystem",
            "transport_type": "stdio",
            "command": "npx",
            "args": ["-y", "@modelcontextprotocol/server-filesystem", "/home"]
        },
        {
            "name": "github",
            "transport_type": "streamable_http",
            "url": "http://localhost:8080/mcp",
            "headers": {"Authorization": "Bearer github-token"}
        }
    ]
)

await agent.connect_mcp_servers()
# Agent now has access to both filesystem and GitHub tools
```

**Note**: For standalone MCP client usage (CLI tool), see the [MCP Client CLI](#-mcp-client-cli-commands) section at the end of this document.



---

## 📦 Installation & Setup

### Requirements

- Python 3.10+
- LLM API key (OpenAI, Anthropic, Groq, etc.)

### Optional Dependencies (For Advanced Features)

- **Redis**: For persistent memory and events (`memory_store_type="redis"`, `event_store_type="redis_stream"`)
- **PostgreSQL/MySQL**: For database memory (`memory_store_type="database"`)
- **MongoDB**: For document storage (`memory_store_type="mongodb"`)
- **Opik**: For tracing and observability (production monitoring)

### Installation

```bash
# Using uv (recommended)
uv add omnicoreagent

# Or with pip
pip install omnicoreagent
```

### Environment Variables

```bash
# ===============================================
# REQUIRED: AI Model API Key (Choose one provider)
# ===============================================
LLM_API_KEY=your_openai_api_key_here
# OR for other providers:
# LLM_API_KEY=your_anthropic_api_key_here
# LLM_API_KEY=your_groq_api_key_here
# LLM_API_KEY=your_azure_openai_api_key_here


# ===============================================
# OPTIONAL: Persistent Memory Storage
# ===============================================
# Redis - for memory_store_type="redis" (defaults to: redis://localhost:6379/0)
# REDIS_URL=redis://your-remote-redis:6379/0
# REDIS_URL=redis://:password@localhost:6379/0  # With password

# Database - for memory_store_type="database"
# DATABASE_URL=sqlite:///omnicoreagent_memory.db
# DATABASE_URL=postgresql://user:password@localhost:5432/omnicoreagent
# DATABASE_URL=mysql://user:password@localhost:3306/omnicoreagent

# MongoDB - for memory_store_type="mongodb" (defaults to: mongodb://localhost:27017/omnicoreagent)
# MONGODB_URI="your_mongodb_connection_string"
# MONGODB_DB_NAME="db name"

# ===============================================
# OPTIONAL: Tracing & Observability
# ===============================================
# For advanced monitoring and performance optimization
# 🔗 Sign up: https://www.comet.com/signup?from=llm
OPIK_API_KEY=your_opik_api_key_here
OPIK_WORKSPACE=your_opik_workspace_name
```

> **💡 Quick Start**: Just set `LLM_API_KEY` and you're ready to go! Add other variables only when you need advanced features.

---

## 📚 Examples

### Basic Agent

```python
import asyncio
from omnicoreagent import OmniAgent

async def main():
    agent = OmniAgent(
        name="assistant",
        system_instruction="You are a helpful assistant.",
        model_config={"provider": "openai", "model": "gpt-4o"}
    )
    
    # Run without session_id (auto-generated)
    result = await agent.run("What is the capital of France?")
    print(result["response"])
    print(f"Session ID: {result['session_id']}")
    
    # Run with same session_id for context continuity
    result2 = await agent.run("What is its population?", session_id=result["session_id"])
    print(result2["response"])
    
    await agent.cleanup()

asyncio.run(main())
```

**Note**: `session_id` is optional. If omitted, a new session is created automatically. Use the same `session_id` across multiple calls to maintain conversation context.

### Agent with Custom Tools

```python
from omnicoreagent import OmniAgent, ToolRegistry

tool_registry = ToolRegistry()

@tool_registry.register_tool("get_weather")
def get_weather(city: str) -> str:
    """Get weather for a city."""
    return f"Weather in {city}: Sunny, 25°C"

agent = OmniAgent(
    name="weather_agent",
    system_instruction="You help users with weather information.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    local_tools=tool_registry
)

result = await agent.run("What's the weather in Tokyo?")
```

### Agent with MCP Servers

```python
agent = OmniAgent(
    name="mcp_agent",
    system_instruction="You have access to filesystem and GitHub tools.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    mcp_tools=[
        {
            "name": "filesystem",
            "transport_type": "stdio",
            "command": "npx",
            "args": ["-y", "@modelcontextprotocol/server-filesystem", "/home"]
        }
    ]
)

await agent.connect_mcp_servers()
result = await agent.run("List files in /home directory")
```

### Production Agent with All Features

```python
from omnicoreagent import (
    OmniAgent,
    ToolRegistry,
    MemoryRouter,
    EventRouter
)

# Memory & Events
memory = MemoryRouter("redis")
events = EventRouter("redis_stream")

# Custom Tools
tools = ToolRegistry()
@tools.register_tool("analyze")
def analyze(data: str) -> str:
    return f"Analyzed: {len(data)} chars"

# Agent
agent = OmniAgent(
    name="production_agent",
    system_instruction="You are a production agent.",
    model_config={"provider": "openai", "model": "gpt-4o"},
    local_tools=tools,
    mcp_tools=[...],
    memory_router=memory,
    event_router=events,
    agent_config={
        "max_steps": 20,
        "enable_advanced_tool_use": True,
        "memory_tool_backend": "local",
        "memory_results_limit": 10
    }
)

await agent.connect_mcp_servers()
result = await agent.run("Process this data", session_id="user_123")
```

---

## 🎓 Learning Resources

### Example Projects

#### Basic Examples
```bash
# Simple introduction
python examples/cli/basic.py

# Complete OmniAgent demo - All features showcase
python examples/cli/run_omni_agent.py

```

#### Custom Agents
```bash
# Background agents
python examples/background_agent_example.py

# Custom agent implementations
python examples/custom_agents/e_commerce_personal_shopper_agent.py
python examples/custom_agents/flightBooking_agent.py
python examples/custom_agents/real_time_customer_support_agent.py
```

#### Workflow Agents
```bash
# Sequential agent chaining
python examples/workflow_agents/sequential_agent.py

# Parallel agent execution
python examples/workflow_agents/parallel_agent.py

# Router agent (intelligent routing)
python examples/workflow_agents/router_agent.py
```

#### Web Applications
```bash
# FastAPI integration
python examples/fast_api_iml.py

# Full web interface
python examples/enhanced_web_server.py
# Open http://localhost:8000
```

#### Production Examples
- **DevOps Copilot Agent**: `examples/devops_copilot_agent/`
  - Production-ready DevOps assistant
  - Safe bash command execution
  - Rate limiting, audit logging, Prometheus metrics
  - Health checks, Redis persistence
  
- **Deep Code Agent**: `examples/deep_code_agent/`
  - Advanced coding agent
  - Sandbox code execution
  - Memory tool backend
  - Session workspaces
  - Code analysis and test execution

### Documentation

- **Getting Started**: See examples above
- **API Reference**: Check source code docstrings
- **Architecture**: See `docs/advanced/architecture.md`
- **Complete Documentation**: [OmniCoreAgent Docs](https://omnirexflora-labs.github.io/omnicoreagent)

### Build Documentation Locally

```bash
# Install documentation dependencies
pip install mkdocs mkdocs-material

# Serve documentation locally
mkdocs serve
# Open http://127.0.0.1:8000

# Build static documentation
mkdocs build
```

---

## 🔧 Configuration Reference

### Agent Configuration

```python
agent_config = {
    # Execution
    "agent_name": "my_agent",
    "max_steps": 15,
    "tool_call_timeout": 30,
    "request_limit": 0,  # 0 = unlimited
    "total_tokens_limit": 0,  # 0 = unlimited
    
    # Memory
    "memory_config": {"mode": "sliding_window", "value": 10000},
    
    # Tools
    "enable_advanced_tool_use": True,
    
    
    # Memory Tool
    "memory_tool_backend": "local"  # or "s3", "db", None
}
```

### Model Configuration

```python
model_config = {
    "provider": "openai",  # or anthropic, groq, etc.
    "model": "gpt-4o",
    "temperature": 0.7,
    "max_tokens": 2000,
    "top_p": 0.95
}
```

### MCP Tool Configuration

#### Basic stdio Configuration

```python
mcp_tools = [
    {
        "name": "filesystem",
        "transport_type": "stdio",
        "command": "npx",
        "args": ["-y", "@modelcontextprotocol/server-filesystem", "/home"]
    }
]
```

#### HTTP Configuration with Bearer Token

```python
mcp_tools = [
    {
        "name": "github",
        "transport_type": "streamable_http",
        "url": "http://localhost:8080/mcp",
        "headers": {
            "Authorization": "Bearer your-token"
        },
        "timeout": 60
    }
]
```

#### HTTP Configuration with OAuth

```python
mcp_tools = [
    {
        "name": "oauth_server",
        "transport_type": "streamable_http",
        "auth": {
            "method": "oauth"
        },
        "url": "http://localhost:8000/mcp"
    }
]
```

#### SSE Configuration

```python
mcp_tools = [
    {
        "name": "sse_server",
        "transport_type": "sse",
        "url": "http://localhost:3000/sse",
        "headers": {
            "Authorization": "Bearer token"
        },
        "timeout": 60,
        "sse_read_timeout": 120
    }
]
```

### Server Configuration JSON Examples

#### Complete Configuration with Multiple Providers

```json
{
  "AgentConfig": {
    "tool_call_timeout": 30,
    "max_steps": 15,
    "request_limit": 0,
    "total_tokens_limit": 0,
    "enable_advanced_tool_use": true,
    "memory_tool_backend": "local"
  },
  "LLM": {
    "provider": "openai",
    "model": "gpt-4o",
    "temperature": 0.7,
    "max_tokens": 2000,
    "max_context_length": 30000,
    "top_p": 0.95
  },
  "mcpServers": {
    "filesystem": {
      "transport_type": "stdio",
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/home"]
    },
    "github": {
      "transport_type": "streamable_http",
      "url": "http://localhost:8080/mcp",
      "headers": {
        "Authorization": "Bearer your-token"
      }
    }
  }
}
```

#### Anthropic Claude Configuration

```json
{
  "LLM": {
    "provider": "anthropic",
    "model": "claude-3-5-sonnet-20241022",
    "temperature": 0.7,
    "max_tokens": 4000,
    "max_context_length": 200000,
    "top_p": 0.95
  }
}
```

#### Groq Configuration (Ultra-Fast)

```json
{
  "LLM": {
    "provider": "groq",
    "model": "llama-3.1-8b-instant",
    "temperature": 0.5,
    "max_tokens": 2000,
    "max_context_length": 8000,
    "top_p": 0.9
  }
}
```

#### Azure OpenAI Configuration

```json
{
  "LLM": {
    "provider": "azureopenai",
    "model": "gpt-4",
    "temperature": 0.7,
    "max_tokens": 2000,
    "max_context_length": 100000,
    "top_p": 0.95,
    "azure_endpoint": "https://your-resource.openai.azure.com",
    "azure_api_version": "2024-02-01",
    "azure_deployment": "your-deployment-name"
  }
}
```

#### Ollama Local Model Configuration

```json
{
  "LLM": {
    "provider": "ollama",
    "model": "llama3.1:8b",
    "temperature": 0.5,
    "max_tokens": 5000,
    "max_context_length": 100000,
    "top_p": 0.7,
    "ollama_host": "http://localhost:11434"
  }
}
```

#### OpenRouter Configuration (200+ Models)

```json
{
  "LLM": {
    "provider": "openrouter",
    "model": "anthropic/claude-3.5-sonnet",
    "temperature": 0.7,
    "max_tokens": 4000,
    "max_context_length": 200000,
    "top_p": 0.95
  }
}
```

### Configuration Examples by Use Case

#### Local Development (stdio)

```json
{
  "mcpServers": {
    "local-tools": {
      "transport_type": "stdio",
      "command": "uvx",
      "args": ["mcp-server-tools"]
    }
  }
}
```

#### Remote Server with Token

```json
{
  "mcpServers": {
    "remote-api": {
      "transport_type": "streamable_http",
      "url": "http://api.example.com:8080/mcp",
      "headers": {
        "Authorization": "Bearer abc123token"
      }
    }
  }
}
```

#### Remote Server with OAuth

```json
{
  "mcpServers": {
    "oauth-server": {
      "transport_type": "streamable_http",
      "auth": {
        "method": "oauth"
      },
      "url": "http://oauth-server.com:8080/mcp"
    }
  }
}
```

---

## 🧪 Testing

### Running Tests

```bash
# Run all tests with verbose output
pytest tests/ -v

# Run specific test file
pytest tests/test_specific_file.py -v

# Run tests with coverage report
pytest tests/ --cov=src --cov-report=term-missing
```

### Test Structure

```
tests/
├── unit/           # Unit tests for individual components
├── omni_agent/     # OmniAgent system tests
├── mcp_client/     # MCPOmni Connect system tests
└── integration/    # Integration tests for both systems
```

### Development Quick Start

1. **Installation**

   ```bash
   # Clone the repository
   git clone https://github.com/omnirexflora-labs/omnicoreagent.git
   cd omnicoreagent

   # Create and activate virtual environment
   uv venv
   source .venv/bin/activate

   # Install dependencies
   uv sync --dev
   ```

2. **Configuration**

   ```bash
   # Set up environment variables
   echo "LLM_API_KEY=your_api_key_here" > .env

   # Configure your servers in servers_config.json
   ```

3. **Start Systems**

   ```bash
   # Try OmniAgent
   python examples/cli/run_omni_agent.py

   # Or try MCPOmni Connect
   python examples/cli/run_mcp.py
   ```

---

## 🔍 Troubleshooting

> **🚨 Most Common Issues**: Check [Quick Fixes](#-quick-fixes-common-issues) below first!

### 🚨 **Quick Fixes (Common Issues)**

| **Error** | **Quick Fix** |
|-----------|---------------|
| `Error: Invalid API key` | Check your `.env` file: `LLM_API_KEY=your_actual_key` |
| `ModuleNotFoundError: omnicoreagent` | Run: `uv add omnicoreagent` or `pip install omnicoreagent` |
| `Connection refused` | Ensure MCP server is running before connecting |

| `Redis connection failed` | Install Redis or use in-memory mode (default) |
| `Tool execution failed` | Check tool permissions and arguments |


### Detailed Issues and Solutions

#### 1. Connection Issues

```bash
Error: Could not connect to MCP server
```

**Solutions:**
- Check if the server is running
- Verify server configuration in `servers_config.json` or `mcp_tools` parameter
- Ensure network connectivity
- Check server logs for errors
- **See [Transport Types & Authentication](#-transport-types--authentication) for detailed setup**

#### 2. API Key Issues

```bash
Error: Invalid API key
```

**Solutions:**
- Verify API key is correctly set in `.env`
- Check if API key has required permissions
- Ensure API key is for correct environment (production/development)
- For Azure OpenAI, verify `azure_endpoint`, `azure_api_version`, and `azure_deployment`
- **See [Configuration Guide](#-configuration-reference) for correct setup**

#### 3. Redis Connection

```bash
Error: Could not connect to Redis
```

**Solutions:**
- Verify Redis server is running: `redis-cli ping`
- Check Redis connection settings in `.env`: `REDIS_URL=redis://localhost:6379/0`
- Ensure Redis password is correct (if configured)
- Use in-memory mode as fallback: `MemoryRouter("in_memory")`

#### 4. Tool Execution Failures

```bash
Error: Tool execution failed
```

**Solutions:**
- Check tool availability on connected servers: `/tools` command
- Verify tool permissions
- Review tool arguments for correctness
- Check tool timeout settings in `agent_config`


#### 6. Import Errors

```bash
ImportError: cannot import name 'OmniAgent'
```

**Solutions:**
- Check package installation: `pip show omnicoreagent`
- Verify Python version compatibility (3.10+)
- Try reinstalling: `pip uninstall omnicoreagent && pip install omnicoreagent`
- Check virtual environment is activated

#### 7. OAuth Server Behavior

**Question**: "Started callback server on http://localhost:3000" - Is This Normal?

**Answer**: **Yes, this is completely normal** when:
- You have `"auth": {"method": "oauth"}` in any server configuration
- The OAuth server handles authentication tokens automatically
- You cannot and should not try to change this address

**If you don't want the OAuth server:**
- Remove `"auth": {"method": "oauth"}` from all server configurations
- Use alternative authentication methods like Bearer tokens

#### 8. Memory Tool Backend Issues

```bash
Error: Memory tool backend not available
```

**Solutions:**
- Verify `memory_tool_backend` is set correctly: `"local"`, `"s3"`, `"db"`, or `None`
- For local backend, ensure write permissions in project directory
- Check that `./memories/` directory can be created

### Debug Mode

Enable debug mode for detailed logging:

```bash
# In MCPOmni Connect CLI
/debug

# In OmniAgent
agent = OmniAgent(..., debug=True)
```

### Getting Help

1. **First**: Check the [Quick Fixes](#-quick-fixes-common-issues) above
2. **Examples**: Study working examples in the `examples/` directory
3. **Issues**: Search [GitHub Issues](https://github.com/omnirexflora-labs/omnicoreagent/issues) for similar problems
4. **New Issue**: [Create a new issue](https://github.com/omnirexflora-labs/omnicoreagent/issues/new) with detailed information

---

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Development Setup

```bash
# Fork and clone the repository
git clone https://github.com/omnirexflora-labs/omnicoreagent.git
cd omnicoreagent

# Set up development environment
uv venv
source .venv/bin/activate
uv sync --dev

# Install pre-commit hooks
pre-commit install
```

### Contribution Areas

- **OmniAgent System**: Custom agents, local tools, background processing
- **MCPOmni Connect**: MCP client features, transport protocols, authentication
- **Shared Infrastructure**: Memory systems, vector databases, event handling
- **Documentation**: Examples, tutorials, API documentation
- **Testing**: Unit tests, integration tests, performance tests

### Pull Request Process

1. Create a feature branch from `main`
2. Make your changes with tests
3. Run the test suite: `pytest tests/ -v`
4. Update documentation as needed
5. Submit a pull request with a clear description

### Code Standards

- Python 3.10+ compatibility
- Type hints for all public APIs
- Comprehensive docstrings
- Unit tests for new functionality
- Follow existing code style

---

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author & Credits

**Created by [Abiola Adeshina](https://github.com/Abiorh001)**

OmniCoreAgent is built by the **OmniCoreAgent Team** - the same team behind powerful AI agent frameworks and event-driven systems.

**🌟 Related Projects:**

- **[OmniCoreAgent](https://github.com/omnirexflora-labs/omnicoreagent)** - Production-ready AI agent framework with built-in MCP client, multi-tier memory, and workflow orchestration (this project)

- **[OmniDaemon](https://github.com/omnirexflora-labs/OmniDaemon)** - Universal event-driven runtime engine for AI agents

> 💡 OmniCoreAgent and OmniDaemon are designed to work seamlessly together, providing a complete AI agent development ecosystem!

**Connect with the creator:**

- **GitHub**: [@Abiorh001](https://github.com/Abiorh001)
- **X (Twitter)**: [@abiorhmangana](https://x.com/abiorhmangana)
- **Website**: [mintify.com](https://mintify.com)
- **Email**: abiolaadedayo1993@gmail.com
- **Documentation**: [omnirexflora-labs.github.io/omnicoreagent](https://omnirexflora-labs.github.io/omnicoreagent)

---

## 🙏 Acknowledgments

OmniCoreAgent is built on the shoulders of giants:

- **[LiteLLM](https://github.com/BerriAI/litellm)** - Unified LLM interface for 100+ models
- **[FastAPI](https://fastapi.tiangolo.com/)** - Modern Python web framework
- **[Redis](https://redis.io/)** - In-memory data store and message broker
- **[Qdrant](https://qdrant.tech/)** - Vector database for semantic search
- **[ChromaDB](https://www.trychroma.com/)** - Embedding database
- **[Opik](https://opik.ai/)** - Production observability and tracing
- **[Pydantic](https://pydantic-docs.helpmanual.io/)** - Data validation
- **[APScheduler](https://apscheduler.readthedocs.io/)** - Advanced Python scheduler

And all the amazing open-source projects that make OmniCoreAgent possible!

---

## 🌟 Why OmniCoreAgent?

### What Sets It Apart

**True Autonomy**: Agents don't just respond—they plan multi-step workflows, use tools to gather information, validate results, and adapt their approach based on outcomes.

**Composable Architecture**: Build small, focused agents and compose them into sophisticated systems. A file system agent, data analysis agent, and reporting agent work together through routing, each handling what it does best.

**Full Control**: Create custom tools, define specialized routing logic, integrate any external service, and extend the framework to match your exact requirements. No black boxes.

**Production-Ready**: Not an experimental framework—built for real applications. Includes proper error handling, retry logic, session management, and observability. Deploy confidently knowing agents handle edge cases gracefully.

**Framework Agnostic**: Works seamlessly with FastAPI for web APIs, event-driven architectures, or any Python application. Build agents that respond to events, serve HTTP requests, or run as background services—same core agent definition.

**Cost Optimized**: Smart context management and model switching reduce LLM costs. Use cheaper models for simple tasks, powerful models for complex reasoning, and maintain only necessary context in memory.

**Clean Developer Experience**: Abstract away LLM orchestration complexity while staying flexible. Define agent behavior, tools, and routing in clean Python code. The framework handles prompt management, tool calling, error handling, and model interactions.

### Perfect For

- **Enterprise AI Applications**: Production-ready agents for business automation
- **Intelligent Automation**: Autonomous agents that handle complex workflows
- **Customer Service Systems**: AI-powered support with tool integration
- **Data Analysis Workflows**: Agents that analyze, process, and report on data
- **Development Assistants**: Code generation, testing, and DevOps automation
- **Multi-Agent Systems**: Complex orchestration with specialized agents
- **Any scenario requiring AI agents that think, decide, and act autonomously**

---


---

<div align="center">

**Created by [Abiola Adeshina](https://github.com/Abiorh001) and the OmniCoreAgent Team**

*Building the future of production-ready AI agent frameworks*

[⭐ Star us on GitHub](https://github.com/omnirexflora-labs/omnicoreagent) | [🐛 Report Bug](https://github.com/omnirexflora-labs/omnicoreagent/issues) | [💡 Request Feature](https://github.com/omnirexflora-labs/omnicoreagent/issues) | [📖 Documentation](https://omnirexflora-labs.github.io/omnicoreagent) | [💬 Discussions](https://github.com/omnirexflora-labs/omnicoreagent/discussions)

</div>
