# 🧬 NexPharmAI

**NexPharmAI** is a multilingual AI-powered medical assistant and drug concept generator built using **Google Gemini AI**. Users can describe symptoms and allergies in their preferred language and receive conceptual medical diagnoses with AI-generated hypothetical drug suggestions in a modern, responsive interface.

> ⚠️ For informational and conceptual use only. Not a substitute for professional medical advice.

---

## 🚀 Features

- 🌍 Multilingual support (20+ languages including English, Hindi, Spanish, German, French)
- 🧠 AI-generated conceptual medical diagnosis
- 💊 Hypothetical drug creation based on diagnosis
- 📄 PDF report download in selected language
- 💻 Responsive and user-friendly Gradio interface

---

## ⚠️ Disclaimer

- Diagnoses and treatments are **AI-generated** and may not be accurate.
- Drug suggestions are **hypothetical** and not tested or approved.
- Always consult a licensed medical professional for health concerns.

---

## 🧰 Tech Stack

| Component      | Technology          |
|----------------|---------------------|
| AI Backend     | Google Gemini AI    |
| Interface      | Gradio              |
| PDF Generator  | FPDF                |
| Environment    | python-dotenv       |

---

## 📁 Project Structure

```
NexPharmAI/
├── app.py
├── requirements.txt
├── .env                 # Optional for API key
├── utils/
│   └── pdf_generator.py
└── README.md
```

---

## 📦 Installation

### Prerequisites

- Python 3.8 or higher
- Google Gemini API Key (Get it from: https://aistudio.google.com/app/apikey)

### Setup Instructions

```bash
git clone https://github.com/yourusername/NexPharmAI.git
cd NexPharmAI
pip install -r requirements.txt
```

### Set Your API Key

Option 1: Directly in `app.py`  
```python
API_KEY = "your-api-key-here"
```

Option 2: Use `.env` file  
Create a `.env` file in the root directory and add:
```
GEMINI_API_KEY=your-api-key-here
```
Then in `app.py`:
```python
from dotenv import load_dotenv
load_dotenv()
API_KEY = os.getenv("GEMINI_API_KEY")
```

---

## ▶️ How to Use

Run the app:

```bash
python app.py
```

Then open in your browser:

```
http://127.0.0.1:7860
```

Steps:
1. Choose language
2. Describe symptoms and allergies
3. Get conceptual diagnosis and drug concept
4. Download PDF report (optional)

---

## ☁️ Run in Google Colab

1. Upload `app.py`
2. Install dependencies:
```python
!pip install gradio google-generativeai fpdf
```
3. Add API key and run the app
4. Access the Gradio-generated public link

---

## 📌 Roadmap

- [ ] Auto symptom suggestions
- [ ] DrugBank/OpenFDA integration
- [ ] ICD-10/11 diagnosis codes
- [ ] Mobile-friendly version
- [ ] Real-time translation API support

---

## 🤝 Contributing

1. Fork the repository
2. Create your branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m "Add feature"`
4. Push the branch: `git push origin feature-name`
5. Open a Pull Request

---

## 📜 License

Licensed under the **MIT License**.  
See the `LICENSE` file for more details.

---

## 🙏 Acknowledgments

- Powered by [Google Gemini AI](https://aistudio.google.com/)
- Interface built using [Gradio](https://gradio.app/)
