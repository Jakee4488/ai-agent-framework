# Educational AI Agent Framework

An advanced educational AI agent framework built using **LangGraph** and **Claude AI**, designed to showcase production-grade context engineering and complex agent architectures. 

This project is structured as a comprehensive 5-part tutorial demonstrating how to build deep-reasoning agents from scratch, featuring ReAct loops, Pydantic-based state management, and asynchronous orchestration.

## Key Features

- **Advanced Agent Architectures**: Implemented robust ReAct (Reason-Act) loops for systematic problem-solving and tool execution.
- **Production-Grade Context Engineering**: Designed sophisticated context management to handle long-horizon tasks efficiently without exceeding token limits.
- **Task Planning**: Integrated structured task tracking and planning using robust TODO lists, enabling agents to monitor progress and prevent task drift.
- **Virtual File Systems**: Engineered a virtual file system stored entirely in the agent state, allowing for intelligent context offloading (`ls`, `read_file`, `write_file`, `edit_file`) and persistent memory across turns.
- **Hierarchical Sub-Agents**: Built complex reasoning capabilities through context isolation, delegating specialized tool sets to focused sub-agents for parallel research and task execution.
- **Tavily-Powered Web Search**: Seamless integration with Tavily for real-time web search, enabling agents to gather, summarize, and synthesize live information.


##  Quickstart

### Prerequisites

- Python 3.11 or later
- [uv](https://docs.astral.sh/uv/) package manager

### Installation

1. Clone the repository and navigate into it:
```bash
git clone https://github.com/your-username/ai-agent-framework.git
cd ai-agent-framework
```

2. Install dependencies (this creates the virtual environment automatically):
```bash
uv sync
```

3. Set up your environment variables:
```bash
cp example.env .env
```
Add your API keys (`ANTHROPIC_API_KEY`, `TAVILY_API_KEY`, etc.) to the `.env` file.

4. Launch the Jupyter Notebooks:
```bash
uv run jupyter notebook
```

## Technology Stack
- **Python 3.11+**
- **LangGraph & LangChain** for asynchronous orchestration and agent loops
- **Claude AI (Anthropic)** as the core LLM engine
- **Pydantic** for rigorous state management and data validation
- **Tavily API** for intelligent web search
