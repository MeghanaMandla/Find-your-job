# ⚡ ResumeAI — Cyberpunk Career Intelligence

> AI-powered resume analyzer with job matching, ATS scoring, resume rewriting, cover letter generation, interview prep, and salary insights.

![ResumeAI](https://img.shields.io/badge/ResumeAI-Cyberpunk-00ffff?style=for-the-badge&logo=lightning)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Ready-bf00ff?style=for-the-badge&logo=github)
![No Backend](https://img.shields.io/badge/No%20Backend-Pure%20HTML-00ff88?style=for-the-badge)
![AI Powered](https://img.shields.io/badge/Claude%20AI-Powered-ff0080?style=for-the-badge)

---

## 🚀 Live Demo

👉 **[yourname.github.io/resume-ai](https://yourname.github.io/resume-ai)**

---

## ✨ Features

| Feature | Description |
|---|---|
| 📄 **PDF Upload** | Pure JS PDF parser — no library, no worker, no errors |
| 🤖 **AI Analysis** | Claude AI extracts real skills from your resume |
| 💯 **ATS Score** | Animated score ring showing ATS compatibility |
| 💼 **Job Matching** | 8 real jobs matched to your actual skills |
| 🔑 **Keyword Scanner** | 18 keywords — found / missing / partial |
| 🔍 **AI Feedback** | 8 specific, actionable improvement tips |
| ✏️ **Resume Rewrite** | Full AI-improved resume with stronger language |
| 📝 **Cover Letter** | Per-job tailored cover letters generated instantly |
| 🎤 **Interview Prep** | 8 resume-specific Q&A with STAR-method answers |
| 💰 **Salary Insights** | Market salary ranges for matched roles |
| 🗺️ **Career Roadmap** | 6-step personalized career plan |
| ❤️ **Save Jobs** | Bookmark jobs and filter by Remote / 80%+ match |

---

## 🛠️ Tech Stack

- **Frontend** — Pure HTML + CSS + Vanilla JS (zero frameworks)
- **3D Background** — Three.js WebGL particle system
- **PDF Parsing** — Custom pure-JS PDF byte parser + pako zlib
- **AI Engine** — Anthropic Claude API (`claude-sonnet-4-6`)
- **Hosting** — GitHub Pages (single file, no build step)

---

## 📦 Deploy to GitHub Pages in 3 Steps

### Step 1 — Create Repository
```
1. Go to github.com → New repository
2. Name it: resume-ai
3. Set to Public
4. Click "Create repository"
```

### Step 2 — Upload Files
```
1. Click "uploading an existing file"
2. Drag and drop both files:
   - index.html
   - README.md
3. Click "Commit changes"
```

### Step 3 — Enable GitHub Pages
```
1. Go to Settings → Pages
2. Source: Deploy from a branch
3. Branch: main / (root)
4. Click Save
5. Wait 2 minutes
6. Your site is live at: https://yourname.github.io/resume-ai
```

---

## 🔧 Local Development

No build step needed — just open `index.html` in your browser:

```bash
git clone https://github.com/yourname/resume-ai
cd resume-ai
# Open index.html in Chrome/Firefox
```

Or use a local server:
```bash
npx serve .
# or
python3 -m http.server 8080
```

---

## 📁 Project Structure

```
resume-ai/
├── index.html      # Entire app — single file
└── README.md       # This file
```

---

## 🎨 Design

- 🌙 **Dark cyberpunk** theme with neon cyan, purple, and pink
- 🌌 **WebGL particles** — Three.js 2000-particle animated background  
- 🌊 **Aurora backgrounds** — animated radial gradient layers
- 📱 **Fully responsive** — works on mobile and desktop
- ✨ **Glassmorphism** cards with backdrop blur
- 🔆 **Neon glow** effects on hover

---

## ⚙️ How the PDF Parser Works

This app uses **zero external PDF libraries**. Instead:

1. Reads raw PDF bytes with `FileReader`
2. Loads **pako** (tiny zlib library) to decompress `FlateDecode` streams
3. Scans `BT...ET` text blocks and extracts `(string) Tj` / `[(array)] TJ` operators
4. Decodes PDF escape sequences and hex strings
5. Falls back to ASCII scan for uncompressed PDFs

No PDF.js = No Web Worker = No sandbox errors.

---

## 🤝 Contributing

```bash
git fork https://github.com/yourname/resume-ai
git checkout -b feature/your-feature
# make changes to index.html
git commit -m "feat: your feature"
git push origin feature/your-feature
# open a Pull Request
```

---

## 📄 License

MIT License — free to use, modify, and deploy.

---

<div align="center">
  <p>Built with ⚡ by ResumeAI</p>
  <p>
    <a href="https://yourname.github.io/resume-ai">Live Demo</a> •
    <a href="https://github.com/yourname/resume-ai/issues">Report Bug</a> •
    <a href="https://github.com/yourname/resume-ai/issues">Request Feature</a>
  </p>
</div>
