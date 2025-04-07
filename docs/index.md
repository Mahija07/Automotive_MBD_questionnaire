<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AutoDev Vault</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600&family=Roboto&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-light: #f7f9fc;
      --card-light: #ffffff;
      --text-light: #222;
      --accent: #0077cc;

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
      background: linear-gradient(90deg, #0077cc, #00d9ff);
      color: #fff;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-family: 'Poppins', sans-serif;
      font-size: 1.3rem;
      font-weight: bold;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .intro {
      text-align: center;
      padding: 2rem 1rem;
      max-width: 800px;
      margin: auto;
    }

    .dark-toggle {
      background: var(--accent);
      border: none;
      border-radius: 20px;
      padding: 0.5rem 1rem;
      color: #fff;
      cursor: pointer;
      font-weight: bold;
      font-size: 0.9rem;
      transition: background 0.3s;
    }

    .dark-toggle:hover {
      background: #0099cc;
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
    }

    footer {
      text-align: center;
      padding: 2rem 1rem;
      font-size: 0.85rem;
      color: #aaa;
    }
  </style>
</head>
<body>
  <header>
    🚗 AutoDev Vault
    <button class="dark-toggle" onclick="toggleTheme()">🌗 Theme</button>
  </header>

  <section class="intro">
    <p><strong>AutoDev Vault</strong> is a comprehensive interview prep guide designed for professionals in the Automotive industry.<br>
    Dive into MBD, Simulink, Stateflow, Testing, and more with curated Q&A sets.</p>
  </section>

  <section class="topics">
    <a class="card" href="mbd/"><h3>⚙️ Model-Based Development</h3><p>Simulink | Stateflow | TLC | SIL | MIL</p></a>
    <a class="card" href="cbd/"><h3>💻 Code-Based Development</h3><p>C | Embedded C | MISRA | Unit Testing</p></a>
    <a class="card" href="simulink/"><h3>📊 Simulink</h3><p>Subsystems | Masking | Solvers</p></a>
    <a class="card" href="stateflow/"><h3>🔁 Stateflow</h3><p>Events | States | Logic | Transitions</p></a>
    <a class="card" href="autsar/"><h3>🧩 AUTOSAR & RTE</h3><p>Modules | RTE | Com Stack</p></a>
    <a class="card" href="polyspace/"><h3>📋 PolySpace & SonarQube</h3><p>Static Analysis & Compliance</p></a>
    <a class="card" href="tools/"><h3>🛠 Tools & Scripting</h3><p>MATLAB | M-Scripting | Python | Git | VSCode</p></a>
    <a class="card" href="testing/"><h3>✅ Testing & Safety</h3><p>Google Test | ISO-26262 | JAMA | JIRA</p></a>
    <a class="card" href="system/"><h3>🔧 System Design & Integration</h3><p>Preevision | MagicDraw | Zonal Modules</p></a>
  </section>

  <footer>
    Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages
  </footer>

  <script>
    function toggleTheme() {
      const html = document.documentElement;
      const current = html.getAttribute('data-theme');
      html.setAttribute('data-theme', current === 'dark' ? 'light' : 'dark');
      localStorage.setItem('theme', html.getAttribute('data-theme'));
    }

    window.addEventListener('DOMContentLoaded', () => {
      const savedTheme = localStorage.getItem('theme');
      if (savedTheme) {
        document.documentElement.setAttribute('data-theme', savedTheme);
      } else {
        const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
        document.documentElement.setAttribute('data-theme', prefersDark ? 'dark' : 'light');
      }
    });
  </script>
</body>
</html>
