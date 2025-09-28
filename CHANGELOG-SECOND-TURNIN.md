/* =============================
   Project 2 Second Turn‑in: Required Fixes
   This block intentionally addresses rubric items: centered nav with floats,
   text-decoration removal, list-style removal, margins after reset, fluid/fixed
   layouts, accessible focus, and four floats/positions utilities.
   ============================= */

/* 1) Global base (mobile first); use relative units */
:root {
  font-size: 100%; /* 16px browser default; keep rem math simple */
}
html { box-sizing: border-box; }
*, *::before, *::after { box-sizing: inherit; }

body {
  line-height: 1.6;
  color: #222;
  margin: 1.25rem; /* After reset: ensure text not touching edges */
}

/* 2) Containers: one fluid, one fixed */
.container {
  width: 90%;
  max-width: 60rem; /* ≈960px */
  margin: 0 auto;
}
.page-fixed { /* apply on exactly one page wrapper to satisfy fixed layout */
  width: 60rem; /* fixed ≈960px */
  margin: 0 auto;
}

/* 3) Centered horizontal navigation using FLOATS (per rubric) */
.site-nav { width: 100%; overflow: hidden; }
.site-nav ul {
  list-style: none;
  margin: 0; padding: 0;
  /* center the float row by shrinking UL to its contents and centering it */
  width: -moz-fit-content; /* Firefox legacy */
  width: -webkit-fit-content; /* Safari legacy */
  width: fit-content;
  margin-left: auto; margin-right: auto; /* centers the UL */
}
.site-nav li { float: left; margin: 0 1rem; }
.site-nav a {
  text-decoration: none; /* remove underline per rubric */
  font-weight: 600;
  display: block; /* larger click target */
  padding: 0.5rem 0.25rem;
}

/* clearfix utility for floated nav and any float layouts */
.clearfix::after { content: ""; display: table; clear: both; }

/* 4) Resume lists: remove bullets (per rubric) */
.resume ul, .resume ol { list-style: none; padding-left: 0; }

/* 5) Accessible keyboard focus */
:focus-visible { outline: 2px solid currentColor; outline-offset: 2px; }

/* 6) Four floats/positions utilities to satisfy the requirement */
.float-left { float: left; }
.float-right { float: right; }
.rel { position: relative; }
.abs-top-right { position: absolute; top: 0.5rem; right: 0.5rem; }

/* Example two-column layout using floats (apply on one page section) */
.columns { /* parent wrapper */ }
.columns .col { width: 100%; }
@media screen and (min-width: 40rem) {
  .columns.clearfix .col { width: 48%; }
  .columns.clearfix .col:first-child { margin-right: 4%; }
}

/* 7) Utility spacing scale (optional use across pages) */
:root { --space-1: 0.5rem; --space-2: 1rem; --space-3: 1.5rem; }
.mt-2 { margin-top: var(--space-2); }
.mb-2 { margin-bottom: var(--space-2); }

/* 8) Link hover transition for a touch of polish */
 a, button { transition: all 150ms ease-in-out; }
