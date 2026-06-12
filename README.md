# ⚡ ResumeAI – AI Resume Screener & Keyword Matcher

> **Live Demo:** [Deployed on Netlify](https://resumeai-screener.netlify.app) | **GitHub:** [resume-screener](https://github.com/shanukhandala4-cell/resume-screener)

A lightweight, production-ready NLP web application that analyzes how well a resume matches a job description. Fully client-side — no server required, no data ever leaves your browser.

---

## ✨ Features

- **📄 PDF Text Extraction** — Parses uploaded PDF resumes using PDF.js directly in the browser
- **🎯 ATS Match Score** — Uses TF-IDF vectorization and cosine similarity to calculate a compatibility percentage
- **🔑 Keyword Gap Analysis** — Identifies important keywords in the JD missing from the resume, ranked by importance
- **✅ Matched Keywords** — Shows what you're already doing right
- **💡 Improvement Tips** — Actionable advice to boost your ATS score
- **🌙 Dark/Light Theme** — System-aware theming with manual override
- **🔒 100% Private** — No data sent to servers; everything runs in your browser

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **Vanilla HTML/CSS/JS** | Frontend & UI |
| **PDF.js** | Client-side PDF text extraction |
| **TF-IDF (custom JS)** | Text vectorization |
| **Cosine Similarity** | Similarity scoring |
| **Netlify** | Static site deployment |
| **Streamlit** | Python-based alternative UI |
| **PyPDF2 + scikit-learn** | Python PDF parsing + ML vectorization |

---

## 🚀 Running Locally

### Web Version (Recommended)
```bash
open index.html
```

### Streamlit Version
```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## 📂 Project Structure

```
resume-screener/
├── index.html          # Main web app
├── styles.css          # Premium glassmorphic UI
├── app.js              # TF-IDF + Cosine Similarity in JS
├── app.py              # Streamlit Python version
├── requirements.txt    # Python dependencies
└── README.md           # Documentation
```

---

## 🧠 How It Works

1. **Text Extraction** — PDF.js reads the uploaded PDF entirely in your browser
2. **TF-IDF Vectorization** — Both texts converted into numerical TF-IDF vectors
3. **Cosine Similarity** — The angle between vectors gives the match percentage

$$\text{similarity} = \frac{\vec{A} \cdot \vec{B}}{|\vec{A}||\vec{B}|}$$

---

*Built with ❤️ using vanilla JS, TF-IDF, and Cosine Similarity*
