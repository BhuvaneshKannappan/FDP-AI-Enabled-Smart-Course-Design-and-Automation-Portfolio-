# 🎓 SmartCourse AI
### AI-Enabled Smart Course Design and Automation Portfolio

**FDP Capstone Project | Educational Technology | Outcome-Based Education (OBE)**

SmartCourse AI is a web-based teaching-workflow prototype designed to help educators organize course planning, learning activities, assessments, academic records, and course documentation in one place. It supports structured syllabus entry, Bloom’s Taxonomy question-bank preparation, CO–PO mapping, and downloadable reports.

> **Project status:** Local development/capstone prototype. The current application is not a deployed AI model or production-ready student information system. AI-related planning and responsible-use workflows are provided as portfolio modules; review generated or drafted educational content before use.

## 🎯 Objectives

- Simplify course design and academic documentation.
- Support Outcome-Based Education through course outcomes and CO–PO mapping.
- Prepare and export Bloom’s Taxonomy-aligned question papers.
- Organize teaching plans, learning activities, assessments, and records.
- Encourage transparent, ethical use of AI in education.

## ✨ Key Features

- **User accounts:** registration, username/email login, password hashing, session-based logout.
- **Course workspace:** subject details, syllabus, units, outcomes, resources, and announcements.
- **Teaching and learning:** planning, course website content, experiential and interactive activities.
- **Assessment:** question drafts, answer keys, quizzes, Bloom’s Taxonomy question bank.
- **OBE:** CO–PO mapping (CO1–CO5 and common engineering POs).
- **Academic records:** attendance, marks, and CSV export.
- **Research and responsible AI:** paper records, verification fields, and AI-use policy documentation.
- **Reporting:** subject reports and downloads; Bloom question-paper export in DOCX, PDF, and JPG.
- **Interface:** responsive design, profile-area light/dark theme toggle with browser-persisted preference, and animated teacher–student SVG illustration in the updated Flask version.

## 🧩 Project Modules

| Module | Purpose |
|---|---|
| Course / Subject Setup | Enter course information and syllabus |
| Planning | Organize teaching and course delivery |
| Course Website | Prepare course-facing information |
| Experiential Learning | Document activity-based learning |
| Interactive Learning | Prepare interactive learning material and quizzes |
| Assessment | Manage questions and answer keys |
| Records | Track attendance and assessment marks |
| Outcome-Based Education | Document course outcomes |
| Bloom’s Taxonomy | Prepare and export categorized questions |
| CO–PO Mapping | Record outcome alignment |
| Research | Maintain research-paper references |
| Responsible AI | Record AI-use and verification practices |
| Reports | Download course portfolio documentation |

## 🛠️ Technology Stack

| Layer | Technology |
|---|---|
| Backend (primary version) | Python, Flask |
| Database | SQLite, Flask-SQLAlchemy |
| Frontend | HTML, CSS, JavaScript, Jinja templates |
| Authentication | Werkzeug password hashing, Flask sessions |
| Document export | python-docx, ReportLab, Pillow |
| Alternative starter | PHP with SQL schema (separate from Flask login) |

## 📂 Project Structure

```text
SmartCourse/
├── README.md
├── LOGIN_SETUP.txt
├── docs/
│   └── DATABASE_SCHEMA.md
├── flask_app/
│   ├── app.py
│   ├── requirements.txt
│   ├── instance/             # SQLite database directory (created locally)
│   ├── static/               # CSS and illustration assets
│   └── templates/            # Flask/Jinja pages
└── php_version/              # Separate PHP starter and schema
```

## 🚀 Installation and Local Setup (Windows)

**Prerequisites:** Python 3.10 or later and pip.

1. Clone the repository:

   ```powershell
   git clone https://github.com/BhuvaneshKannappan/FDP-AI-Enabled-Smart-Course-Design-and-Automation-Portfolio-.git
   ```

2. Open the folder containing `flask_app`. Depending on how the ZIP was extracted, there may be an additional `SmartCourse` folder. For the local extracted path used during development:

   ```powershell
   cd "E:\FDP\FDP Capstone Project\SmartCourse\SmartCourse\flask_app"
   ```

3. Create and activate a virtual environment (recommended):

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

4. Install dependencies:

   ```powershell
   python -m pip install -r requirements.txt
   ```

5. **Important:** `instance` must be a **directory**, not a file. Some ZIP copies contain an empty file named `instance`. If that is the case, preserve it under another name and create the directory:

   ```powershell
   Rename-Item .\instance instance_backup
   New-Item -ItemType Directory .\instance
   ```

   Run these two commands **only if `instance` is currently a file**. If the directory already exists, skip them.

6. Start the application:

   ```powershell
   python app.py
   ```

7. Visit **http://127.0.0.1:5000** (or the address printed in the terminal). Create an account and sign in.

## 🖼️ Screenshots

Add your own application screenshots to a `screenshots/` folder and link them here:

- Login and registration
- Course dashboard (light theme / dark theme)
- Subject creation and planning
- Bloom’s Taxonomy question bank
- CO–PO mapping
- Reports and downloads

## 🔐 Security and Data Limitations

This is an educational prototype intended for local demonstration. Passwords are hashed and sessions use HTTP-only cookies with SameSite=Lax. However, **sample subjects and course records are shared across registered accounts**; per-user record ownership and authorization are not implemented. Do not upload confidential student records or deploy publicly without adding appropriate permissions, CSRF protection, HTTPS, rate limiting, and other production security measures. Set a strong `SECRET_KEY` environment variable before any deployment. Back up your local `smartcourse.db` before replacing files.

## 🔮 Future Enhancements

- Integrate and evaluate actual AI-assisted course and question-generation services.
- Add role-based access for administrators, teachers, and students.
- Add per-user course ownership and secure student-record permissions.
- Provide learning analytics, dashboard visualizations, and stronger validation.
- Add automated testing, accessibility reviews, and deployment configuration.

## 👨‍💻 Project Information

**Project:** AI-Enabled Smart Course Design and Automation Portfolio  
**Category:** FDP Capstone Project  
**Repository:** [GitHub](https://github.com/BhuvaneshKannappan/FDP-AI-Enabled-Smart-Course-Design-and-Automation-Portfolio-)

---

*SmartCourse AI — Supporting organized, outcome-oriented and responsible digital teaching workflows.*
