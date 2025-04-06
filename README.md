# 🤖 CrewAI Kubernetes Blog Agent 🚀

> **Create Local AI Agents at Zero Cost using CrewAI + Ollama + Llama3**  
> No OpenAI keys, no huge bills – just pure open-source AI magic 🪄

---

### 🧠 What This Project Does

This project is an end-to-end tutorial and implementation to **build your own AI Agents** using **CrewAI** and **Llama3**, powered locally by **Ollama**.  
It performs a real-world task:  
📌 **"Research the latest trends in Kubernetes and generate a blog post"**

---

### 📌 Why This Project?

There’s a big myth that AI Agent development is:
- 🧪 Complex
- 💸 Expensive
- 👨‍💻 Only for hardcore developers

We’re here to bust that myth. Thanks to open-source tools like **CrewAI**, **Ollama**, and **LangChain-style agents**, you can build powerful multi-agent setups on your own laptop – for free!

---

### 🔍 Features

- ✅ Local LLM setup with **Ollama**
- ✅ Use of **Llama3 1B** model (totally free & local)
- ✅ Built with **CrewAI** multi-agent orchestration
- ✅ No cloud API usage or token limit
- ✅ Zero-to-hero guide with clear steps
- ✅ Clean Python project structure
- ✅ Final output in Markdown (`report.md`)

---

### 🚧 What You’ll Learn

- 🤖 AI Agents vs AI Assistants  
- 📦 Installing & setting up **CrewAI**  
- 🐍 Python virtual environment & dependency management  
- ⚙️ Ollama setup & local LLM configuration  
- 🔁 Agent collaboration using **CrewAI**  
- 🧩 Multi-agent configuration using YAML  
- 📝 Final blog generation on **Kubernetes trends**

---

### ⚙️ Setup & Installation

```bash
# Step 1: Create virtual environment
python -m venv crew
source crew/bin/activate  # use crew\Scripts\activate for Windows

# Step 2: Install CrewAI
pip install crewai

# Step 3: Create new project
crewai create crew devops-ai-project
cd devops_ai_project/

# Step 4: Setup Ollama (run in another terminal)
ollama list
ollama run llama3.2:1b

# Step 5: Configure the LLM in .env
echo "MODEL_NAME=llama3.2:1b" > .env

# Step 6: Install agent dependencies
crewai install

# Step 7: Run the agents
crewai run
