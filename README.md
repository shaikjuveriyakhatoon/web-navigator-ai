# web-navigator-ai
# Web Navigator AI Agent

## 📌 Overview
The **Web Navigator AI Agent** is a local-first assistant that takes plain-language instructions and autonomously browses the web.  
It uses a **locally running LLM** (e.g., Ollama) for planning and **Playwright** for browser automation.  

Example:
```bash
python app.py "search for laptops under 50000 and list top 5"
 output human readable json output
Top 5 laptops under ₹50,000:
1. HP 14s – ₹47,999 – link
2. Lenovo IdeaPad Slim 3 – ₹49,500 – link
...
[
  {"title": "HP 14s", "price": "₹47,999", "url": "https://example.com"},
  {"title": "Lenovo IdeaPad Slim 3", "price": "₹49,500", "url": "https://example.com"}
]
what each  is what to post 
web-navigator-ai-agent/
│─ README.md            # Project overview, install, usage, demo (post this)
│─ LICENSE              # e.g. MIT (post this)
│─ .gitignore           # Python, venv, .env (post this)
│─ requirements.txt     # pip deps (post)
│─ app.py               # starter CLI (post)
│─ agent/               # planning + LLM integration (post)
│   ├─ llm_interface.py # wrapper to call local LLM (post)
│   └─ planner.py       # converts instruction -> step plan (post)
│─ browser/             # Playwright automation code (post)
│   └─ engine.py        # functions to open page, search, extract (post)
│─ outputs/             # example JSON outputs (post)
│─ examples/            # example queries + expected outputs (post)
│─ docs/                # architecture, diagrams, security notes (post)
│─ .github/             # CI workflows, issue templates (post)
│   └─ workflows/ci.yml
│─ CONTRIBUTING.md      # how to contribute (post)
│─ CODE_OF_CONDUCT.md   # optional (post)
