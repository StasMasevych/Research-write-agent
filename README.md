# Write Article Agent

A Python-based autonomous agent system that automates research and content drafting using CrewAI. This project demonstrates how multiple specialized agents can collaborate to gather information, summarize findings, and generate well-structured written reports.

## 🚀 Features

- **Agentic Research Pipeline**: Multiple agents (Researcher, Writer, Summarizer) work together to complete research and writing tasks.
- **Automated Web Research**: Agents search the web and extract relevant, credible information.
- **Content Summarization & Drafting**: Converts raw research into summaries and full reports.
- **Modular & Extensible**: Add or modify agents for custom workflows.
- **Environment Configurable**: API keys and settings via `.env` file.

## 🧩 Main Agents

- **Research Agent**: Gathers and synthesizes information from online sources.
- **Write Agent**: Structures and drafts readable content from research.
- **Summarizer Agent**: Condenses large texts into concise summaries.

## 🏗️ How It Works

1. **Setup**: Configure your API keys and environment variables in the `.env` file.
2. **Run the App**: Execute `main.py` to start the agent workflow.
3. **Agent Collaboration**: Agents pass tasks/results to each other until the final output is produced.
4. **Output**: Generates a research summary or report based on your query.

## 📦 Installation

```bash
git clone <repo-url>
cd research-write-agent
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## ⚙️ Usage

1. Set up your `.env` file with required API keys.
2. Run the main script:
   ```bash
   python main.py
   ```
3. Follow prompts or modify `main.py` to customize agent tasks and topics.

## 📝 Example

```
$ python main.py
Enter your research topic: "AI in Renewable Energy"
[ResearchAgent] Searching for latest developments...
[WriteAgent] Drafting summary...
[SummarizerAgent] Finalizing report...
Output saved to: output/ai_renewable_energy_report.txt
```

## 🛠️ Customization

- Add new agents in `utils.py` or separate files.
- Modify agent logic for your needs.
- Integrate with other APIs for more capabilities.

## 📚 Dependencies

- Python 3.8+
- CrewAI (or your agent framework)
- Requests, dotenv, and other packages in `requirements.txt`

## 🤝 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss what you want to change.
