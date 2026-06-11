# Research AI Agent

An AI-powered research assistant built with LangChain that can search the web, query Wikipedia, and generate structured research outputs.

## Features

- **Web Search** — Uses DuckDuckGo to find relevant information online
- **Wikipedia Lookup** — Queries Wikipedia for topic summaries
- **Structured Output** — Returns research in a consistent format (topic, summary, sources, tools used)
- **Save to File** — Persists research results to a text file with timestamps

## Setup

1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd research-ai-agent
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. Create a `.env` file from the sample:
   ```bash
   cp sample.env .env
   ```
   Then fill in your API keys.

## Usage

```bash
python main.py
```

You'll be prompted to enter a research topic. The agent will search the web and Wikipedia, then return a structured response with a summary and sources.

## Project Structure

```
├── main.py           # Agent setup and execution
├── tools.py          # Tool definitions (web search, wiki, file save)
├── requirements.txt  # Python dependencies
├── sample.env        # Example environment variables
└── .gitignore
```
