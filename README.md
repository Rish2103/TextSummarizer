# AI Text Summarizer Web Application 🚀

A full-stack web application that leverages a fine-tuned Hugging Face `t5-small` transformer model to generate concise, abstractive summaries from conversational text and dialogues. 

## 🛠️ Tech Stack
* **Backend:** FastAPI (Python)
* **Frontend:** Modern HTML5, CSS3 (Inter font), JavaScript Fetch API
* **ML Framework:** PyTorch & Hugging Face Transformers

## 📌 How the Model Weights Work
Because deep learning model weights and training checkpoints (`/results_8k`, `/saved_summary_model_8k`) are too massive to host on GitHub, they have been excluded from this repository using a `.gitignore` file. 

**How to run it:**
1. Clone this repository.
2. Run the FastAPI server using: `uvicorn app:app --reload`
3. The application is built with an automatic cloud fallback. On its first run, if it doesn't detect a local fine-tuned folder, it will automatically pull the standard `t5-small` architecture directly from the Hugging Face Hub to ensure the app spins up and functions perfectly!
