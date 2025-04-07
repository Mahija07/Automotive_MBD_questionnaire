<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AutoDev Vault</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-dark: #121212;
      --card-dark: #1e1e2f;
      --text-dark: #e0e0e0;
      --accent-dark: #00d9ff;
      --nav-dark: #0d47a1;
    }

    html[data-theme="dark"] {
      --bg: var(--bg-dark);
      --card: var(--card-dark);
      --text: var(--text-dark);
      --accent: var(--accent-dark);
      --nav: var(--nav-dark);
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    header {
      background-color: var(--nav);
      color: white;
      padding: 1.2rem 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    header .logo {
      font-family: 'Poppins', sans-serif;
      font-size: 1.8rem;
      color: var(--accent);
    }

    .container {
      max-width: 1100px;
      margin: auto;
      padding: 2rem 1rem;
    }

    .description {
      text-align: center;
      font-size: 1.1rem;
      margin-bottom: 2rem;
    }

    .topics {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }

    .card {
      display: block;
      background-color: var(--card);
      color: inherit;
      border-radius: 12px;
      padding: 1.2rem;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
      text-decoration: none;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.25);
    }

    .card h3 {
      margin-top: 0;
      margin-bottom: 0.5rem;
      color: var(--accent);
    }

    .card p {
      margin: 0;
      font-size: 0.9rem;
    }

    footer {
      text-align: center;
      padding: 2rem 1rem;
      font-size: 0.85rem;
      color: #aaa;
    }

    .nav-links {
      display: flex;
      gap: 1.2rem;
      flex-wrap: wrap;
      font-size: 0.9rem;
    }

    .nav-links a {
      color: #ffffff;
      text-decoration: none;
      font-weight: 600;
    }

    .nav-links a:hover {
      color: var(--accent);
    }

    .dark-toggle {
      background: none;
      border: 2px solid var(--accent);
      border-radius: 18px;
      padding: 0.4rem 0.8rem;
      cursor: pointer;
      color: var(--accent);
      font-weight: bold;
      transition: background 0.3s, color 0.3s;
    }

    .dark-toggle:hover {
      background: var(--accent);
      color: #000;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">🚗 AutoDev Vault</div>
    <div class="nav-links">
      <a href="mbd.md">Model-Based Dev</a>
      <a href="cbd.md">Code-Based Dev</a>
      <a href="simulink.md">Simulink</a>
      <a href="stateflow.md">Stateflow</a>
      <a href="autsar.md">AUTOSAR</a>
      <a href="polyspace.md">Polyspace</a>
      <a href="tools.md">Tools</a>
      <a href="testing.md">Testing</a>
      <a href="system.md">System</a>
    </div>
    <button class="dark-toggle" onclick="toggleTheme()">🌗</button>
  </header>

  <div class="container">
    <div class="description">
      <strong>AutoDev Vault</strong> is a comprehensive interview prep guide for professionals in the Automotive industry.
      Dive into MBD, Simulink, Stateflow, Testing, and more with curated Q&A sets.
    </div>

    <section class="topics">
      <a class="card" href="mbd.md"><h3>⚙️ Model-Based Development</h3><p>Simulink | Stateflow | TLC | SIL | MIL</p></a>
      <a class="card" href="cbd.md"><h3>💻 Code-Based Development</h3><p>C | Embedded C | MISRA | Unit Testing</p></a>
      <a class="card" href="simulink.md"><h3>📊 Simulink</h3><p>Subsystems | Masking | Solvers</p></a>
      <a class="card" href="stateflow.md"><h3>🔁 Stateflow</h3><p>Events | States | Logic | Transitions</p></a>
      <a class="card" href="autsar.md"><h3>🧩 AUTOSAR & RTE</h3><p>Modules | RTE | Com Stack</p></a>
      <a class="card" href="polyspace.md"><h3>📋 PolySpace & SonarQube</h3><p>Static Analysis & Compliance</p></a>
      <a class="card" href="tools.md"><h3>🛠 Tools & Scripting</h3><p>MATLAB | M-Scripting | Python | Git | VSCode</p></a>
      <a class="card" href="testing.md"><h3>✅ Testing & Safety</h3><p>Google Test | ISO-26262 | JAMA | JIRA</p></a>
      <a class="card" href="system.md"><h3>🔧 System Design & Integration</h3><p>Preevision | MagicDraw | Zonal Modules</p></a>
    </section>
  </div>

  <footer>
    Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages
  </footer>

  <script>
    function toggleTheme() {
      const html = document.documentElement;
      const current = html.getAttribute('data-theme');
      html.setAttribute('data-theme', current === 'dark' ? 'light' : 'dark');
    }
  </script>
</body>
</html>
