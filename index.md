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
      --bg: #f6f7f4;
      --panel: #ffffff;
      --ink: #1f2933;
      --muted: #52606d;
      --accent: #2f6f6b;
      --accent-dark: #235552;
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

    .hero { padding: 82px 0 50px; }

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
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: 20px;
      box-shadow: var(--shadow);
    }

    .profile-card { padding: 28px; }

    .photo-placeholder {
      min-height: 210px;
      border: 2px dashed var(--border);
      border-radius: 18px;
      background: linear-gradient(135deg, var(--accent-soft), #fff);
      display: grid;
      place-items: center;
      text-align: center;
      color: var(--muted);
      padding: 20px;
      margin-bottom: 20px;
    }

    .quick-list { list-style: none; padding: 0; margin: 0; }
    .quick-list li { padding: 10px 0; border-bottom: 1px solid var(--border); }
    .quick-list li:last-child { border-bottom: none; }
    .quick-list strong { color: var(--ink); }

    section { padding: 54px 0; }

    .section-copy {
      color: var(--muted);
      max-width: 760px;
      margin: 0 0 28px;
    }

    .grid-2 { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 22px; }
    .grid-3 { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 22px; }

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
      .hero-inner, .grid-2, .grid-3 { grid-template-columns: 1fr; }
      .nav { flex-direction: column; justify-content: center; padding: 18px 0; }
      .hero { padding-top: 52px; }
    }
  </style>
</head>
<body>
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
            <a class="button primary" href="mailto:gaikovina7@gmail.com">Contact Me</a>
            <a class="button secondary" href="#experience">View Experience</a>
          </div>
        </div>

        <aside class="profile-card" aria-label="Profile summary">
          <div class="photo-placeholder">
            <div>
              <strong>Professional Headshot</strong><br>
              Photo placeholder
            </div>
          </div>
          <ul class="quick-list">
            <li><strong>Name:</strong> Gaikovina Amini</li>
            <li><strong>University:</strong> Ritsumeikan Asia Pacific University</li>
            <li><strong>Major:</strong> Accounting / Finance</li>
            <li><strong>Expected Graduation:</strong> 2027</li>
            <li><strong>Location:</strong> Japan</li>
          </ul>
        </aside>
      </div>
    </section>

    <section id="about">
      <div class="container">
        <h2 class="section-title">About Me</h2>
        <p class="section-copy">
          I enjoy working with numbers, solving problems, and creating clear financial insights that support better decision-making. My long-term goal is to grow into a reliable and skilled accounting specialist.
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
        <p class="section-copy">A growing set of technical, professional, and leadership skills for accounting and finance work.</p>
        <div class="grid-3">
          <article class="card"><h3>Accounting Software</h3><p>QuickBooks, Xero, MYOB</p></article>
          <article class="card"><h3>Microsoft Excel</h3><p>Pivot tables, formulas, financial modeling, expense tracking, and automation.</p></article>
          <article class="card"><h3>Financial Statements</h3><p>Preparation, analysis, reporting, trends, and key ratios.</p></article>
          <article class="card"><h3>Bookkeeping</h3><p>Accounts payable/receivable, reconciliations, records, and accuracy.</p></article>
          <article class="card"><h3>Tax & Budgeting</h3><p>Tax basics, monthly budgets, forecasting, and variance analysis.</p></article>
          <article class="card"><h3>Communication</h3><p>English fluent, Japanese intermediate, teamwork, collaboration, and organizing.</p></article>
        </div>
      </div>
    </section>

    <section id="leadership">
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
          <div class="timeline-item"><h3>Hotel Accounting System Integration Project</h3><p>Managed a full accounting system integration for a hotel, connecting operations with a financial platform for real-time visibility of budgets, expenses, and financial performance.</p></div>
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
              <li>Financial Statement Analysis</li>
              <li>Budget Planning Assignment</li>
              <li>Accounting Report</li>
              <li>Excel Automation for expense tracking</li>
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

    <section id="team">
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
          <a class="button primary" href="mailto:gaikovina7@gmail.com">gaikovina7@gmail.com</a>
          <a class="button secondary" href="#">Instagram: Charles_yatna_</a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">© 2026 Gaikovina Amini. All rights reserved.</div>
  </footer>
</body>
</html>
