---
layout: null
permalink: /
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Website</title>
  <style>
    :root {
      --bg: #f6f7f4;
      --panel: #ffffff;
      --ink: #1f2933;
      --muted: #52606d;
      --accent: #2f6f6b;
      --accent-soft: #eaf4f3;
      --border: #dfe6e8;
      --shadow: 0 12px 30px rgba(31, 41, 51, 0.08);
    }

    * { box-sizing: border-box; }

    html { scroll-behavior: smooth; }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: var(--bg);
      color: var(--ink);
      line-height: 1.6;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover { text-decoration: underline; }

    .container {
      width: min(1100px, calc(100% - 32px));
      margin: 0 auto;
    }

    header {
      background: #fff;
      border-bottom: 1px solid var(--border);
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      min-height: 72px;
      gap: 20px;
    }

    .brand {
      font-size: 1.2rem;
      font-weight: 700;
      letter-spacing: 0.04em;
    }

    .nav-links {
      display: flex;
      gap: 22px;
      flex-wrap: wrap;
      color: var(--muted);
    }

    .hero {
      padding: 80px 0 48px;
    }

    .hero-inner {
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      align-items: center;
      gap: 40px;
    }

    .eyebrow {
      display: inline-block;
      padding: 8px 12px;
      background: var(--accent-soft);
      color: var(--accent);
      border-radius: 999px;
      font-size: 0.8rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    h1 {
      font-size: clamp(2.4rem, 5vw, 4.2rem);
      line-height: 1.1;
      margin: 18px 0 16px;
    }

    .lead {
      font-size: 1.08rem;
      color: var(--muted);
      max-width: 620px;
      margin-bottom: 28px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 14px;
    }

    .button {
      display: inline-block;
      padding: 14px 22px;
      border-radius: 10px;
      font-weight: 700;
      transition: 0.2s ease;
    }

    .button.primary {
      background: var(--accent);
      color: white;
      box-shadow: var(--shadow);
    }

    .button.secondary {
      background: white;
      color: var(--ink);
      border: 1px solid var(--border);
    }

    .button:hover {
      text-decoration: none;
      transform: translateY(-1px);
    }

    .hero-card {
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 28px;
      box-shadow: var(--shadow);
    }

    .mini-box {
      background: var(--accent-soft);
      border-radius: 14px;
      padding: 18px;
      margin-bottom: 18px;
    }

    .mini-box strong {
      display: block;
      font-size: 1.8rem;
      margin-bottom: 4px;
      color: var(--accent);
    }

    section {
      padding: 56px 0;
    }

    .section-title {
      font-size: clamp(1.8rem, 3vw, 2.5rem);
      margin-bottom: 14px;
    }

    .section-copy {
      color: var(--muted);
      max-width: 640px;
      margin-bottom: 28px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 22px;
    }

    .card {
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 24px;
      box-shadow: var(--shadow);
    }

    .card h3 {
      margin-top: 0;
      font-size: 1.2rem;
    }

    .card p {
      color: var(--muted);
      margin-bottom: 0;
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 26px;
      align-items: center;
    }

    .about-box {
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 30px;
      box-shadow: var(--shadow);
    }

    .list {
      list-style: none;
      padding: 0;
      margin: 18px 0 0;
      color: var(--muted);
    }

    .list li {
      padding: 8px 0;
      border-bottom: 1px solid var(--border);
    }

    .list li:last-child { border-bottom: none; }

    footer {
      background: #1f2933;
      color: #e5e7eb;
      padding: 28px 0;
      text-align: center;
    }

    @media (max-width: 760px) {
      .hero-inner,
      .about-grid,
      .cards {
        grid-template-columns: 1fr;
      }

      .nav {
        flex-direction: column;
        justify-content: center;
        padding: 18px 0;
      }

      .hero {
        padding-top: 52px;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">MY SITE</div>
      <nav class="nav-links" aria-label="Main navigation">
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-inner">
        <div>
          <span class="eyebrow">Simple • Clean • Modern</span>
          <h1>Build something beautiful without overthinking it.</h1>
          <p class="lead">
            A small, stylish website that makes your message clear and helps people connect with you quickly.
          </p>
          <div class="actions">
            <a class="button primary" href="#contact">Get Started</a>
            <a class="button secondary" href="#about">Learn More</a>
          </div>
        </div>

        <div class="hero-card" aria-label="Website preview card">
          <div class="mini-box">
            <strong>1 Page</strong>
            Easy layout, simple content, fast loading.
          </div>
          <div class="mini-box">
            <strong>Mobile</strong>
            Looks good on phones, tablets, and desktops.
          </div>
          <div class="mini-box">
            <strong>Easy</strong>
            Simple to update whenever you want.
          </div>
        </div>
      </div>
    </section>

    <section id="about">
      <div class="container">
        <h2 class="section-title">About</h2>
        <p class="section-copy">
          This is a simple one-page website designed to feel fresh, friendly, and easy to navigate.
        </p>

        <div class="about-grid">
          <div class="about-box">
            <h3>What this site is for</h3>
            <p>
              It can be used for a personal brand, small business, portfolio, or a simple landing page.
            </p>
          </div>

          <div class="about-box">
            <h3>Why it works</h3>
            <ul class="list">
              <li>Clear headline and message</li>
              <li>Simple sections with readable layout</li>
              <li>Clean colors and calm design</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section id="services">
      <div class="container">
        <h2 class="section-title">Services</h2>
        <p class="section-copy">
          Easy, helpful, and focused on the essentials.
        </p>

        <div class="cards">
          <article class="card">
            <h3>Brand Basics</h3>
            <p>Clean structure, clear message, and a website that feels professional from the start.</p>
          </article>

          <article class="card">
            <h3>Simple Design</h3>
            <p>Balanced layout, comfortable spacing, and a design that is easy on the eyes.</p>
          </article>

          <article class="card">
            <h3>Fast Setup</h3>
            <p>Launch your site quickly without a lot of complicated features or unnecessary extras.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <h2 class="section-title">Contact</h2>
        <p class="section-copy">
          Want to build something simple and effective? Reach out and let’s get started.
        </p>
        <div class="actions">
          <a class="button primary" href="mailto:hello@example.com">hello@example.com</a>
          <a class="button secondary" href="tel:+123456789">+1 (234) 567-890</a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">© 2026 My Site. All rights reserved.</div>
  </footer>
</body>
</html>