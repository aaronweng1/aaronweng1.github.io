---
layout: null
title: Aaron Weng | Software Developer
---

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Aaron Weng's portfolio: software, machine learning, and systems projects.">
  <title>{{ page.title }}</title>
  <style>
    :root {
      --ink: #17231f;
      --muted: #61716a;
      --paper: #f4f1e9;
      --surface: #fbfaf6;
      --line: #d8ddd4;
      --accent: #d65a32;
      --accent-dark: #9f3e25;
      --green: #315c4c;
      --serif: Georgia, "Times New Roman", serif;
      --sans: "Trebuchet MS", "Segoe UI", sans-serif;
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      color: var(--ink);
      background: var(--paper);
      font-family: var(--sans);
      line-height: 1.6;
    }
    a { color: inherit; }
    .site-header {
      border-bottom: 1px solid var(--line);
      background: rgba(244, 241, 233, .92);
      position: sticky;
      top: 0;
      z-index: 2;
      backdrop-filter: blur(12px);
    }
    .nav, .wrap { width: min(1100px, calc(100% - 40px)); margin: 0 auto; }
    .nav {
      min-height: 72px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 24px;
    }
    .wordmark { font-weight: 700; text-decoration: none; letter-spacing: .02em; }
    .wordmark span { color: var(--accent); }
    .nav-links { display: flex; gap: 25px; font-size: .9rem; }
    .nav-links a { text-decoration: none; color: var(--muted); }
    .nav-links a:hover { color: var(--accent-dark); }
    .hero {
      min-height: 630px;
      display: grid;
      align-items: center;
      padding: 88px 0 105px;
      background:
        radial-gradient(circle at 86% 24%, rgba(214, 90, 50, .16), transparent 24%),
        linear-gradient(135deg, var(--paper) 0%, #e6eee4 100%);
    }
    .hero-grid { display: grid; grid-template-columns: 1.25fr .75fr; gap: 80px; align-items: center; }
    .eyebrow { color: var(--accent-dark); font-size: .76rem; font-weight: 700; letter-spacing: .18em; text-transform: uppercase; }
    h1, h2, h3 { line-height: 1.1; margin: 0; }
    h1 { max-width: 760px; margin-top: 20px; font: 700 clamp(3.5rem, 8vw, 7rem)/.94 var(--serif); letter-spacing: -.055em; }
    .hero-copy { max-width: 570px; margin: 30px 0 0; color: var(--muted); font-size: 1.15rem; }
    .hero-actions { display: flex; flex-wrap: wrap; gap: 14px; margin-top: 35px; }
    .button { display: inline-block; padding: 12px 18px; border: 1px solid var(--ink); text-decoration: none; font-weight: 700; font-size: .9rem; }
    .button-primary { background: var(--ink); color: var(--surface); }
    .button:hover { transform: translateY(-2px); }
    .hero-note { border-top: 1px solid var(--ink); padding-top: 18px; color: var(--muted); font-size: .92rem; }
    .hero-note strong { display: block; color: var(--ink); font: 700 1.4rem var(--serif); margin-bottom: 10px; }
    section { padding: 105px 0; }
    .section-heading { display: flex; justify-content: space-between; gap: 30px; align-items: end; margin-bottom: 42px; }
    h2 { font: 700 clamp(2.4rem, 5vw, 4rem)/1 var(--serif); letter-spacing: -.04em; }
    .section-intro { max-width: 420px; margin: 0; color: var(--muted); }
    .projects { display: grid; grid-template-columns: repeat(2, 1fr); gap: 18px; }
    .project { min-height: 310px; display: flex; flex-direction: column; justify-content: space-between; padding: 28px; border: 1px solid var(--line); background: var(--surface); transition: transform .2s ease, border-color .2s ease; }
    .project:hover { transform: translateY(-5px); border-color: var(--accent); }
    .project-number { color: var(--accent); font-size: .8rem; font-weight: 700; letter-spacing: .1em; }
    .project h3 { margin-top: 18px; font: 700 1.65rem/1.1 var(--serif); }
    .project p { color: var(--muted); }
    .tags { display: flex; flex-wrap: wrap; gap: 7px; margin-top: 22px; }
    .tag { padding: 4px 9px; border: 1px solid var(--line); color: var(--green); font-size: .75rem; }
    .project-link { margin-top: 27px; color: var(--accent-dark); font-size: .88rem; font-weight: 700; text-decoration: none; }
    .about { background: var(--green); color: #f5f3e9; }
    .about .section-intro, .about .eyebrow { color: #c5d7ca; }
    .about-grid { display: grid; grid-template-columns: .9fr 1.1fr; gap: 90px; }
    .about-copy { max-width: 620px; font-size: 1.15rem; }
    .skills { display: grid; grid-template-columns: repeat(2, 1fr); gap: 28px; }
    .skill-group { border-top: 1px solid rgba(245, 243, 233, .35); padding-top: 15px; }
    .skill-group h3 { font-size: .85rem; text-transform: uppercase; letter-spacing: .1em; }
    .skill-group p { color: #c5d7ca; }
    .contact { text-align: center; background: var(--surface); }
    .contact p { max-width: 530px; margin: 20px auto 32px; color: var(--muted); }
    footer { padding: 25px 0; color: var(--muted); font-size: .8rem; }
    @media (max-width: 760px) {
      .nav, .wrap { width: min(100% - 28px, 1100px); }
      .nav { min-height: 64px; }
      .nav-links { gap: 12px; font-size: .78rem; }
      .hero { min-height: auto; padding: 76px 0 86px; }
      .hero-grid, .about-grid { grid-template-columns: 1fr; gap: 48px; }
      .projects { grid-template-columns: 1fr; }
      .section-heading { display: block; }
      .section-intro { margin-top: 18px; }
      section { padding: 75px 0; }
      .skills { gap: 20px; }
    }
  </style>
</head>
<body>
  <header class="site-header">
    <nav class="nav" aria-label="Main navigation">
      <a class="wordmark" href="#top">Aaron <span>Weng</span></a>
      <div class="nav-links">
        <a href="#work">Work</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>
  </header>

  <main id="top">
    <section class="hero">
      <div class="wrap hero-grid">
        <div>
          <div class="eyebrow">Software developer · builder · problem solver</div>
          <h1>Ideas made useful.</h1>
          <p class="hero-copy">I’m Aaron Weng, a developer interested in the space where thoughtful interfaces, intelligent systems, and reliable software meet.</p>
          <div class="hero-actions">
            <a class="button button-primary" href="#work">Explore my work</a>
            <a class="button" href="https://github.com/aaronweng1">View GitHub</a>
          </div>
        </div>
        <div class="hero-note">
          <strong>Selected focus</strong>
          Web applications, machine learning, cybersecurity, and systems programming.
        </div>
      </div>
    </section>

    <section id="work">
      <div class="wrap">
        <div class="section-heading">
          <h2>Selected work</h2>
          <p class="section-intro">A collection of projects built through coursework, research, and competition.</p>
        </div>
        <div class="projects">
          <article class="project">
            <div><div class="project-number">01 / PRODUCT</div><h3>Tiff’s Treats Order Interface</h3><p>A responsive snack-ordering experience with accessibility controls, translation, weather data, OAuth, and PostgreSQL-backed inventory.</p></div>
            <div><div class="tags"><span class="tag">SvelteKit</span><span class="tag">TypeScript</span><span class="tag">PostgreSQL</span></div><a class="project-link" href="https://github.com/csce-315-331-2023c/project-3-903_03">View repository ↗</a></div>
          </article>
          <article class="project">
            <div><div class="project-number">02 / CYBERSECURITY</div><h3>Adaptive Phishing Detection</h3><p>A real-time Discord system combining a bidirectional LSTM spam detector with URL classification and feedback-driven retraining.</p></div>
            <div><div class="tags"><span class="tag">Python</span><span class="tag">Flask</span><span class="tag">RNN / LSTM</span></div><a class="project-link" href="https://github.com/aaronweng1/spambot/tree/1">View repository ↗</a></div>
          </article>
          <article class="project">
            <div><div class="project-number">03 / INFORMATION RETRIEVAL</div><h3>ResumeRanker</h3><p>A recruiter-focused web application using BM25 to rank resumes against job descriptions by contextual relevance and term importance.</p></div>
            <div><div class="tags"><span class="tag">Python</span><span class="tag">BM25</span><span class="tag">Flask</span></div><a class="project-link" href="https://github.com/aaronweng1/weng-CSCE470">View repository ↗</a></div>
          </article>
          <article class="project">
            <div><div class="project-number">04 / MACHINE LEARNING</div><h3>Credit Fraud Detection</h3><p>An evaluation of Logistic Regression, SVM, and XGBoost models on more than 56,000 anonymized credit card transactions.</p></div>
            <div><div class="tags"><span class="tag">Python</span><span class="tag">Scikit-learn</span><span class="tag">XGBoost</span></div><a class="project-link" href="https://github.com/aaronweng1/439-Research">View repository ↗</a></div>
          </article>
          <article class="project">
            <div><div class="project-number">05 / DATA VISUALIZATION</div><h3>Stock Portfolio Trends</h3><p>An interactive web application for tracking portfolio value, visualizing historical performance, and projecting future trends.</p></div>
            <div><div class="tags"><span class="tag">HTML / CSS</span><span class="tag">JavaScript</span><span class="tag">Flask</span></div><a class="project-link" href="https://github.com/aaronweng1/tamuhack22">View repository ↗</a></div>
          </article>
          <article class="project">
            <div><div class="project-number">06 / SYSTEMS</div><h3>Geographic Forwarding Protocol</h3><p>A C implementation of greedy routing that forwards packets through a 2D network based on neighbor distance to the destination.</p></div>
            <div><div class="tags"><span class="tag">C</span><span class="tag">Networking</span><span class="tag">Algorithms</span></div><a class="project-link" href="https://github.com/aaronweng1/geo-routing">View repository ↗</a></div>
          </article>
        </div>
      </div>
    </section>

    <section id="about" class="about">
      <div class="wrap about-grid">
        <div><div class="eyebrow">A little about me</div><h2>Curious by default.</h2></div>
        <div>
          <p class="about-copy">I like turning complex problems into software people can actually use. My projects have taken me from accessible ordering flows and real-time messaging to information retrieval, anomaly detection, and network routing.</p>
          <div class="skills">
            <div class="skill-group"><h3>Build</h3><p>JavaScript, TypeScript, SvelteKit, HTML, CSS, Flask</p></div>
            <div class="skill-group"><h3>Analyze</h3><p>Python, machine learning, BM25, data preprocessing</p></div>
            <div class="skill-group"><h3>Engineer</h3><p>C, PostgreSQL, OAuth, APIs, networking</p></div>
            <div class="skill-group"><h3>Collaborate</h3><p>Research, debugging, testing, and shipping with a team</p></div>
          </div>
        </div>
      </div>
    </section>

    <section id="contact" class="contact">
      <div class="wrap"><div class="eyebrow">Let’s connect</div><h2>Have a problem worth solving?</h2><p>Find my code, experiments, and project history on GitHub.</p><a class="button button-primary" href="https://github.com/aaronweng1">Open GitHub profile ↗</a></div>
    </section>
  </main>
  <footer><div class="wrap">© 2026 Aaron Weng</div></footer>
</body>
</html>