# 🚀 **RAG-Based Review Helper Bot**

### *A dangerously smooth blend of LLMs, embeddings, vector databases & irresistible prompt engineering.*

Welcome to the **Review Helper Bot** — a project where **Retrieval-Augmented Generation** meets **healthcare reviews**, sprinkled with just enough **Google Gemini magic**, **LangChain wizardry**, and **Chroma vector charm** to make any AI engineer blush with pride.

This repository walks you through building a fully functional RAG pipeline in Google Colab — from setting up your model to deploying a sleek Gradio UI.
All while keeping things **clean, fast, clinical… stunning**

---

## 💡 **What This Project Does**

This project uses:

* **Gemini 2.5 Flash** as the LLM
* **ChromaDB** as the vector database
* **Google Embeddings** to embed review text
* **LangChain** to orchestrate prompts & retrieval
* **Gradio** to wrap it all up in a pretty interactive UI

All together, they create a chatbot that:

✔️ Retrieves real patient reviews
✔️ Uses them to answer questions
✔️ Refuses to hallucinate
✔️ Behaves like a polished professional
✔️ …and still charms you with accuracy

---

## 🔥 **Core Features**

### ✨ Retrieval-Augmented Generation (RAG)

The bot doesn't just "guess."
It **fetches relevant reviews** from a real dataset and answers based on actual text.
Truthful. Contextual. Deliciously reliable.

### 🧠 Custom Prompt Engineering

You sculpt the model's personality with:

* **SystemMessagePromptTemplate**
* **HumanMessagePromptTemplate**
* **ChatPromptTemplate**

Think of it as giving your AI assistant a tailored suit and a fresh haircut.

### 🏥 Healthcare Domain Behavior

The assistant stays loyal:

* Asks healthcare questions = ✔️ Smart, detailed answers
* Asks unrelated things like “How do I change a tire?” = ✔️ Perfectly professional refusal

Your LLM finally knows boundaries. *Sexy, right?*

### 💬 Gradio Chat Interface

A clean, interactive UI to show off your bot to your friends, boss, or that one colleague who insists their model is “better.”

---

## 🧩 **Tech Stack**

| Component        | Purpose                              |
| ---------------- | ------------------------------------ |
| **LangChain**    | Prompt handling + workflow pipelines |
| **Gemini API**   | LLM + embeddings                     |
| **Chroma**       | Vector database                      |
| **Google Colab** | Execution environment                |
| **Gradio**       | Chat interface                       |
| **CSVLoader**    | Ingesting review data                |

---

## ⚙️ **How It Works (The Magic Pipeline)**

1. **Load CSV reviews**
2. **Chunk & embed** using Google Embeddings
3. **Store embeddings** in Chroma
4. **Build a retriever** to pull the most relevant review chunks
5. **Feed them into a ChatPromptTemplate**
6. **Pass prompt → Gemini model**
7. **Parse clean outputs**
8. **Serve responses in Gradio**

It’s like a Michelin-star kitchen…
but instead of cooking food, it cooks **contextual AI responses**.

---

## 🎯 Example Use Case

User: *“Has anyone complained about communication with hospital staff?”*
Bot:

* Searches vector DB
* Extracts related complaints
* Responds based on real text
  No hallucinations. No drama.
  Just cold, hard evidence served with elegance.

---

## 🖥️ **Launching the Gradio App**

Once the full pipeline is set up:

```python
interface = gr.ChatInterface(fn=respond_to_user_question, title="Review Helper Bot")
interface.launch()
```

And boom — your **RAG-powered healthcare review chatbot** is alive and flirting with accuracy.

---

## 🧪 **Why This Project Matters**

* Shows a complete **end-to-end RAG workflow**
* Demonstrates modern **Gemini + LangChain** best practices
* Easy to extend to other domains (legal, HR, finance, etc.)
* Clean enough for production
* Fun enough for a weekend project

---

## ❤️‍🔥 Final Thoughts

This project isn’t just about building a chatbot.
It’s about:

* Mastering RAG
* Understanding vector search
* Engineering prompts like a pro

Think of this repo as the perfect first date between **retrieval systems** and **LLMs** —
one that can actually turn into a long-term relationship.