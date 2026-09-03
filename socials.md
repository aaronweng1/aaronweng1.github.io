---
layout: null
title: Socials | Aaron Weng
permalink: /socials/
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
    main { padding: 75px 0; } .eyebrow { color: var(--pink); font-size: .78rem; font-weight: bold; letter-spacing: .14em; text-transform: uppercase; } h1 { margin: 14px 0 45px; font: bold clamp(3rem, 7vw, 5.5rem)/.95 var(--serif); letter-spacing: -.05em; } .socials { display: grid; grid-template-columns: repeat(2, 1fr); gap: 18px; max-width: 700px; } .social { padding: 24px; border: 1px solid var(--line); background: var(--surface); text-decoration: none; } .social strong { display: block; color: var(--accent); font-size: 1.2rem; } .social span { color: var(--muted); font-size: .9rem; } .social:hover { border-color: var(--pink); } footer { padding: 25px 0; color: var(--muted); font-size: .8rem; }
    @media (max-width: 700px) { .nav, main, footer { width: min(100% - 28px, 980px); } .nav-links { gap: 10px; } .nav-links a { font-size: .75rem; } .socials { grid-template-columns: 1fr; } }
  </style>
</head>
<body>
  <header class="header"><nav class="nav" aria-label="Main navigation"><a class="brand" href="{{ '/' | relative_url }}">Aaron <span>Weng</span></a><div class="nav-links"><a href="{{ '/' | relative_url }}">Home</a><a href="{{ '/projects/' | relative_url }}">Projects</a><a href="{{ '/goals/' | relative_url }}">Goals</a><a href="{{ '/socials/' | relative_url }}">Socials</a></div></nav></header>
  <main>
    <div class="eyebrow">Find me online</div>
    <h1>Let’s connect.</h1>
    <div class="socials">
      <a class="social" href="https://github.com/aaronweng1"><strong>GitHub ↗</strong><span>My projects and code</span></a>
      <a class="social" href="#"><strong>LinkedIn ↗</strong><span>Add your LinkedIn profile link</span></a>
      <a class="social" href="mailto:your-email@example.com"><strong>Email ↗</strong><span>your-email@example.com</span></a>
      <a class="social" href="#"><strong>Resume ↗</strong><span>Add your resume link</span></a>
    </div>
  </main>
  <footer>© 2026 Aaron Weng</footer>
</body>
</html>
