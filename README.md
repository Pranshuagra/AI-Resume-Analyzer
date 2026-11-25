# 🤖 AI Resume Analyzer – Powered Resume Matching & Skill Gap Analysis

An AI-powered Resume Analyzer that helps job seekers evaluate how well their resumes match specific job descriptions using Natural Language Processing (NLP) and semantic similarity. It analyzes resumes, identifies matching skills, highlights missing keywords, and provides actionable suggestions for improvement.

## 🚀 Project Overview

AI Resume Analyzer is a Flask-based web application designed to make resume screening smarter and more effective.

Instead of relying only on traditional keyword matching, this application uses transformer-based semantic analysis to understand the contextual relationship between resume content and job requirements.

Users can upload their PDF resumes and enter a job description to receive an intelligent resume analysis.

## ✨ Key Features

- 📄 **PDF Resume Upload:** Upload resumes in PDF format.
- 📝 **Job Description Analysis:** Paste job descriptions for comparison.
- 🧠 **AI-Powered Matching:** Uses RoBERTa-based semantic similarity to evaluate resume relevance.
- 📊 **Resume Match Score:** Calculates a semantic similarity score between resume and job description.
- ✅ **Matched Skills:** Identifies skills that align with job requirements.
- ❌ **Missing Skills & Keywords:** Highlights important skills and keywords missing from the resume.
- 💡 **Smart Suggestions:** Provides improvement recommendations to strengthen the resume.
- 🔍 **Skill Gap Analysis:** Helps candidates identify areas where their profiles need improvement.
- 🌐 **Web Interface:** Interactive interface built using Flask, HTML, CSS and Jinja2 templates.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| Backend | Flask |
| Frontend | HTML, CSS, Tailwind CSS |
| Template Engine | Jinja2 |
| NLP | Sentence Transformers |
| Semantic Model | RoBERTa (`stsb-roberta-large`) |
| PDF Processing | PyMuPDF |
| Skill Extraction | Transformers / NER |
| Similarity Analysis | Cosine Similarity |
| Deployment | Render |

## ⚙️ How It Works

The application follows a simple resume analysis workflow:

1. **Upload Resume:** The user uploads a PDF resume.
2. **Extract Text:** PyMuPDF extracts textual information from the uploaded PDF.
3. **Enter Job Description:** The user provides the target job description.
4. **Generate Embeddings:** Sentence Transformers converts resume and job description text into semantic embeddings.
5. **Calculate Similarity:** Semantic similarity is calculated to estimate how closely the resume matches the job requirements.
6. **Identify Skill Gaps:** Skills and keywords are analyzed to identify matching and missing requirements.
7. **Generate Suggestions:** The system provides recommendations to improve resume relevance.

## 📁 Project Structure

```text
AI-Resume-Analyzer/
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── templates/
│   ├── index.html
│   └── result.html
│
├── app.py
├── utils.py
├── requirements.txt
├── runtime.txt
├── README.md
└── .gitignore
```

*Note: The folder structure above is illustrative. Adjust the template and static subfolders according to your actual project.*

## 💻 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/AI-Resume-Analyzer.git
```

### 2. Navigate to Project Directory

```bash
cd AI-Resume-Analyzer
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
python app.py
```

### 6. Open in Browser

```text
http://127.0.0.1:5000/
```

## 📊 Expected Analysis Output

The application provides insights such as:

- Resume Match Percentage
- Matched Skills
- Missing Skills and Keywords
- Skill Gap Analysis
- Resume Improvement Suggestions

## 🌍 Deployment

The application can be deployed using Render.

**Suggested Render Configuration:**

| Configuration | Value |
|---|---|
| Runtime | Python 3 |
| Build Command | `pip install -r requirements.txt` |
| Start Command | `gunicorn app:app` |
| Branch | `main` |

Make sure the Flask application instance is named `app` in `app.py` before using this start command.

## 🎯 Use Cases

- Students preparing for campus placements.
- Freshers searching for their first job.
- Professionals switching careers.
- Job seekers optimizing resumes for specific roles.
- Recruiters looking for intelligent resume screening assistance.

## 🔮 Future Improvements

- ATS-friendly resume scoring.
- Multiple resume comparison.
- Resume recommendations based on job roles.
- Support for additional document formats.
- Enhanced skill extraction and analysis.
- Integration with job portals and recruitment platforms.

## 👨‍💻 Author

**Pranshu Agrahari**

AI/ML & Data Science Enthusiast

GitHub: [Pranshuagra](https://github.com/Pranshuagra)

## ⭐ Support

If you find this project useful, consider giving it a ⭐ on GitHub!

---

**Disclaimer:** The resume match score is an AI-generated estimate and should not be considered a guarantee of ATS selection or job placement.
