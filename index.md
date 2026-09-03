---
layout: null
title: Aaron Weng | Software Developer
---
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Aaron Weng's personal portfolio.">
  <title>{{ page.title }}</title>
  <style>
    :root { --ink: #18231f; --muted: #64716b; --paper: #f4f1e9; --line: #d7ddd5; --accent: #d65a32; --serif: Georgia, "Times New Roman", serif; --sans: "Trebuchet MS", "Segoe UI", sans-serif; }
    * { box-sizing: border-box; }
    body { margin: 0; color: var(--ink); background: var(--paper); font-family: var(--sans); line-height: 1.6; }
    a { color: inherit; }
    .header { border-bottom: 1px solid var(--line); }
    .nav, .main, footer { width: min(100% - 40px, 980px); margin: auto; }
    .nav { min-height: 76px; display: flex; align-items: center; justify-content: space-between; }
    .brand { font-weight: bold; text-decoration: none; }
    .brand span { color: var(--accent); }
    .nav a:last-child { padding: 9px 16px; border: 1px solid var(--ink); text-decoration: none; font-size: .9rem; }
    .intro { min-height: calc(100vh - 77px); display: grid; grid-template-columns: 1fr 300px; align-items: center; gap: 90px; padding: 70px 0; }
    .eyebrow { color: var(--accent); font-size: .78rem; font-weight: bold; letter-spacing: .14em; text-transform: uppercase; }
    h1 { max-width: 620px; margin: 16px 0 24px; font: bold clamp(3.4rem, 8vw, 6.5rem)/.95 var(--serif); letter-spacing: -.05em; }
    .description { max-width: 540px; margin: 0; color: var(--muted); font-size: 1.15rem; }
    .links { display: flex; gap: 20px; margin-top: 30px; font-weight: bold; font-size: .9rem; }
    .links a:first-child { color: var(--accent); }
    .photo-slot { aspect-ratio: 4 / 5; display: grid; place-items: center; border: 1px dashed var(--muted); background: #e7ebe3; color: var(--muted); text-align: center; }
    .photo-slot span { max-width: 150px; }
    footer { padding: 25px 0; color: var(--muted); font-size: .8rem; }
    @media (max-width: 700px) { .nav, .main, footer { width: min(100% - 28px, 980px); } .intro { min-height: auto; grid-template-columns: 1fr; gap: 45px; padding: 75px 0; } .photo-slot { width: min(100%, 250px); } }
  </style>
</head>
<body>
  <header class="header">
    <nav class="nav" aria-label="Main navigation">
      <a class="brand" href="{{ '/' | relative_url }}">Aaron <span>Weng</span></a>
      <a href="{{ '/projects/' | relative_url }}">Projects</a>
    </nav>
  </header>
  <main class="main">
    <section class="intro">
      <div>
        <div class="eyebrow">Hello, I’m Aaron</div>
        <h1>Software developer building useful things.</h1>
        <p class="description">I’m interested in web applications, machine learning, cybersecurity, and systems programming. Welcome to my portfolio.</p>
        <div class="links"><a href="{{ '/projects/' | relative_url }}">See my projects →</a><a href="https://github.com/aaronweng1">GitHub ↗</a></div>
      </div>
      <div class="photo-slot" aria-label="Place a profile photo here"><span>Add your photo here</span></div>
    </section>
  </main>
  <footer>© 2026 Aaron Weng</footer>
</body>
</html>
