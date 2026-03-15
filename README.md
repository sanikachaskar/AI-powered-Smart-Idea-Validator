# 🔍 IdeaLens — AI-Powered Startup Idea Validator

> Drop your startup idea. Get an AI-powered verdict in seconds.

![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Claude AI](https://img.shields.io/badge/Claude_AI-Anthropic-orange?style=flat)
![License](https://img.shields.io/badge/license-MIT-green?style=flat)

---

## 🚀 Live Demo

> Open `index.html` in any browser — no server, no build step, no install.

---

## ✨ What It Does

**IdeaLens** analyzes your startup idea using Claude AI (Anthropic) and returns:

- ✅ **Overall viability score** — 1 to 100
- 📊 **5 detailed metrics** — Market size, Problem clarity, Competitive edge, Revenue potential, Execution difficulty
- 💪 **Strengths** — What's working in your favor
- ⚠️ **Risks** — What could go wrong
- 💡 **Opportunities** — What you might be missing
- 🎯 **Recommendation** — Actionable next steps from an AI VC advisor
- 🔗 **Share results** — Copy a formatted report to your clipboard

---

## 📸 Screenshots

| Auth | Analyzer | Dashboard |
|------|----------|-----------|
| Sign up / Sign in | Paste idea → get full AI report | All past analyses saved |

---

## 🗂️ Project Structure
```
idealens/
├── index.html          # App shell + auth screen
├── css/
│   └── style.css       # Clean minimal design system
└── js/
    ├── auth.js         # Login, register, session (localStorage)
    ├── app.js          # Navigation, toast, share modal
    ├── analyze.js      # Claude API call + result rendering
    └── dashboard.js    # Saved ideas grid + detail view
```

---

## ⚙️ Setup & Usage

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/idealens.git
cd idealens
```

### 2. Add your Anthropic API key

Open `js/analyze.js` and update the fetch call:
```js
headers: {
  'Content-Type': 'application/json',
  'x-api-key': 'YOUR_ANTHROPIC_API_KEY',
  'anthropic-version': '2023-06-01',
  'anthropic-dangerous-direct-browser-access': 'true'
}
```

Get your free API key at 👉 [console.anthropic.com](https://console.anthropic.com)

### 3. Open in browser
```bash
open index.html
# or just double-click the file
```

No npm. No build. No server. Just open and go.

---

## 🌐 Deploy on GitHub Pages (Free Hosting)

1. Push your code to GitHub
2. Go to **Settings → Pages**
3. Set source to **main branch → / (root)**
4. Your app is live at:
   `https://YOUR_USERNAME.github.io/idealens`

---

## 🛠️ Tech Stack

| Layer | Tech |
|-------|------|
| Structure | HTML5 |
| Styling | CSS3 (custom design system, CSS variables) |
| Logic | Vanilla JavaScript (ES6+) |
| AI Engine | Claude Sonnet — Anthropic API |
| Storage | localStorage (no backend needed) |
| Fonts | DM Sans + DM Serif Display (Google Fonts) |

---

## 🔐 Auth & Data

- User accounts are stored in `localStorage` — no backend or database required
- Sessions persist across page refreshes
- All idea analyses are saved per user account
- Supports up to 50 saved analyses per user

---

## 🤝 Contributing

Pull requests are welcome! Here are some ideas to extend the project:

- [ ] Export report as PDF
- [ ] Compare two ideas side by side
- [ ] Add charts/graphs for metric visualization
- [ ] Dark mode toggle
- [ ] Firebase backend for real user accounts


