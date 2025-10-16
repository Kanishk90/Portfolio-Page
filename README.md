<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1.0">
  <title>Data Science Enthusiast Portfolio</title>
  <style>
    :root {
      --primary: #234567;
      --accent: #16a085;
      --bg-light: #f8f9fa;
      --text-dark: #223;
      --card-bg: #fff;
      --shadow: 0 4px 12px rgba(60,60,100,0.08);
    }
    body { font-family:"Segoe UI",Arial,sans-serif; margin:0; background: var(--bg-light); color: var(--text-dark); }
    header {
      background: var(--primary);
      color: #fff;
      padding: 40px 0 20px;
      text-align: center;
      box-shadow: var(--shadow);
    }
    header h1 { margin-bottom: 10px; font-size: 2.5rem; }
    nav {
      margin-top: 12px;
    }
    nav a {
      color: #fff; text-decoration: none; margin:0 12px; font-weight:bold; transition: color 0.2s;
    }
    nav a:hover { color: var(--accent); }
    .container { max-width: 900px; margin: auto; padding: 28px 12px;}
    section {margin-bottom:38px;}

    /* Responsive grid */
    .grid { display: flex; gap: 18px; flex-wrap:wrap;}
    .card {
      background: var(--card-bg);
      border-radius: 13px;
      box-shadow: var(--shadow);
      padding: 22px;
      flex: 1 1 220px;
      min-width: 220px;
      transition: transform 0.14s;
    }
    .card:hover { transform: translateY(-7px) scale(1.03); background: #eef7f7; }

    /* Project Links */
    .card a { color: var(--accent); text-decoration: underline; word-break:break-all;}
    .card strong {color: var(--accent);}

    /* Skills badges */
    .skill-badge {
      display: inline-block;
      background: var(--accent);
      color: #fff;
      padding:4px 11px;
      border-radius: 12px;
      margin: 2px 7px 2px 0;
      font-size: .98em;
      font-weight: 600;
      box-shadow:0 1px 5px rgba(15,120,100,0.14);
    }

    /* Contact inputs */
    form input, form textarea {
      width: 100%; padding: 9px; margin:4px 0 18px; border: 1px solid #ccc; border-radius:7px;
      font-size:1em;
      background:#f6f6f6;
      resize:vertical;
    }
    form input[type=submit] {
      background: var(--primary); color: #fff; font-weight:700; border: none; cursor:pointer;
      transition: background 0.2s;
    }
    form input[type=submit]:hover { background: var(--accent); }

    /* Footer */
    footer { background: var(--primary); color: #fff; text-align:center; padding: 14px 0; margin-top:30px; font-size:1em; }

    /* Responsive Design */
    @media (max-width:600px) {
      header h1 { font-size:1.4rem;}
      .container { padding:12px 3px;}
      .grid { flex-direction:column; gap:13px; }
      .card { min-width:100%; }
      nav a { margin:0 7px; font-size:.98em;}
    }
  </style>
</head>
<body>
  <header>
    <h1>Your Name</h1>
    <p>Data Science Enthusiast · Programmer · Machine Learning Explorer</p>
    <nav>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#education">Education</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>
  <div class="container">
    <section id="about">
      <h2>About Me</h2>
      <div class="card">Welcome! I'm passionate about Data Science, Machine Learning, and Web Scraping.<br>
        Computer Science student with hands-on experience on open source, Kaggle, and IITM courses.
      </div>
    </section>
    <section id="skills">
      <h2>Skills</h2>
      <div class="grid">
        <div class="card"><span class="skill-badge">Python</span><span class="skill-badge">Pandas</span><span class="skill-badge">NumPy</span><span class="skill-badge">Jupyter</span></div>
        <div class="card"><span class="skill-badge">Machine Learning</span><span class="skill-badge">Scikit-learn</span><span class="skill-badge">Deep Learning</span></div>
        <div class="card"><span class="skill-badge">Web Scraping</span><span class="skill-badge">BeautifulSoup</span><span class="skill-badge">Selenium</span></div>
        <div class="card"><span class="skill-badge">Data Viz</span><span class="skill-badge">Matplotlib</span><span class="skill-badge">Seaborn</span></div>
        <div class="card"><span class="skill-badge">Git</span><span class="skill-badge">GitHub</span></div>
        <div class="card"><span class="skill-badge">Google Cloud</span><span class="skill-badge">Kaggle</span></div>
      </div>
    </section>
    <section id="projects">
      <h2>Projects</h2>
      <div class="grid">
        <div class="card">
          <strong>Agmarknet Web Scraper</strong><br>
          Extract agricultural market data from HTML tables, handle irregular structures, export clean CSVs. <br>
          <a href="https://github.com/yourusername/agmarknet-scraper" target="_blank">GitHub Repo</a>
        </div>
        <div class="card">
          <strong>MNIST Classification</strong><br>
          Image classifier for handwritten digits using neural networks and pandas. <br>
          <a href="https://github.com/yourusername/mnist-classification" target="_blank">GitHub Repo</a>
        </div>
        <div class="card">
          <strong>MLOps Pipeline</strong><br>
          Automated model versioning with DVC & Google Cloud Storage for reproducible ML projects. <br>
          <a href="https://github.com/yourusername/mlops-pipeline" target="_blank">GitHub Repo</a>
        </div>
      </div>
    </section>
    <section id="education">
      <h2>Education</h2>
      <div class="grid">
        <div class="card">B.Sc. Data Science, IITM Online Degree (Year - Present)</div>
        <div class="card">NPTEL Quantum Computing Course (2025)</div>
      </div>
    </section>
    <section id="contact">
      <h2>Contact</h2>
      <form action="mailto:your.email@gmail.com" method="POST" enctype="text/plain">
        <input type="text" name="name" placeholder="Your Name" required>
        <input type="email" name="email" placeholder="Your Email" required>
        <textarea name="message" rows="4" placeholder="Your Message"></textarea>
        <input type="submit" value="Send">
      </form>
    </section>
  </div>
  <footer>
    &copy; 2025 Your Name. Made with 💡 for Data Science.
  </footer>
</body>
</html>
