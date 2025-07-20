Sure! Here's your **final, clean, and polished README** written in **plain text** for direct copy-paste (not in markdown code blocks), formatted with spacing and emojis for professional appearance. The live app link is included:
👉 **[https://ai-resume-and-job-matching-assistant.onrender.com/](https://ai-resume-and-job-matching-assistant.onrender.com/)**

---

# 🤖 AI Resume & Job Matching Assistant

An intelligent, AI-powered web app that helps users upload their resumes, analyzes them based on a chosen job role using **Gemini 1.5 Flash**, and provides personalized feedback, skill gap insights, resume score, and a downloadable improved version — all within a simple UI.

🌐 **Live Demo:**
👉 [https://ai-resume-and-job-matching-assistant.onrender.com/](https://ai-resume-and-job-matching-assistant.onrender.com/)

---

## 🚀 Features

* 📄 Upload resume files (`.pdf`, `.docx`, `.txt`)
* 🧠 Gemini AI-powered resume analysis
* 🎯 Select from multiple job roles (e.g., Software Developer, Data Analyst)
* 📊 Resume scoring: Structure, Length, and Keywords
* 🔍 Extracted & missing skills list
* 📝 Line-by-line resume improvement suggestions
* 📥 Downloadable improved `.docx` version
* 🔐 Secure upload handling (5MB max, temp stored)

---

## 💻 Tech Stack

* **Backend**: Python, Flask
* **AI Integration**: Google Gemini 1.5 Flash API
* **PDF Parser**: PyPDF2
* **DOCX Generation**: python-docx
* **Frontend**: HTML (Jinja2 Templates)
* **Deployment**: Render.com

---

## 📁 Project Structure

ai-resume-and-job-matching-assistant/
├── templates/ (index.html, results.html)
├── uploads/
├── app.py
├── requirements.txt
├── .gitignore
└── README.md

---

## ⚙️ How to Run Locally

1. **Clone the Repository**

```
git clone https://github.com/onkars2006/ai-resume-and-job-matching-assistant.git
cd ai-resume-and-job-matching-assistant
```

2. **(Optional) Create a Virtual Environment**

```
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
```

3. **Install Dependencies**

```
pip install -r requirements.txt
```

4. **Set your Google Gemini API key**

On Unix/macOS:

```
export GEMINI_API_KEY="your-api-key"
```

On Windows (PowerShell):

```
$env:GEMINI_API_KEY="your-api-key"
```

5. **Run the App**

```
python app.py
```

Or in production mode:

```
gunicorn app:app
```

Then open: [http://localhost:5000/](http://localhost:5000/)

---

## 🧠 Resume Scoring Logic

| Criteria               | Weight |
| ---------------------- | ------ |
| ✅ Length (1–2 pages)   | 20%    |
| ✅ Structure (Sections) | 30%    |
| ✅ Keyword Match        | 50%    |

AI also gives:

* Extracted skills
* Missing skill gaps
* Suggested job roles
* Readiness scores
* Line-by-line resume improvement suggestions

---

## 📥 Example Output

```
"skills": ["Python", "Flask", "SQL"],
"job_roles": ["Backend Developer", "Software Engineer"],
"skill_gaps": ["CI/CD", "Unit Testing"],
"resume_score": 82,
"line_improvements": {
  "Worked on data": "Designed and optimized data pipelines using SQL and Python"
}
```

---

## 📂 Upload Rules

* ✅ Allowed formats: `.pdf`, `.docx`, `.txt`
* ⛔ Max size: 5MB
* 🗑️ Files are processed temporarily (in `/tmp` on Render)

---

## 🙋‍♂️ Author

**Onkar Somvanshi**
🔗 [LinkedIn](https://www.linkedin.com/in/onkar-somvanshi-b26572331)
💻 [GitHub Profile](https://github.com/onkars2006)

---

## 📄 License

MIT License — Free to use, modify, and distribute.

---

## 🔮 Upcoming Features

* ✅ Export to PDF
* ✅ Email integration for sending resumes
* ✅ User login for saved resume versions
* ✅ More job roles and languages

---
