# 📧 Cold Email Generator with ChromaDB + LLMs

This project leverages **ChromaDB**, **Large Language Models**, and **semantic search** to generate personalized cold emails for outreach, marketing, and lead generation. Just upload your contact/portfolio CSV, and the system crafts tailored messages using context-aware retrieval and prompting.

---

## ✨ Features

- 🧠 **Semantic Matching**: Uses ChromaDB to match user profiles with optimal messaging strategies.
- ✉️ **Personalized Cold Emails**: Automatically generates persuasive cold emails using LLMs (e.g., OpenAI GPT or Claude).
- 📂 **CSV Upload Support**: Ingest a portfolio/contact list and receive email drafts in seconds.
- 🔎 **Retrieval-Augmented Generation**: Fetches relevant background context from vector store before generation.
- 🛠️ **Notebook-Based Interface**: Built in Jupyter Notebooks for experimentation and fast iteration.

---

## 🖼️ Screenshot

[Cold Email Screenshot] ![image](https://github.com/user-attachments/assets/54d77b8a-98af-4285-a4da-ecc474647fa5)

---

## 🧱 Project Structure

```
├── Cold_email_Generator.ipynb    # Main notebook to generate emails
├── Chromadb.ipynb                # Handles vector embedding + indexing
├── my_portfolio.csv              # Sample input data
├── requirements.txt              # Required Python packages
├── screenshots/                  # (Optional) Add demo images here
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/cold-email-generator.git
cd cold-email-generator
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` is not available, manually install:

```bash
pip install openai pandas langchain chromadb tiktoken
```

---

### 3. Run the Notebooks

Open in Jupyter:

```bash
jupyter notebook
```

- Run `Chromadb.ipynb` to load & embed data
- Then run `Cold_email_Generator.ipynb` to generate emails

---

## 📄 Sample Input Format

Your CSV (`my_portfolio.csv`) should include:

| Name       | Company        | Title       | Notes / Context      |
|------------|----------------|-------------|-----------------------|
| John Smith | Acme Corp      | Marketing VP| Interested in AI      |
| Jane Doe   | Future Startups| CTO         | Loves automation tools|

---

## 🔐 Environment Variables

Add your OpenAI or LLM API key:

```bash
export OPENAI_API_KEY=your-key-here
```

Or create a `.env` file with:

```
OPENAI_API_KEY=your-key-here
```

---

## 📬 Example Output

```
Hi John,

I noticed you're leading marketing at Acme Corp and are exploring AI-driven strategies. I'd love to introduce a tool that helps automate lead segmentation...

Best,  
Your Name
```

---
