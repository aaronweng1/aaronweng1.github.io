---
layout: null
title: Goals | Aaron Weng
permalink: /goals/
---
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>{{ page.title }}</title>
  <style>
    :root { --ink: #e7f7f5; --muted: #91aaa9; --paper: #080c12; --surface: #101a27; --line: #233640; --accent: #00f0ff; --pink: #ff3cac; --serif: Georgia, "Times New Roman", serif; --sans: "Trebuchet MS", "Segoe UI", sans-serif; }
    * { box-sizing: border-box; } body { margin: 0; color: var(--ink); background: radial-gradient(circle at 80% 10%, #142238 0, transparent 28%), var(--paper); font-family: var(--sans); line-height: 1.6; } a { color: inherit; }
    .header { border-bottom: 1px solid var(--line); background: rgba(8, 12, 18, .9); } .nav, main, footer { width: min(100% - 40px, 980px); margin: auto; } .nav { min-height: 76px; display: flex; align-items: center; justify-content: space-between; } .brand { font-weight: bold; text-decoration: none; } .brand span { color: var(--accent); } .nav-links { display: flex; gap: 20px; align-items: center; } .nav-links a { color: var(--muted); text-decoration: none; font-size: .88rem; } .nav-links a:hover { color: var(--accent); }
    main { padding: 75px 0; } .eyebrow { color: var(--pink); font-size: .78rem; font-weight: bold; letter-spacing: .14em; text-transform: uppercase; } h1 { max-width: 700px; margin: 14px 0 55px; font: bold clamp(3rem, 7vw, 5.5rem)/.95 var(--serif); letter-spacing: -.05em; } .goals { display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; } article { min-height: 240px; padding: 26px; border: 1px solid var(--line); background: var(--surface); } article h2 { margin: 16px 0 12px; font: bold 1.55rem/1.1 var(--serif); } article p { margin: 0; color: var(--muted); } .number { color: var(--accent); font-size: .75rem; font-weight: bold; letter-spacing: .1em; } footer { padding: 25px 0; color: var(--muted); font-size: .8rem; }
    @media (max-width: 700px) { .nav, main, footer { width: min(100% - 28px, 980px); } .nav-links { gap: 10px; } .nav-links a { font-size: .75rem; } .goals { grid-template-columns: 1fr; } }
  </style>
</head>
<body>
  <header class="header"><nav class="nav" aria-label="Main navigation"><a class="brand" href="{{ '/' | relative_url }}">Aaron <span>Weng</span></a><div class="nav-links"><a href="{{ '/' | relative_url }}">Home</a><a href="{{ '/projects/' | relative_url }}">Projects</a><a href="{{ '/goals/' | relative_url }}">Goals</a><a href="{{ '/socials/' | relative_url }}">Socials</a></div></nav></header>
  <main>
    <div class="eyebrow">What I’m working toward</div>
    <h1>Build with purpose. Keep learning.</h1>
    <div class="goals">
      <article><div class="number">01 / GROW</div><h2>Become a stronger engineer</h2><p>Keep improving my foundations in software design, systems, algorithms, and dependable development practices.</p></article>
      <article><div class="number">02 / CREATE</div><h2>Make useful products</h2><p>Build thoughtful tools that turn complicated ideas into clear, accessible experiences for real people.</p></article>
      <article><div class="number">03 / EXPLORE</div><h2>Connect technology and impact</h2><p>Continue exploring machine learning and cybersecurity while staying focused on responsible, practical applications.</p></article>
    </div>
  </main>
  <footer>© 2026 Aaron Weng</footer>
</body>
</html>
