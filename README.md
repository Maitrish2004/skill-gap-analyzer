 Skill Gap Analyzer

A web-based application that helps students and job seekers evaluate their skills against the requirements of a selected career role.
The system calculates a skill match percentage, identifies missing skills, and provides skill-specific improvement suggestions to help users understand 
what they need to learn next.

---

 Features

-  Career role selection
-  User skill input
-  Automatic skill match percentage
-  Missing skill identification
-  Skill-wise improvement suggestions
-  Readiness status
-  Frontend and backend integration through REST API
-  Simple and responsive user interface

---

 Supported Career Roles

The application currently supports:

- Data Analyst
- Frontend Developer
- Backend Developer
- Mechanical Engineer
- Civil Engineer
- Electrical Engineer
- Electronics Engineer
- Teacher
- Business Analyst

---

 Tech Stack

Frontend

- HTML
- CSS
- JavaScript

Backend

- Python
- Flask
- Flask-CORS

Server

- Gunicorn

Deployment

- Vercel — Frontend
- Render — Backend

---

How It Works

User
  │
  ▼
Select Career Role
  │
  ▼
Enter Existing Skills
  │
  ▼
Frontend (HTML/CSS/JavaScript)
  │
  │  REST API Request
  ▼
Python + Flask Backend
  │
  ▼
Compare User Skills
with Required Role Skills
  │
  ├── Calculate Match Score
  ├── Find Missing Skills
  └── Generate Suggestions
  │
  ▼
Results Displayed
  │
  ├── Skill Score
  ├── Readiness Status
  ├── Missing Skills
  └── Improvement Suggestions

---

Skill Evaluation

The skill score is calculated based on how many required skills the user already has for the selected role.

Score| Status
80% – 100%| Job Ready
50% – 79%| Needs Improvement
Below 50%| Beginner Level

---

 API

Analyze Skills

Endpoint

POST /api/analyze

Request Example

{
  "role": "Data Analyst",
  "skills": ["Python", "SQL", "Excel"]
}

Response includes:

Role
Skill Score
Missing Skills
Status
Improvement Suggestions

---

Project Structure

skill-gap-analyzer/
│
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── Procfile
│
└── frontend/
    ├── index.html
    ├── style.css
    ├── script.js
    └── config.js



Live Demo

Frontend:
https://skill-gap-analyzer-pi.vercel.app

Backend API:
https://skill-gap-analyzer-o55x.onrender.com

---
 Example

Role: Data Analyst

Skills Entered:

Python, SQL, Excel

The system compares these skills with the required skills for a Data Analyst and displays:

- Match Score
- Current Status
- Missing Skills
- Improvement Suggestions

---

 Future Improvements

- Resume upload and automatic skill extraction
- AI-powered skill recommendations
- More career roles
- Personalized learning resources
- User progress tracking
- Database integration
- User authentication
Author
Maitrish Mandal
B.Tech - Computer Science & Engineering

