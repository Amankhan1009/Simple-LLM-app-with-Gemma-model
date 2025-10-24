# 🧠 LangChain + Ollama + Streamlit | Generative AI Demo

This project is a simple **Generative AI web app** built using **LangChain**, **Ollama**, and **Streamlit**.  
It integrates the **Google Gemma (2B) model** locally through Ollama and uses **LangChain prompt templates** to handle user queries.  
The app demonstrates how Large Language Models (LLMs) can be combined with modern frameworks to create intelligent, interactive applications.

---

## 🚀 Features
- 🧩 **LangChain Integration:** Uses `ChatPromptTemplate` and `StrOutputParser` for prompt handling and output parsing.  
- 🤖 **Ollama Model Backend:** Runs the **Gemma 2B model** locally via Ollama for AI text generation.  
- 🌐 **Streamlit Frontend:** Simple, responsive UI for user interaction.  
- 🔐 **Environment Management:** Securely handles API keys and environment variables using `.env`.  
- 🧠 **End-to-End Chain:** Builds a full pipeline — from prompt → model → output → Streamlit display.

---

## 🛠️ Tech Stack
- **Python 3.10+**  
- **LangChain**  
- **Ollama**  
- **Streamlit**  
- **dotenv**  

---

## 📦 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Amankhan1009/langchain-gemma-demo.git
cd langchain-gemma-demo
```
2. Create a Virtual Environment
```
python -m venv venv
source venv/bin/activate   # For Mac/Linux
venv\Scripts\activate      # For Windows
```

3. Install Dependencies
```bash
3. Install Dependencies
```
4. Set Up Environment Variables
Create a file named .env in the project root and add:
```bash
LANGCHAIN_API_KEY=your_langchain_api_key
LANGCHAIN_PROJECT=your_project_name
```

5. Run Ollama

Make sure Ollama is installed and running on your system.
Then pull the Gemma model:
```bash
ollama pull gemma:2b
```
6. Launch the App
```bash
streamlit run app.py
```
**🧩 Project Structure**
```
📦 langchain-gemma-demo
 ┣ 📜 app.py                # Main Streamlit application
 ┣ 📜 .env                  # Environment variables (not to be committed)
 ┣ 📜 requirements.txt      # Project dependencies
 ┗ 📜 README.md             # Project documentation
```

 💡 How It Works

User Input: You enter a question in the Streamlit app.

Prompt Creation: LangChain formats it into a structured prompt.

LLM Processing: Ollama runs the Gemma model locally to generate a response.

Response Display: The result is parsed and displayed neatly in the Streamlit UI.
