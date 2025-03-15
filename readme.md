Research Assistant Agent
This project implements an AI-powered research assistant that helps generate research papers and gather information using various tools and language models.

Features
Automated research on any topic
Web search integration using DuckDuckGo
Wikipedia article querying
Research output saving to text files
Structured response formatting
Prerequisites
Python 3.8+
OpenAI API key
Installation
# Clone the repository
git clone <repository-url>
cd TIM_Agent

# Create and activate virtual environment
python -m venv venv
.\venv\Scripts\activate

# Install dependencies
pip install langchain langchain-openai python-dotenv pydantic langchain-community

Configuration
Create a .env file in the project root:
OPENAI_API_KEY=your_api_key_here

Project Structure
TIM_Agent/
├── main.py           # Main application file
├── tools.py          # Tool definitions and utilities
├── .env              # Environment variables
├── .gitignore        # Git ignore file
└── research_output.txt   # Generated research outputs

Usage
Run the research assistant:
python main.py


The agent will prompt you for a research topic and then:

Search the web for relevant information
Query Wikipedia articles
Generate a structured response with:
Topic summary
Source citations
Tools used in the research


Tools Available
Web Search: Uses DuckDuckGo for internet searches
Wikipedia: Queries Wikipedia articles for detailed information
Save Tool: Saves research output to text files with timestamps

Response Structure
class ResearchResponse:
    topic: str        # Research topic
    summary: str      # Generated summary
    sources: list     # List of sources used
    tools_used: list  # Tools used in research


Contributing
Fork the repository
Create a feature branch
Commit your changes
Push to the branch
Create a Pull Request
License
[Add your chosen license here]