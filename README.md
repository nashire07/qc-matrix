# QC Matrix ⭐ — Central Kitchen Skill Tracker

A full-featured QC evaluation and skill tracking app for Central Kitchen teams.

---

## 🚀 Deploy to Vercel (Step-by-Step)

### Step 1 — Upload to GitHub

1. Go to [github.com](https://github.com) and sign in
2. Click the **➕ New** button (top-left) → **New repository**
3. Name it `qc-matrix`, set it to **Private**, click **Create repository**
4. On your computer, open a terminal in this folder and run:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/qc-matrix.git
git push -u origin main
```

> Replace `YOUR_USERNAME` with your actual GitHub username.

---

### Step 2 — Deploy on Vercel

1. Go to [vercel.com](https://vercel.com) and sign in with GitHub
2. Click **Add New → Project**
3. Find and select your `qc-matrix` repository → click **Import**
4. Vercel will auto-detect it's a Vite project — leave all settings as-is
5. Click **Deploy**

That's it! In ~1 minute your app will be live at a URL like:
`https://qc-matrix-yourname.vercel.app`

---

### Step 3 — (Optional) Custom Domain

In Vercel's project dashboard → **Settings → Domains** → add your own domain.

---

## 🛠️ Run Locally

```bash
npm install
npm run dev
```

App runs at `http://localhost:5173`

---

## 🔐 Demo Accounts

| Role | Email | Password |
|------|-------|----------|
| 👑 Junior Lead QC | lead@qc.com | lead123 |
| 🔵 QC Officer | officer1@qc.com | officer123 |

---

## 📁 Project Structure

```
qc-matrix/
├── index.html          # Entry HTML (fonts, meta)
├── vite.config.js      # Vite config
├── vercel.json         # Vercel SPA routing fix
├── package.json
└── src/
    ├── main.jsx        # React root mount
    ├── index.css       # Global CSS variables
    └── App.jsx         # Full app (all components)
```

---

## 🗄️ Backend

Uses **Supabase** (already configured). Tables:
- `users` — login accounts
- `mitras` — field staff
- `categories` — competency categories
- `sub_competencies` — individual skills
- `evaluations` — evaluation sessions
- `evaluation_scores` — per-skill scores

---

## ✨ Features

- 🔐 Role-based login (Lead QC / Officer)
- 👥 Mitra management with evaluation tracking
- 📋 3-step evaluation wizard with scoring
- 📊 Analytics with radar & trend charts
- 🗺️ Team skill heatmap
- ⬇️ CSV export
- 📱 Mobile responsive
