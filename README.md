# Search AI Agent

## Overview
A research assistant AI agent built with LangChain that helps generate research papers by gathering information from multiple sources. The agent utilizes Claude 3.5 Sonnet to process queries, search the web, and compile structured research responses.

## Features
- Web search capabilities using DuckDuckGo
- Wikipedia information retrieval
- Structured output with topic summaries and source citations
- Automatic saving of research results to text files
- Powered by Anthropic's Claude 3.5 Sonnet model

## Installation

### Prerequisites
- Python 3.8+
- OpenAI and Anthropic API keys

### Setup
1. Clone the repository:
```bash
git clone https://github.com/salimdev04/search-ai-agent.git
cd search-ai-agent
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the project root with your API keys:
```
OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
```

## Usage
Run the main script and enter your research query when prompted:

```bash
python main.py
```

Example query:
```
What can i help you research? The impact of artificial intelligence on healthcare
```

The agent will:
1. Process your query
2. Search the web for relevant information
3. Retrieve Wikipedia data if needed
4. Generate a structured response with:
   - Topic summary
   - Comprehensive research information
   - List of sources used
   - Tools utilized during research

## Project Structure
- `main.py`: Core application logic and agent configuration
- `tools.py`: Custom tools for web search, Wikipedia queries, and saving results
- `requirements.txt`: Project dependencies

## Dependencies
- langchain - Framework for building AI applications
- langchain-openai & langchain-anthropic - LLM integrations
- wikipedia - Wikipedia API wrapper
- duckduckgo-search - Web search capabilities
- python-dotenv - Environment variable management
- pydantic - Data validation and settings management

## License
MIT

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
