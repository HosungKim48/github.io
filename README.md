# Hosung Kim — Data Science Portfolio

**Live site:** [https://hosungkim.github.io  ](https://hosungkim48.github.io/)

**Purpose:** A recruiter-friendly, visually bold portfolio that links to deep-dive project repos.

This site is a minimalist static page (no framework build needed) styled with Tailwind via CDN.  
It highlights projects with concise business + technical summaries and links out to full repositories.

---

## 🌐 What’s here

- **Landing page** with hero, projects, about, and contact sections
- **Startup-style** design using Tailwind (CDN) for quick iteration
- **Fast updates**: edit a single `index.html` file and push

**Primary project featured:**
- [Demand Prediction (PCA + Perceptron)](https://github.com/HosungKim/demand-prediction) — Forecasts demand to support algorithmic pricing with PCA + Keras.

---

## 🗂 Repo structure

```
hosungkim.github.io/
├─ index.html         # main single-page site (Tailwind via CDN)
├─ /assets            # (optional) images, logos, PDFs
└─ README.md          # this file
```

> Note: Since we use Tailwind via CDN, there’s **no build step**. GH Pages serves `index.html` directly.

---

## 🚀 Update / Publish

1. Edit `index.html` (e.g., add a project card in the “Projects” section).
2. Commit and push to `main`.
3. GitHub Pages auto-deploys from the root (`Settings → Pages → Source: Deploy from a branch → main`).

If you just created the repo, the site may take ~1–2 minutes to appear.

---

## ➕ Add a new project

In `index.html`, duplicate the **Project Card** block and customize:

```html
<a href="https://github.com/HosungKim/REPO_NAME" target="_blank"
   class="group block rounded-3xl border border-neutral-800 glass p-6 hover:border-violet-600 transition">
  <div class="text-sm text-neutral-400">Category · Tags</div>
  <div class="mt-2 text-xl font-bold group-hover:text-violet-300">Project Title</div>
  <p class="mt-2 text-neutral-300">
    One-sentence business + technical summary.
  </p>
  <ul class="mt-4 flex flex-wrap gap-2 text-xs text-neutral-300">
    <li class="px-2 py-1 rounded-full bg-neutral-800/60">Python</li>
    <li class="px-2 py-1 rounded-full bg-neutral-800/60">TensorFlow</li>
    <li class="px-2 py-1 rounded-full bg-neutral-800/60">Forecasting</li>
  </ul>
  <div class="mt-5 text-sm text-violet-300 underline underline-offset-4">Open repo</div>
</a>
```

Recommended content pattern for each project:
- **What it does** (problem → outcome)
- **How it works** (methods/tools)
- **Why it matters** (business impact)

---

## 🧰 Tech stack

- **Static site:** plain HTML
- **Styling:** TailwindCSS via CDN (no Node/Vite)
- **Icons/emoji:** native (no dependency)
- **Optional:** Add images to `/assets` and reference them in `index.html`

If you ever migrate to React/Vite, make sure to add a **404 fallback** (or use hash routing) for GitHub Pages.

---

## 🧪 Local preview (optional)

Any static server works. For a quick check:

```bash
# Python 3
python -m http.server 8080
# then open http://localhost:8080 in your browser
```

---

## 🧭 Content checklist

- [ ] Hero section updated (headline + subhead reflect current focus)
- [ ] At least one featured project card with a repo link
- [ ] About section (skills/interest areas) is current
- [ ] Contact info: email + LinkedIn correct
- [ ] Footer year updates automatically (JS in `index.html`)

---

## 📬 Contact

**Hosung Kim**  
- Email: [hosungkim48@gmail.com](mailto:hosungkim48@gmail.com)  
- LinkedIn: [hosun9k](https://linkedin.com/in/hosun9k)  
- GitHub: [@HosungKim](https://github.com/HosungKim)
