<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AutoDev Vault</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600&family=Roboto&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <style>
    :root {
      --bg-light: #f7f9fc;
      --card-light: #ffffff;
      --text-light: #222;
      --accent: #005f73;

      --bg-dark: #1a1a2e;
      --card-dark: #2e2e3e;
      --text-dark: #f0f0f0;
      --accent-dark: #00d9ff;
    }

    html[data-theme="light"] {
      --bg: var(--bg-light);
      --card: var(--card-light);
      --text: var(--text-light);
      --accent: var(--accent);
    }

    html[data-theme="dark"] {
      --bg: var(--bg-dark);
      --card: var(--card-dark);
      --text: var(--text-dark);
      --accent: var(--accent-dark);
    }

    body {
      margin: 0;
      font-family: 'Roboto', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    header {
      background-color: var(--card);
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
      position: sticky;
      top: 0;
      z-index: 1000;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-family: 'Poppins', sans-serif;
      font-size: 1.8rem;
      font-weight: 600;
      color: var(--accent);
      animation: pulse 2s infinite alternate;
    }

    @keyframes pulse {
      from { transform: scale(1); opacity: 0.8; }
      to { transform: scale(1.05); opacity: 1; }
    }

    .dark-toggle {
      background: var(--accent);
      border: none;
      border-radius: 30px;
      padding: 0.5rem 1rem;
      color: #fff;
      cursor: pointer;
      font-weight: bold;
      transition: background 0.3s;
    }

    .dark-toggle:hover {
      background: #0099cc;
    }

    .intro {
      text-align: center;
      padding: 2rem 1rem 1rem;
      max-width: 900px;
      margin: auto;
    }

    .intro p {
      font-size: 1.1rem;
      line-height: 1.6;
    }

    .topics {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2rem;
      padding: 2rem;
    }

    .card {
      background-color: var(--card);
      border-radius: 16px;
      padding: 1.5rem;
      box-shadow: 0 8px 24px rgba(0,0,0,0.15);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      cursor: pointer;
      text-decoration: none;
      color: inherit;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 12px 32px rgba(0,0,0,0.2);
    }

    .card h3 {
      margin-bottom: 0.5rem;
      color: var(--accent);
      font-family: 'Poppins', sans-serif;
    }

    .card p {
      font-size: 0.95rem;
      color: var(--text);
    }

    footer {
      text-align: center;
      padding: 2rem 1rem;
      font-size: 0.85rem;
      color: #aaa;
    }

    .back-to-top {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: var(--accent);
      color: white;
      padding: 0.6rem 0.8rem;
      border: none;
      border-radius: 50%;
      font-size: 1rem;
      cursor: pointer;
      display: none;
      box-shadow: 0 4px 12px rgba(0,0,0,0.25);
    }

    .back-to-top.show {
      display: block;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">🚗 AutoDev Vault</div>
    <button class="dark-toggle" onclick="toggleTheme()">🌗 Theme</button>
  </header>

  <div class="intro">
    <p><strong>AutoDev Vault</strong> is a comprehensive interview prep guide designed for professionals in the Automotive industry. Dive into MBD, Simulink, Stateflow, Testing, and more with curated Q&A sets.</p>
  </div>

  <section class="topics">
    <a class="card" href="mbd.md"><h3>⚙️ Model-Based Development</h3><p>Simulink | Stateflow | TLC | SIL | MIL</p></a>
    <a class="card" href="cbd.md"><h3>💻 Code-Based Development</h3><p>C | Embedded C | MISRA | Unit Testing</p></a>
    <a class="card" href="simulink.md"><h3>📊 Simulink</h3><p>Subsystems | Masking | Solvers</p></a>
    <a class="card" href="stateflow.md"><h3>🔁 Stateflow</h3><p>Events | States | Logic | Transitions</p></a>
    <a class="card" href="autsar.md"><h3>🧩 AUTOSAR & RTE</h3><p>Modules | RTE | Com Stack</p></a>
    <a class="card" href="polyspace.md"><h3>📋 Polyspace & SonarQube</h3><p>Static Analysis & Compliance</p></a>
    <a class="card" href="tools.md"><h3>🛠 Tools & Scripting</h3><p>MATLAB | M-Scripting | Python | Git | VSCode</p></a>
    <a class="card" href="testing.md"><h3>✅ Testing & Safety</h3><p>Google Test | ISO-26262 | JAMA | JIRA</p></a>
    <a class="card" href="system.md"><h3>🔧 System Design & Integration</h3><p>Preevision | MagicDraw | Zonal Modules</p></a>
  </section>

  <footer>
    Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages
  </footer>

  <button id="backToTop" class="back-to-top" onclick="window.scrollTo({ top: 0, behavior: 'smooth' });">
    ↑
  </button>

  <script>
    function toggleTheme() {
      const html = document.documentElement;
      const current = html.getAttribute('data-theme');
      html.setAttribute('data-theme', current === 'dark' ? 'light' : 'dark');
    }

    window.addEventListener('scroll', () => {
      const backToTopBtn = document.getElementById('backToTop');
      if (window.scrollY > 300) {
        backToTopBtn.classList.add('show');
      } else {
        backToTopBtn.classList.remove('show');
      }
    });
  </script>

</body>
</html>
