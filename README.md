# Snehal Ghodke — Developer Portfolio

A sleek, dark-themed single-page developer portfolio built with pure HTML & CSS. Designed with a terminal/hacker aesthetic that reflects a backend systems engineer's identity — no frameworks, no build tools, just open and run.

---

## 🖥️ Live Preview Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | **Hero** | Full-screen intro with name, role, animated status badge & CTAs |
| 2 | **Terminal Block** | Self-typing JSON profile block with blinking cursor |
| 3 | **Skills** | 4-column grouped skill cards with hover glow effects |
| 4 | **Experience** | 3 internships with bullet points, company tags & date badges |
| 5 | **Projects** | 3 project cards with descriptions and tech stack tags |
| 6 | **Education** | GPA displayed as a large typographic hero number |
| 7 | **Certifications** | 5 certification cards with issuer details |
| 8 | **Contact** | Email, phone, LinkedIn, GitHub — all clickable links |
| 9 | **Footer** | Minimal dark footer with filename-style branding |

---

## 📁 Project Structure

```
snehal-portfolio/
└── snehal-portfolio.html     # Entire portfolio — HTML + CSS + JS in one file
```

Zero dependencies. Zero build step. Single file.

---

## ✨ Features

- **Custom animated cursor** — dot + floating ring follower
- **Animated terminal block** — line-by-line JSON typewriter effect
- **Pulsing availability badge** — "Available for Opportunities" with live dot
- **Scroll-triggered reveals** — IntersectionObserver fade-in with staggered delays
- **Hover interactions** — card lift, green border glow, fill-sweep button transitions
- **Animated scroll indicator** — sliding green line on hero
- **Blinking terminal cursor** — authentic dev aesthetic
- **Responsive grid layouts** — skills, projects, certs auto-wrap on smaller screens
- **Noise texture overlay** — subtle grain for depth and atmosphere
- **Background grid** — dot/line grid with radial mask on hero

---

## 🎨 Design System

### Color Palette

| Variable         | Hex / Value                       | Usage                              |
|------------------|-----------------------------------|------------------------------------|
| `--bg`           | `#080c10`                         | Page background                    |
| `--surface`      | `#0d1117`                         | Card / section backgrounds         |
| `--surface2`     | `#161b22`                         | Terminal bar, secondary surfaces   |
| `--green`        | `#30d4a0`                         | Primary accent — all highlights    |
| `--green-dim`    | `rgba(48, 212, 160, 0.15)`        | Hover backgrounds                  |
| `--blue`         | `#58a6ff`                         | Tech stack tags, hero subtitle     |
| `--orange`       | `#f0883e`                         | Terminal JSON values               |
| `--text`         | `#e6edf3`                         | Primary text                       |
| `--text-muted`   | `#7d8590`                         | Secondary / body text              |
| `--text-dim`     | `#484f58`                         | Timestamps, labels, placeholders   |
| `--border`       | `rgba(48, 212, 160, 0.12)`        | All borders and dividers           |

### Typography

| Font               | Role                            | Weights          |
|--------------------|---------------------------------|------------------|
| **Syne**           | Display headings, section titles | 400, 600, 700, 800 |
| **JetBrains Mono** | Labels, nav, tags, terminal     | 300, 400, 600, 700 |
| **Inter**          | Body copy, descriptions         | 300, 400, 500    |

All fonts loaded via Google Fonts CDN.

---

## 🚀 Getting Started

### Open Locally

No setup required — just open the file:

```bash
# Option 1: Double-click in your file explorer

# Option 2: Serve with Python
python -m http.server 8000
# Visit: http://localhost:8000/snehal-portfolio.html

# Option 3: VS Code — right-click → "Open with Live Server"
```

### Deploy Online

Since it's a single HTML file, deployment is instant on any static host:

```bash
# Netlify — drag & drop the file at netlify.com/drop

# GitHub Pages
git init
git add snehal-portfolio.html
git commit -m "init portfolio"
git push origin main
# Enable Pages in repo Settings → Pages → main branch

# Vercel
npx vercel deploy snehal-portfolio.html
```

---

## ⚙️ Customization Guide

### Update Personal Info
Find and replace the following in the HTML:

| Placeholder | Replace With |
|-------------|--------------|
| `snehalghodake1979@gmail.com` | Your email |
| `+91 7276 996 159` | Your phone number |
| `linkedin.com/in/snehal-ghodke` | Your LinkedIn URL |
| `github.com/snehal-ghodke` | Your GitHub URL |

### Change Accent Color
Edit the `--green` variable in `:root` to any color:
```css
:root {
  --green: #30d4a0;       /* current — terminal green */
  /* --green: #58a6ff;    alternate — electric blue */
  /* --green: #f0883e;    alternate — ember orange */
}
```

### Add / Remove Skills
In the `#skills` section, add or remove `<span class="skill-tag">` elements inside any `.skill-group`.

### Add a New Project
Copy a `.proj-card` block and update the content:
```html
<div class="proj-card reveal">
  <div class="proj-number">project_04.py</div>
  <div class="proj-name">Your Project Name</div>
  <div class="proj-desc">Your project description here.</div>
  <div class="proj-stack">
    <span class="proj-tech">Python</span>
    <span class="proj-tech">FastAPI</span>
  </div>
</div>
```

### Disable Custom Cursor
Remove the `#cur` and `#cur-ring` divs and the cursor JS block at the bottom, and remove `cursor: none` from the `body` style.

---

## 🌐 Browser Support

| Browser      | Support |
|--------------|---------|
| Chrome 90+   | ✅ Full  |
| Firefox 90+  | ✅ Full  |
| Safari 14+   | ✅ Full  |
| Edge 90+     | ✅ Full  |
| IE 11        | ❌ None  |

> Uses `IntersectionObserver`, CSS custom properties, `backdrop-filter`, `mix-blend-mode`, and `clip-path`.

---

## 📦 External Dependencies

| Resource     | URL                        | Used For                        |
|--------------|----------------------------|---------------------------------|
| Google Fonts | `fonts.googleapis.com`     | Syne, JetBrains Mono, Inter     |

No npm packages. No JavaScript libraries. No build tools.

---

## 👤 About

Portfolio for **Snehal Ghodke** — Software Engineer specializing in C++, backend systems, and Linux environments. Currently pursuing B.Tech in Computer Science at Nutan College of Engineering and Research, Pune (GPA: 7.98).

**Contact:** snehalghodake1979@gmail.com | +91 7276 996 159

---

## 📄 License

MIT — free to use, adapt, and share.

---

*Designed with a terminal-meets-modern-tech aesthetic — because great backend engineers deserve a portfolio that looks the part.*
