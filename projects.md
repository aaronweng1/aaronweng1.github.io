---
layout: null
title: Projects | Aaron Weng
permalink: /projects/
---
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>{{ page.title }}</title>
  <style>
    :root { --ink: #18231f; --muted: #64716b; --paper: #f4f1e9; --surface: #fbfaf6; --line: #d7ddd5; --accent: #d65a32; --serif: Georgia, "Times New Roman", serif; --sans: "Trebuchet MS", "Segoe UI", sans-serif; }
    * { box-sizing: border-box; } body { margin: 0; color: var(--ink); background: var(--paper); font-family: var(--sans); line-height: 1.6; } a { color: inherit; }
    .header { border-bottom: 1px solid var(--line); } .nav, main, footer { width: min(100% - 40px, 980px); margin: auto; } .nav { min-height: 76px; display: flex; align-items: center; justify-content: space-between; } .brand { font-weight: bold; text-decoration: none; } .brand span { color: var(--accent); } .home-link { text-decoration: none; color: var(--muted); font-size: .9rem; }
    main { padding: 75px 0; } .eyebrow { color: var(--accent); font-size: .78rem; font-weight: bold; letter-spacing: .14em; text-transform: uppercase; } h1 { margin: 14px 0 45px; font: bold clamp(3rem, 7vw, 5.5rem)/.95 var(--serif); letter-spacing: -.05em; } .projects { display: grid; grid-template-columns: repeat(2, 1fr); gap: 18px; } article { min-height: 280px; display: flex; flex-direction: column; justify-content: space-between; padding: 26px; border: 1px solid var(--line); background: var(--surface); } article h2 { margin: 16px 0 12px; font: bold 1.65rem/1.1 var(--serif); } article p { margin: 0; color: var(--muted); } .number { color: var(--accent); font-size: .75rem; font-weight: bold; letter-spacing: .1em; } .project-link { display: block; margin-top: 25px; color: var(--accent); font-size: .88rem; font-weight: bold; text-decoration: none; } footer { padding: 25px 0; color: var(--muted); font-size: .8rem; }
    @media (max-width: 700px) { .nav, main, footer { width: min(100% - 28px, 980px); } .projects { grid-template-columns: 1fr; } }
  </style>
</head>
<body>
  <header class="header"><nav class="nav" aria-label="Main navigation"><a class="brand" href="{{ '/' | relative_url }}">Aaron <span>Weng</span></a><a class="home-link" href="{{ '/' | relative_url }}">Home</a></nav></header>
  <main>
    <div class="eyebrow">Selected work</div>
    <h1>Projects</h1>
    <div class="projects">
      <article><div><div class="number">01 / PRODUCT</div><h2>Tiff’s Treats Order Interface</h2><p>A responsive snack-ordering experience with accessibility controls, translation, weather data, OAuth, and PostgreSQL-backed inventory.</p></div><a class="project-link" href="https://github.com/csce-315-331-2023c/project-3-903_03">View repository ↗</a></article>
      <article><div><div class="number">02 / CYBERSECURITY</div><h2>Adaptive Phishing Detection</h2><p>A real-time Discord system combining a bidirectional LSTM spam detector with URL classification and feedback-driven retraining.</p></div><a class="project-link" href="https://github.com/aaronweng1/spambot/tree/1">View repository ↗</a></article>
      <article><div><div class="number">03 / INFORMATION RETRIEVAL</div><h2>ResumeRanker</h2><p>A web application using BM25 to rank resumes against job descriptions by contextual relevance and term importance.</p></div><a class="project-link" href="https://github.com/aaronweng1/weng-CSCE470">View repository ↗</a></article>
      <article><div><div class="number">04 / MACHINE LEARNING</div><h2>Credit Fraud Detection</h2><p>An evaluation of Logistic Regression, SVM, and XGBoost models on more than 56,000 anonymized transactions.</p></div><a class="project-link" href="https://github.com/aaronweng1/439-Research">View repository ↗</a></article>
      <article><div><div class="number">05 / DATA VISUALIZATION</div><h2>Stock Portfolio Trends</h2><p>An interactive application for tracking portfolio value, visualizing historical performance, and projecting future trends.</p></div><a class="project-link" href="https://github.com/aaronweng1/tamuhack22">View repository ↗</a></article>
      <article><div><div class="number">06 / SYSTEMS</div><h2>Geographic Forwarding Protocol</h2><p>A C implementation of greedy routing through a 2D network based on neighbor distance to the destination.</p></div><a class="project-link" href="https://github.com/aaronweng1/geo-routing">View repository ↗</a></article>
    </div>
  </main>
  <footer>© 2026 Aaron Weng</footer>
</body>
</html>
