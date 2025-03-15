# Research Assistant Agent

An AI-powered research assistant that automates research, gathers information from multiple sources, and generates structured reports.

## 🚀 Features
- **Automated Research**: Conducts in-depth research on any topic.
- **Web Search Integration**: Retrieves relevant information using DuckDuckGo.
- **Wikipedia Querying**: Extracts detailed knowledge from Wikipedia.
- **Structured Output**: Formats responses into a well-organized structure.
- **Research Output Saving**: Saves research summaries to text files for future reference.

## 🛠 Prerequisites
- Python **3.8+**
- OpenAI API Key

## 📦 Installation

```bash
# Clone the repository
git clone <repository-url>
cd TIM_Agent

# Create and activate virtual environment
python -m venv venv
# Windows
.\venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

## 🔧 Configuration
Create a `.env` file in the project root and add your OpenAI API key:

```ini
OPENAI_API_KEY=your_api_key_here
```

## 📁 Project Structure
```
TIM_Agent/
├── main.py               # Main application file
├── tools.py              # Tool definitions and utilities
├── .env                  # Environment variables
├── .gitignore            # Git ignore file
└── research_output.txt   # Generated research outputs
```

## 🚀 Usage
Run the research assistant:

```bash
python main.py
```

### How It Works
1. The agent prompts you for a research topic.
2. It performs the following tasks:
   - **Web Search**: Fetches relevant information using DuckDuckGo.
   - **Wikipedia Querying**: Retrieves information from Wikipedia.
   - **Structured Response Generation**: Creates a formatted response with:
     - **Topic Summary**
     - **Source Citations**
     - **Tools Used in the Research**
3. Outputs are saved in `research_output.txt`.

## 🛠 Tools Available
- **Web Search**: Uses DuckDuckGo for real-time information retrieval.
- **Wikipedia Query**: Extracts detailed information from Wikipedia.
- **Save Tool**: Stores research outputs with timestamps.

## 📄 Response Structure
```python
class ResearchResponse:
    topic: str        # Research topic
    summary: str      # Generated summary
    sources: list     # List of sources used
    tools_used: list  # Tools used in research
```

## 🤝 Contributing
We welcome contributions! Follow these steps:
1. **Fork** the repository.
2. **Create a feature branch** (`git checkout -b feature-branch`).
3. **Commit your changes** (`git commit -m "Add new feature"`).
4. **Push to your branch** (`git push origin feature-branch`).
5. **Open a Pull Request**.

## 📜 License
[Specify your license here]

---
💡 *Enhance your research process with the AI-powered Research Assistant!*

