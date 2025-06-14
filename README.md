# Assignment 4: RAG Agent Workflow using LangGraph

This project implements a LangGraph-based multi-agent system with routing, retrieval, LLM interaction, web search, and validation logic. It demonstrates a conditional decision-making workflow using LangChain and LangGraph.

## 📌 Objective

Create a supervised multi-agent workflow with:
- Supervisor routing
- LLM-based response generation
- Retrieval-Augmented Generation (RAG)
- Web crawling (real-time info fetch)
- Output validation loop
- Conditional final output generation

## 🧠 Architecture

![image](https://github.com/user-attachments/assets/7c26ab69-ead9-4042-8a7f-5d65f65bed49)

## 🧩 Components

| Node         | Description |
|--------------|-------------|
| Supervisor   | Classifies the query into USA / web_service / Not Related |
| LLM          | Calls Google Gemini to generate answer |
| RAG          | Uses ChromaDB and HuggingFace embeddings for retrieval |
| web_services | Placeholder for real-time fetch (e.g. from SERPAPI) |
| Validation   | Checks response quality and decides if retry is needed |
| FinalOutput  | Returns answer only if validation passes |

## 🚀 How to Run

1. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2. Set your `.env` file with:
    ```
    GOOGLE_API_KEY=your_google_api_key
    ```

3. Run the notebook `Asssignment_RAG_Agent.ipynb`

---

## 🗂 Submission

All files are ready for GitHub upload. Submit your repository link through the provided Google Form.

