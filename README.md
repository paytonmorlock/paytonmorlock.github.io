# Payton Morlock — Quarto Portfolio

A professional Quarto website for GitHub Pages.

## 🚀 Prerequisites

Install [Quarto](https://quarto.org/docs/get-started/) and R (or just Quarto standalone — R not required for this site).

## 💻 Local Preview

```bash
quarto preview
```

## 📦 Deploy to GitHub Pages

### Option A — Quarto publish (easiest)

```bash
quarto publish gh-pages
```

This builds your site and pushes it to a `gh-pages` branch automatically.

### Option B — Manual

```bash
quarto render
```

Then push the `_site/` folder contents to the `gh-pages` branch, or configure GitHub Actions.

## 🛠 Customization

- **Your info**: Edit `index.qmd` and `resume.qmd`
- **Photo**: Add `assets/images/portrait.jpg` and uncomment the `<img>` tag in `index.qmd`
- **PDF CV**: Place your CV at `assets/morlock-cv.pdf`
- **Contact form**: Connect to [Formspree](https://formspree.io) — update the `action` attribute on the form
- **Colors/fonts**: All design tokens are in `assets/css/main.css` under `:root`
- **Social links**: Update links in `index.qmd` footer and `resume.qmd` footer

## 📁 Structure

```
payton-quarto/
├── _quarto.yml          # Quarto project config
├── index.qmd            # Home page (Hero, About, Projects, Contact)
├── resume.qmd           # Resume / CV page
└── assets/
    ├── css/main.css     # All styles
    └── js/main.html     # JS injected after body
```
