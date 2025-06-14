# AI-Text-Detector
# 🤖 AI Text Detector

This is a web application that analyzes whether a piece of text is **AI-generated** or **human-written** using a combination of deep learning models. The app is built with **Streamlit** and powered by:

- 🧠 **RoBERTa-based classifier** (`roberta-base-openai-detector`) for AI text detection
- 📉 **GPT-2 language model** for perplexity scoring
- ⚙️ **PyTorch** for model inference
- 🎨 Aesthetic and responsive UI with Streamlit custom styling

---

## 🚀 Features

- Detects AI-generated vs human-written text
- Provides:
  - Classifier confidence score
  - GPT-2 perplexity (language naturalness)
  - Combined AI-likelihood score
- Clean, interactive web interface
- Works on CPU and GPU

---

## 📦 Installation

1. **Clone the repo:**

   ```bash
   git clone https://github.com/yourusername/ai-text-detector.git
   cd ai-text-detector
Set up a virtual environment (optional but recommended):

bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
🧪 Run the App Locally
bash
Copy
Edit
streamlit run ai_detector_web.py
Then visit: http://localhost:8501

🛠️ Tech Stack
Python 3.8+

Streamlit

PyTorch

Transformers (Hugging Face)

GPT-2 (gpt2)

RoBERTa (roberta-base-openai-detector)

🧩 How It Works
RoBERTa Classifier:

Returns a confidence score that the input was written by AI.

GPT-2 Perplexity:

Measures how “surprising” the text is to a language model.

Low perplexity = likely AI-generated.

Heuristic Score:

Combines classifier confidence and GPT-2 perplexity to provide a more reliable estimate.


