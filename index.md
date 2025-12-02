<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gaikovina Portfolio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f9f9f9;
      color: #333;
    }
    header {
      background-color: #004466;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      background-color: #003344;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      padding: 40px;
      max-width: 900px;
      margin: auto;
    }
    h1, h2 {
      color: #004466;
    }
    .projects {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
    }
    .project-card {
      background: white;
      border: 1px solid #ddd;
      padding: 20px;
      flex: 1 1 250px;
      box-shadow: 2px 2px 5px rgba(0,0,0,0.1);
    }
    footer {
      background-color: #004466;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Gaikovina Portfolio</h1>
    <p>Web Design & Development for Small Businesses</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Me</h2>
    <p>
      I design clear, accessible websites for small companies. My focus is on 
      simple layouts, mobile-friendly design, and practical features that help 
      businesses connect with customers.
    </p>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="project-card">
        <h3>Café Website</h3>
        <p>A demo site for a local café, featuring menu pages and contact form.</p>
      </div>
      <div class="project-card">
        <h3>Tutoring Service</h3>
        <p>Clean, professional site with booking system for lessons.</p>
      </div>
      <div class="project-card">
        <h3>Salon Website</h3>
        <p>Modern design with gallery and appointment scheduling.</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:yourname@email.com">yourname@email.com</a></p>
    <p>LinkedIn: <a href="#">Your LinkedIn Profile</a></p>
  </section>

  <footer>
    <p>&copy; 2025 Gaikovina. All rights reserved.</p>
  </footer>

</body>
</html>