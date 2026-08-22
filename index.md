---
layout: null
permalink: /
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gaikovina Amini | Accounting & Finance Portfolio</title>
  <style>
    :root {
      --bg: #f8f3ea;
      --panel: #ffffff;
      --ink: #241f1b;
      --muted: #66594d;
      --accent: #9f4f28;
      --accent-dark: #56331f;
      --accent-soft: #f5e5d6;
      --border: #ead9c8;
      --shadow: 0 12px 30px rgba(31, 41, 51, 0.08);
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background:
        radial-gradient(circle at 10% 10%, rgba(159, 79, 40, 0.12), transparent 26%),
        radial-gradient(circle at 90% 20%, rgba(86, 51, 31, 0.10), transparent 24%),
        linear-gradient(135deg, #f8f0e3 0%, #f3e1cd 48%, #f9f4eb 100%);
      color: var(--ink);
      line-height: 1.6;
      overflow-x: hidden;
    }

    a { color: var(--accent); text-decoration: none; }
    a:hover { text-decoration: underline; }

    .container {
      width: min(1120px, calc(100% - 32px));
      margin: 0 auto;
    }

    header {
      background: rgba(255, 255, 255, 0.94);
      border-bottom: 1px solid var(--border);
      position: sticky;
      top: 0;
      z-index: 10;
      backdrop-filter: blur(10px);
    }

    main, footer {
      position: relative;
      z-index: 1;
    }

    .sticker-layer {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 0;
      overflow: hidden;
    }

    .sticker {
      position: absolute;
      width: clamp(86px, 12vw, 170px);
      aspect-ratio: 1;
      object-fit: cover;
      border-radius: 22px;
      border: 6px solid rgba(255, 255, 255, 0.74);
      box-shadow: 0 18px 36px rgba(86, 51, 31, 0.16);
      opacity: 0.18;
      filter: saturate(1.08) contrast(0.98);
    }

    .profile-sticker {
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%) rotate(-3deg);
      width: clamp(180px, 22vw, 260px);
      border-radius: 50%;
      box-shadow: 0 12px 36px rgba(60, 32, 12, 0.24), 0 2px 8px rgba(0,0,0,0.1);
      border: 6px solid #fff;
      opacity: 1;
      filter: none;
      background: #fff;
      z-index: 2;
    }

    .sticker.one { top: 110px; left: 22px; transform: rotate(-10deg); }
    .sticker.two { top: 230px; right: 30px; transform: rotate(9deg); }
    .sticker.three { top: 760px; left: 5%; transform: rotate(8deg); }
    .sticker.four { top: 1180px; right: 6%; transform: rotate(-8deg); }
    .sticker.five { bottom: 130px; left: 26px; transform: rotate(12deg); }
    .sticker.six { bottom: 260px; right: 38px; transform: rotate(-12deg); }
    .sticker.seven { top: 430px; left: 34px; transform: rotate(7deg); }
    .sticker.eight { top: 560px; right: 44px; transform: rotate(-7deg); }

    .nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      min-height: 72px;
      gap: 20px;
    }

    .brand {
      font-size: 1.05rem;
      font-weight: 800;
      letter-spacing: 0.08em;
      color: var(--accent-dark);
    }

    .nav-links {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
      font-size: 0.95rem;
    }

    .hero {
      padding: 98px 0 66px;
      background: linear-gradient(90deg, rgba(255, 250, 243, 0.9), rgba(255, 250, 243, 0.58));
      border-bottom: 1px solid rgba(255, 255, 255, 0.55);
    }

    .hero-inner {
      display: grid;
      grid-template-columns: 1.15fr 0.85fr;
      align-items: center;
      gap: 40px;
    }

    .eyebrow {
      display: inline-block;
      padding: 8px 12px;
      background: var(--accent-soft);
      color: var(--accent);
      border-radius: 999px;
      font-size: 0.78rem;
      font-weight: 800;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    h1 {
      font-size: clamp(2.5rem, 5vw, 4.4rem);
      line-height: 1.05;
      margin: 18px 0 16px;
    }

    h2.section-title {
      font-size: clamp(1.75rem, 3vw, 2.45rem);
      margin: 0 0 12px;
    }

    h3 { margin-top: 0; }

    .lead {
      font-size: 1.08rem;
      color: var(--muted);
      max-width: 700px;
      margin-bottom: 26px;
    }

    .actions { display: flex; flex-wrap: wrap; gap: 14px; }

    .button {
      display: inline-block;
      padding: 13px 20px;
      border-radius: 10px;
      font-weight: 800;
      transition: 0.2s ease;
    }

    .button.primary { background: var(--accent); color: white; box-shadow: var(--shadow); }
    .button.secondary { background: white; color: var(--ink); border: 1px solid var(--border); }
    .button:hover { text-decoration: none; transform: translateY(-1px); }

    .profile-card, .card, .about-box {
      background: rgba(255, 255, 255, 0.92);
      border: 1px solid rgba(223, 230, 232, 0.9);
      border-radius: 20px;
      box-shadow: var(--shadow);
      backdrop-filter: blur(6px);
    }

    .profile-card { padding: 28px; }

    .profile-photo {
      width: 100%;
      max-height: 320px;
      object-fit: cover;
      object-position: center;
      border-radius: 18px;
      margin-bottom: 20px;
      box-shadow: var(--shadow);
      display: block;
    }

    .quick-list { list-style: none; padding: 0; margin: 0; }
    .quick-list li { padding: 10px 0; border-bottom: 1px solid var(--border); }
    .quick-list li:last-child { border-bottom: none; }
    .quick-list strong { color: var(--ink); }

    section { padding: 54px 0; }

    .culture-section {
      position: relative;
      background: linear-gradient(135deg, rgba(86, 51, 31, 0.92), rgba(159, 79, 40, 0.84));
      color: #fff;
    }

    .culture-section.alt {
      background: linear-gradient(135deg, rgba(122, 59, 32, 0.9), rgba(61, 77, 55, 0.86));
    }

    .culture-section .section-copy,
    .culture-section .card p,
    .culture-section .about-box p,
    .culture-section .list,
    .culture-section .timeline-item p { color: rgba(255, 255, 255, 0.86); }

    .culture-section .card,
    .culture-section .about-box {
      background: rgba(255, 255, 255, 0.12);
      border-color: rgba(255, 255, 255, 0.24);
    }

    .culture-section .tag {
      background: rgba(255, 255, 255, 0.16);
      color: #fff;
    }

    .section-copy {
      color: var(--muted);
      max-width: 760px;
      margin: 0 0 28px;
    }

    .grid-2 { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 22px; }
    .grid-3 { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 22px; }

    .culture-mosaic {
      padding: 34px 0 20px;
      background: linear-gradient(180deg, rgba(248, 243, 234, 0.9), rgba(248, 243, 234, 0.98));
    }

    .mosaic-grid {
      display: grid;
      grid-template-columns: 1fr 1.15fr 1fr;
      gap: 18px;
      align-items: center;
    }

    .mosaic-card {
      position: relative;
      min-height: 190px;
      border-radius: 24px;
      overflow: hidden;
      box-shadow: var(--shadow);
      border: 8px solid rgba(255, 255, 255, 0.78);
      background: var(--accent-soft);
    }

    .mosaic-card img {
      width: 100%;
      height: 100%;
      min-height: 190px;
      object-fit: cover;
      display: block;
    }

    .mosaic-card:nth-child(2) {
      min-height: 250px;
      transform: translateY(-12px);
    }

    .mosaic-card::after {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(180deg, transparent 45%, rgba(86, 51, 31, 0.28));
      pointer-events: none;
    }

    .mosaic-note {
      text-align: center;
      color: var(--muted);
      max-width: 720px;
      margin: 14px auto 0;
      font-weight: 700;
    }

    .card, .about-box { padding: 24px; }
    .card p, .about-box p { color: var(--muted); margin-bottom: 0; }

    .tag-list { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 14px; }
    .tag {
      background: var(--accent-soft);
      color: var(--accent-dark);
      padding: 8px 11px;
      border-radius: 999px;
      font-size: 0.9rem;
      font-weight: 700;
    }

    .timeline { display: grid; gap: 18px; }
    .timeline-item { border-left: 4px solid var(--accent); padding-left: 18px; }
    .timeline-item h3 { margin-bottom: 6px; }
    .timeline-item p { margin-top: 0; color: var(--muted); }

    .list { padding-left: 20px; color: var(--muted); }
    .list li { margin-bottom: 8px; }

    footer {
      background: #1f2933;
      color: #e5e7eb;
      padding: 28px 0;
      text-align: center;
    }

    @media (max-width: 820px) {
      .hero-inner, .grid-2, .grid-3, .mosaic-grid { grid-template-columns: 1fr; }
      .nav { flex-direction: column; justify-content: center; padding: 18px 0; }
      .hero { padding-top: 52px; }
      .mosaic-card:nth-child(2) { transform: none; }
      .sticker { width: 82px; opacity: 0.11; }
      .sticker.three, .sticker.four, .sticker.five, .sticker.six, .sticker.seven, .sticker.eight { display: none; }
    }
  </style>
</head>
<body>
  <div class="sticker-layer" aria-hidden="true">
    <img class="sticker profile-sticker" src="/assets/images/gaikovina-profile.png" alt="Gaikovina Amini">
    <img class="sticker one" src="/assets/images/culture-detail-1.jpg" alt="">
    <img class="sticker two" src="/assets/images/culture-detail-2.jpg" alt="">
    <img class="sticker three" src="/assets/images/culture-detail-3.jpg" alt="">
    <img class="sticker four" src="/assets/images/culture-bg-1.jpg" alt="">
    <img class="sticker five" src="/assets/images/culture-bg-2.jpg" alt="">
    <img class="sticker six" src="/assets/images/culture-detail-2.jpg" alt="">
    <img class="sticker seven" src="/assets/images/sticker-img-5714.jpg" alt="">
    <img class="sticker eight" src="/assets/images/sticker-img-5713.jpg" alt="">
  </div>

  <header>
    <div class="container nav">
      <div class="brand">GAIKOVINA AMINI</div>
      <nav class="nav-links" aria-label="Main navigation">
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#experience">Experience</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-inner">
        <div>
          <span class="eyebrow">Accounting & Finance Student</span>
          <h1>Professional Profile — Gaikovina Amini</h1>
          <p class="lead">
            I am an aspiring accounting and finance professional with a strong interest in auditing, bookkeeping, and corporate financial management. Originally from Papua New Guinea and currently studying in Japan, I am building a strong foundation in academic knowledge and practical financial skills.
          </p>
          <div class="actions">
            <a class="button primary" href="mailto:aminigaikovin7@gmail.com">Contact Me</a>
            <a class="button secondary" href="#experience">View Experience</a>
          </div>
        </div>

        <aside class="profile-card" aria-label="Profile summary">
          <img class="profile-photo" src="/assets/images/gaikovina-profile.png" alt="Gaikovina Amini" style="max-width:220px;width:90vw;margin-bottom:16px;box-shadow:0 4px 36px rgba(40,40,45,0.13), 0 1px 8px rgba(0,0,0,0.07);border-radius:22px;">
          <ul class="quick-list">
            <li><strong>Name:</strong> Gaikovina Amini</li>
            <li><strong>University:</strong> Ritsumeikan Asia Pacific University</li>
            <li><strong>Major:</strong> Accounting / Finance</li>
            <li><strong>Expected Graduation:</strong> 2027</li>
            <li><strong>Nationality:</strong> Papua New Guinean</li>
            <li><strong>Location:</strong> Japan</li>
          </ul>
        </aside>
      </div>
    </section>


    <section id="about" class="culture-section">
      <div class="container">
        <h2 class="section-title">About Me</h2>
        <p class="section-copy">
          I am a proud Papua New Guinean who values diversity and enjoys working with people from many different cultures. Through my experiences in PNG and Japan, I’ve collaborated with teams from various backgrounds and learned the importance of cultural understanding. I like solving problems, I like numbers, and I’m passionate about using both to create meaningful results in any environment.
        </p>
        <div class="grid-2">
          <div class="about-box">
            <h3>Education</h3>
            <p><strong>Ritsumeikan Asia Pacific University (APU)</strong><br>Bachelor’s Degree — Accounting / Finance Major<br>Expected Graduation: 2027</p>
          </div>
          <div class="about-box">
            <h3>Career Goals</h3>
            <div class="tag-list">
              <span class="tag">Audit</span><span class="tag">Tax</span><span class="tag">Bookkeeping</span><span class="tag">Corporate Accounting</span><span class="tag">Financial Analysis</span><span class="tag">Budgeting</span><span class="tag">Finance</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="skills">
      <div class="container">
        <h2 class="section-title">Skills</h2>
        <p class="section-copy">Practical skills I am developing through study, projects, leadership, and real experience.</p>
        <div class="grid-3">
          <article class="card"><h3>Web Design & Website Management</h3><p>Creating, updating, and managing clean websites for events and projects.</p></article>
          <article class="card"><h3>Communication</h3><p>English fluent, Japanese intermediate, teamwork, collaboration, and organizing.</p></article>
          <article class="card"><h3>Accounting Software Integration</h3><p>Experience helping integrate accounting software with hotel operations, including bar, booking, and restaurant systems.</p></article>
          <article class="card"><h3>Event Organization</h3><p>Helped organize large cultural events such as Pasifika Week, including planning, coordination, and team support.</p></article>
          <article class="card"><h3>Administration</h3><p>Documentation, scheduling, data entry, communication, and financial tracking support.</p></article>
          <article class="card"><h3>Accounting & Finance Foundations</h3><p>Currently building knowledge in bookkeeping, budgeting, financial statements, and accounting concepts.</p></article>
        </div>
      </div>
    </section>

    <section id="leadership" class="culture-section alt">
      <div class="container">
        <h2 class="section-title">Leadership & Organizing Roles</h2>
        <div class="grid-2">
          <article class="card"><h3>Vice President — PIA, APU</h3><p>Organizing cultural events, supporting Pacific Island students, coordinating meetings, and representing the Pacific community.</p></article>
          <article class="card"><h3>Group Project Leader</h3><p>Managed schedules, delegated tasks, coordinated shared documents, and helped ensure deadlines were met.</p></article>
          <article class="card"><h3>Event Organizer</h3><p>Planned student activities, coordinated logistics, communicated with participants, and supported teamwork.</p></article>
          <article class="card"><h3>Workplace Leadership</h3><p>Guided new staff, organized daily tasks, and maintained workflow during busy periods.</p></article>
        </div>
      </div>
    </section>

    <section id="experience">
      <div class="container">
        <h2 class="section-title">Experience</h2>
        <div class="timeline">
          <div class="timeline-item"><h3>Hotel Accounting System Integration Project</h3><p>Managed the integration of accounting systems into hotel operations, connecting bar, booking, and restaurant systems with financial platforms for real-time budgeting and expense tracking. Oversaw planning, implementation, and staff coordination.</p></div>
          <div class="timeline-item"><h3>Administrator — Niugini Native</h3><p>Handled documentation, communication, scheduling, financial tracking, data entry, reporting, and departmental coordination.</p></div>
          <div class="timeline-item"><h3>Women Entrepreneurs Non-Profit Organization — Part-Time</h3><p>Supported event coordination, administrative tasks, financial tracking, and community outreach for women entrepreneurs.</p></div>
          <div class="timeline-item"><h3>ASPA — Cultural Advocacy</h3><p>Participated in events promoting Papua New Guinea’s culture and identity through presentations, activities, and advocacy initiatives in Japan.</p></div>
          <div class="timeline-item"><h3>CleanGen Papua New Guinea — Member</h3><p>Contributed to youth-focused environmental and community projects, awareness campaigns, sustainability activities, and volunteer programs.</p></div>
          <div class="timeline-item"><h3>Leadership — Port Moresby International School</h3><p>Served as a student leader for UN cultural events and school cultural programs, organizing performances and representing PNG culture.</p></div>
          <div class="timeline-item"><h3>Rugby Career</h3><p>Played competitively from high school to premier grade, including Valley Hunters U20, Valley Hunters Premier Grade debut at age 18, and rugby in Japan while studying.</p></div>
        </div>
      </div>
    </section>

    <section id="projects">
      <div class="container">
        <h2 class="section-title">Projects & Courses</h2>
        <div class="grid-2">
          <div class="card">
            <h3>Projects</h3>
            <ul class="list">
              <li><strong>Accounting System Integration for Bars, Booking & Restaurants:</strong> Integrated accounting systems into operations to streamline financial tracking, budgeting, and reporting.</li>
              <li><strong>ICT Cluster PNG — Non-Profit Support Work:</strong> Contributed to ICT Cluster initiatives in Papua New Guinea, supporting digital development and community technology projects.</li>
              <li><strong>Web Manager — Bridges 2026:</strong> Managed and updated the official Bridges 2026 event website, ensuring smooth digital communication and content management. <a href="https://bridges-png.github.io/2026/" target="_blank" rel="noopener">Visit website</a>.</li>
              <li><strong>Financial Statement Analysis:</strong> Reviewed company statements and identified trends.</li>
              <li><strong>Budget Planning Assignment:</strong> Created monthly budgets with income, expenses, and savings goals.</li>
            </ul>
          </div>
          <div class="card">
            <h3>Certifications & Courses</h3>
            <ul class="list">
              <li>Introduction to Accounting</li>
              <li>Financial Accounting Basics</li>
              <li>Excel for Business</li>
              <li>Bookkeeping Fundamentals</li>
              <li>Japanese Language Courses — Beginner to Intermediate</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section id="team" class="culture-section">
      <div class="container">
        <h2 class="section-title">Team Member</h2>
        <div class="about-box">
          <h3>Charles Yatna</h3>
          <p>Collaborator involved in organizing tasks, coordinating group activities, and supporting project planning. Works closely with Gaikovina on student projects, budgeting tasks, and leadership roles.</p>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <h2 class="section-title">Contact</h2>
        <p class="section-copy">Available for accounting, finance, leadership, student project, and professional networking opportunities.</p>
        <div class="actions">
          <a class="button primary" href="mailto:aminigaikovin7@gmail.com">aminigaikovin7@gmail.com</a>
          <a class="button secondary" href="#">Instagram: Charles yatna</a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">© 2026 Gaikovina Amini. All rights reserved.</div>
  </footer>
</body>
</html>
