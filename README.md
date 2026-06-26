# ⚡ Find Your Job — AI Resume Analyzer & Job Finder

> Upload your resume → AI analyzes it → matched jobs appear instantly. Built for Indian job seekers — freshers, experienced, and everyone in between.

![Find Your Job](https://img.shields.io/badge/Find%20Your%20Job-AI%20Powered-00ffff?style=for-the-badge&logo=lightning)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-bf00ff?style=for-the-badge&logo=github)
![No Backend](https://img.shields.io/badge/No%20Backend-Pure%20HTML-00ff88?style=for-the-badge)
![Claude AI](https://img.shields.io/badge/Claude%20AI-Sonnet%204.6-ff0080?style=for-the-badge)

---

## 🚀 Live Demo

👉 **[meghanamandla.github.io/Find-your-job](https://meghanamandla.github.io/Find-your-job)**

---

## ✨ Features

### 📄 Resume Upload & Auto Job Search
| Feature | Description |
|---|---|
| 📄 **PDF / DOCX / TXT Upload** | Drag & drop or click to browse — text extracted instantly |
| 🔍 **Auto Job Search** | Role detected from resume → jobs load immediately on upload |
| 🎯 **ATS Score** | Animated score ring showing ATS compatibility % |
| 🔑 **Keyword Scanner** | Found / missing / partial keywords highlighted |
| 🤖 **AI Analysis** | Claude AI extracts real skills, roles, and gaps |

### 💼 Job Search
| Feature | Description |
|---|---|
| 💼 **Jobs** | Live Adzuna job listings matched to your resume |
| 🎓 **Internships** | Internship search with category chips (Python, ML, Web Dev…) |
| 🎯 **Fresher Jobs** | Entry-level jobs with "fresher" filter on all platforms |
| 🚶 **Walk-in Interviews** | Walk-in listings from Adzuna + direct links to Naukri, Indeed, LinkedIn, Google |
| 🌐 **Remote / WFH** | Remote job search across India |
| 🏛️ **Govt Jobs** | Government sector job search |
| 🔎 **Google Jobs** | Pre-filled Google Jobs banner (aggregates LinkedIn, Naukri, Indeed & more) |
| 💡 **11 Job Boards** | Google Jobs, LinkedIn, Naukri, Indeed, Freshersworld, Internshala, Instahyre, Cutshort, Wellfound, Foundit, Glassdoor |

### 🤖 AI-Powered Tools
| Feature | Description |
|---|---|
| 🔍 **AI Feedback** | Specific, actionable resume improvement tips |
| ✏️ **Resume Rewrite** | Full AI-improved resume with stronger language & ATS keywords |
| 📝 **Cover Letter** | Per-job tailored cover letters generated instantly |
| 🎤 **Interview Prep** | Resume-specific Q&A with STAR-method answers |
| 💰 **Salary Insights** | Market salary ranges for matched roles in India |
| 🗺️ **Career Roadmap** | Personalized step-by-step career plan |
| 🐙 **GitHub Analyzer** | AI review of your GitHub profile & repositories |
| 📝 **Grammar Check** | Writing quality & grammar analysis of your resume |
| 🔗 **LinkedIn Optimizer** | AI-written headline, About section, skill list & tips |

### 📋 Resume Playbook
| Feature | Description |
|---|---|
| ✅ **Live Checklist** | 12-item auto-check against your resume (email, GitHub, LinkedIn, summary, skills, etc.) |
| 📖 **Sections Guide** | 8 must-have resume sections with descriptions |
| ❌ **Mistakes to Avoid** | 6 common resume red flags |
| ⚙️ **Must-Have Skills** | Grid of key skills for software engineering roles |
| 💡 **Project Writing Guide** | 5-question framework + worked example |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | Pure HTML + CSS + Vanilla JS — zero frameworks |
| **3D Background** | Three.js WebGL 2000-particle animated starfield |
| **Physics Effects** | Matter.js — falling text physics on drop zone hover |
| **PDF Parsing** | PDF.js (cdnjs) — text extraction from PDF resumes |
| **DOCX Parsing** | Mammoth.js (unpkg) — Word document text extraction |
| **AI Engine** | Anthropic Claude API (`claude-sonnet-4-6`) |
| **Job Listings** | Adzuna India API — real-time job search |
| **Animations** | CSS transitions + IntersectionObserver scroll reveal |
| **Hosting** | GitHub Pages — single `index.html`, no build step |

---

## 🎯 Job Search Flow

```
Upload Resume
     │
     ▼
quickExtractRole() — scans text for known roles / tech keywords
     │
     ▼
searchJobs() — searches Adzuna India API in parallel (up to 3 roles)
     │
     ▼
Jobs Tab opens automatically with matched listings
     │
     ▼
Google Jobs banner + 11-platform strip appear below results
     │
     ▼
Click "Analyze Resume" for full AI analysis (feedback, rewrite, salary…)
```

---

## 🌐 Supported Job Boards (deep-linked, pre-filled)

| Platform | Type |
|---|---|
| 🔎 Google Jobs | Aggregates all boards |
| 💼 LinkedIn Jobs | Professional network |
| 🚀 Naukri | #1 India portal |
| 🔍 Indeed India | Global board |
| 🌱 Freshersworld | Freshers & entry-level |
| 🎓 Internshala | Internships & jobs |
| ⚡ Instahyre | AI-matched roles |
| ✂️ Cutshort | Curated tech roles |
| 🦄 Wellfound | Startups & VC-backed |
| 📌 Foundit | Ex-Monster India |
| 🪟 Glassdoor | Salary insights |

---

## 📦 Deploy to GitHub Pages

### Step 1 — Fork / Clone
```bash
git clone https://github.com/MeghanaMandla/Find-your-job
cd Find-your-job
```

### Step 2 — Enable GitHub Pages
```
1. Go to your repo → Settings → Pages
2. Source: Deploy from a branch
3. Branch: main / (root)
4. Click Save — live in ~2 minutes
```

### Step 3 — Open
```
https://yourusername.github.io/Find-your-job
```

---

## 🔧 Local Development

No build step — just open in a browser:

```bash
# Option 1 — direct open
open index.html

# Option 2 — local server (avoids CORS on file://)
npx serve .
# or
python3 -m http.server 8080
```

---

## 📁 Project Structure

```
Find-your-job/
├── index.html      # Entire app — single self-contained file
└── README.md       # This file
```

---

## 🎨 Design System

| Element | Detail |
|---|---|
| 🌙 **Default theme** | Dark cyberpunk — neon cyan, purple, pink |
| ☀️ **Light theme** | Clean white mode (toggle in navbar) |
| 🌌 **3D Background** | Three.js WebGL particle starfield |
| 🌊 **Aurora** | Animated radial gradient layers |
| ✨ **Cards** | Glassmorphism with backdrop blur |
| 📱 **Responsive** | Mobile, tablet, desktop |
| 🎬 **Scroll reveal** | Cards fade-in + slide-up on scroll (IntersectionObserver) |
| 🎯 **Drop zone** | Falling text physics (Matter.js) on hover |

---

## 🗂️ Tab Overview

| Tab | What it shows |
|---|---|
| 💡 Skills | ATS score, keyword scanner, role comparison |
| 💼 Jobs | Live job listings + Google Jobs + 11 platform links |
| 🔍 Feedback | AI feedback + Resume Playbook checklist |
| ✏️ Rewrite | AI-improved resume (copy / download) |
| 📝 Cover | Cover letter generator per job |
| 🎤 Interview | Q&A with STAR answers |
| 💰 Salary | Market salary ranges |
| 🗺️ Roadmap | Career plan steps |
| 🐙 GitHub | GitHub profile analyzer |
| 📝 Grammar | Writing quality check |
| 🔗 LinkedIn | LinkedIn profile optimizer |

---

## 👩‍💻 Built By

**Meghana Mandla** — [github.com/MeghanaMandla](https://github.com/MeghanaMandla)

---

## 📄 License

MIT License — free to use, modify, and deploy.

---

<div align="center">
  <p>Built with ⚡ by <a href="https://github.com/MeghanaMandla">Meghana Mandla</a></p>
  <p>
    <a href="https://meghanamandla.github.io/Find-your-job">Live Demo</a> •
    <a href="https://github.com/MeghanaMandla/Find-your-job/issues">Report Bug</a> •
    <a href="https://github.com/MeghanaMandla/Find-your-job/issues">Request Feature</a>
  </p>
</div>
