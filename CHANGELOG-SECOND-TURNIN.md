# Project 2 — Second Turn‑in Fixes

This document tracks every change made to address grader/TA comments for the **Project Two: Add CSS** second submission. Fill one row **per comment** and include the commit hash for easy verification.

## How to use this log
1) Copy each grader comment word‑for‑word into the first column.
2) Describe precisely what you changed in the second column (HTML/CSS + what/where).
3) List all files you touched.
4) After committing, paste the short commit hash.

| Grader Comment | Fix Implemented | Files Touched | Commit |
|---|---|---|---|
| e.g., “Missing reset file on about.html” | Linked `reset.css` in `<head>` for all pages (before `styles.css`) | `index.html`, `about.html`, `contact.html` | |
| e.g., “Nav not centered on contact page” | Converted nav to flexbox; `justify-content: center; gap: 2rem;` | `styles.css` | |
| e.g., “Using px for layout widths” | Switched to fluid `rem/%`; kept max‑width at `60rem` | `styles.css` | |
| e.g., “Different nav markup between pages” | Reused a single `<nav class="site-nav">…</nav>` snippet on all pages | `index.html`, `about.html`, `contact.html` | |
| e.g., “No imported font” | Added Google Fonts `@import` for Inter; kept native fallback stack | `styles.css` | |
| e.g., “CSS indentation not 2 spaces” | Reformatted all CSS: 2‑space indentation; sorted sections | `styles.css`, `reset.css` | |
| e.g., “HTML validation error: stray end tag” | Fixed mismatched `</section>`; validated clean | `about.html` | |
| e.g., “Lacks one fixed‑width page” | Made About page fixed (`.page-fixed { width: 60rem; }`) | `about.html`, `styles.css` | |
| e.g., “No screenshots from live URLs” | Re‑validated via GitHub Pages and captured 6 screenshots | `screenshots/*.png` | |

---

## Shared (same) styles applied on all pages
- Unified typography (font‑family, line‑height, color)
- Centered horizontal navigation with list bullets removed
- Consistent container: `width: 90%`, `max-width: 60rem`, `margin: 0 auto`
- Link and button hover transitions (`transition: all 150ms ease-in-out`)
- Accessible focus styles with `:focus-visible`

## Page‑specific (different) styles
- **Index:** hero block with larger spacing and call‑to‑action
- **About:** fixed‑width layout and image treatment (border‑radius/shadow)
- **Contact:** styled form controls and submit button

## Validation Proof (attach these 6 exact filenames)
- `screenshots/valid-index-html.png`
- `screenshots/valid-index-css.png`
- `screenshots/valid-about-html.png`
- `screenshots/valid-about-css.png`
- `screenshots/valid-contact-html.png`
- `screenshots/valid-contact-css.png`

## Submission Links (paste live URLs)
- **GitHub Repo:** 
- **GitHub Pages (index.html):** 

## Commit Log (paste hashes for quick reference)
- Setup fixes branch + changelog: 
- Link reset + styles on all pages: 
- Nav centering + consistency: 
- Fluid/fixed layouts implemented: 
- Fonts (imported + native): 
- Indentation cleanup (2 spaces): 
- Validation fixes: 
- Add screenshots: 
