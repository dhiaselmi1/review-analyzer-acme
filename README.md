# 🛒 Acme Product Review Analyzer

An AI-powered dashboard to extract insights from customer product reviews using open-source language models like **Mistral** (via Ollama). It helps retail teams automate the understanding of thousands of customer reviews by classifying sentiment, identifying key topics, and summarizing feedback — all in a visual and downloadable format.

---

## ✨ Features

- 📁 Upload CSV files containing customer reviews
- 🤖 Automatically:
  - Classify **sentiment** (Positive, Neutral, Negative)
  - Detect **topics** (e.g., "delivery", "quality") — single-word outputs
  - Generate a **one-line summary**
- 📊 Interactive visualizations:
  - Sentiment distribution
  - Top topics across products
- 💾 Download the processed results as a CSV file

---

## 🧱 Tech Stack

| Component     | Technology       |
|---------------|------------------|
| Backend       | FastAPI          |
| Frontend      | Streamlit        |
| LLM Hosting   | Ollama + Mistral |
| Data Handling | Pandas, CSV      |
| Charts        | Streamlit Charts / Altair |

---

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/acme-review-analyzer.git
cd acme-review-analyzer
```
2.  **Create and activate a Python virtual environment**:
    ```bash
    python -m venv venv
    # On macOS/Linux:
    source venv/bin/activate
    # On Windows (PowerShell):
    .\venv\Scripts\Activate.ps1
    # Or Windows (CMD):
    .\venv\Scripts/activate.bat
    ```

  ## ▶️ Running the Application

1.  **Start the FastAPI backend server**:
    ```bash
    uvicorn backend.main:app --reload
    ```

2.  **In a new terminal, start the Streamlit frontend**:
    ```bash
    streamlit run frontend/app.py
    ```
    Open your browser to `http://localhost:8501`.

---
