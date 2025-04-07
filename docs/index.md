<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AutoDev Vault</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap" rel="stylesheet">
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
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    nav {
      background: linear-gradient(to right, #0077ff, #00cfff);
      padding: 1rem 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    .nav-left {
      font-family: 'Poppins', sans-serif;
      font-size: 1.5rem;
      font-weight: bold;
      color: white;
      display: flex;
      align-items: center;
    }

    .nav-links {
      display: flex;
      gap: 1.5rem;
      flex-wrap: wrap;
      justify-content: center;
      margin-top: 0.5rem;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      font-size: 1rem;
      transition: all 0.3s ease;
    }

    .nav-links a:hover {
      text-decoration: underline;
      transform: scale(1.05);
    }

    .search-box {
      display: flex;
      align-items: center;
      margin-top: 0.5rem;
    }

    .search-box input {
      padding: 0.4rem 1rem;
      border-radius: 20px;
      border: none;
      font-size: 0.9rem;
      outline: none;
      box-shadow: 0 0 5px rgba(0,0,0,0.2);
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 2rem;
    }

    header {
      text-align: center;
      padding: 3rem 1rem 2rem;
      position: relative;
    }

    .logo {
      font-family: 'Poppins', sans-serif;
      font-size: 3rem;
      color: var(--accent);
      animation: pulse 1.8s infinite alternate;
      letter-spacing: 1px;
    }

    @keyframes pulse {
      from { transform: scale(1); opacity: 0.8; }
      to { transform: scale(1.05); opacity: 1; }
    }

    header p {
      font-size: 1.1rem;
      max-width: 800px;
      margin: 1rem auto 0;
    }

    .dark-toggle {
      position: absolute;
      top: 1rem;
      right: 1.5rem;
      background: none;
      border: 2px solid var(--accent);
      border-radius: 20px;
      padding: 0.4rem 1rem;
      cursor: pointer;
      color: var(--accent);
      font-weight: bold;
      transition: background 0.3s, color 0.3s;
    }

    .dark-toggle:hover {
      background: var(--accent);
      color: #fff;
    }

    .topics {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 1.5rem;
      margin-top: 3rem;
    }

    .card {
      background-color: var(--card);
      border-radius: 15px;
      padding: 1.5rem;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      cursor: pointer;
      text-decoration: none;
      color: inherit;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgba(0,0,0,0.15);
    }

    .card h3 {
      color: var(--accent);
      margin-bottom: 0.5rem;
    }

    .card p {
      font-size: 0.9rem;
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
  <nav>
    <div class="nav-left">AutoDev Vault</div>
    <div class="nav-links">
      <a href="index.html">Home</a>
      <a href="mbd.md">Model-Based Development (MBD)</a>
      <a href="cbd.md">Code-Based Development (CBD)</a>
      <a href="simulink.md">Simulink</a>
      <a href="stateflow.md">Stateflow</a>
      <a href="autsar.md">AUTOSAR & RTE</a>
      <a href="polyspace.md">PolySpace & SonarQube</a>
      <a href="tools.md">Tools & Scripting</a>
      <a href="testing.md">Testing & Safety</a>
      <a href="system.md">System Design & Integration</a>
    </div>
    <div class="search-box">
      <input type="text" placeholder="🔍 Search topics..." />
    </div>
  </nav>

  <div class="container">
    <header>
      <div class="logo">🚗 AutoDev Vault</div>
      <p>A rich questionnaire for the Automotive domain focused on practical technical topics. This will help you in cracking interviews, strengthening fundamentals, and understanding real-world systems in MBD, Simulink, Stateflow, and more!</p>
      <button class="dark-toggle" onclick="toggleTheme()">🌗 Toggle Theme</button>
    </header>

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

    <footer>
      Made with ❤️ by Mahija
    </footer>
  </div>

  <script>
    function toggleTheme() {
      const html = document.documentElement;
      const current = html.getAttribute('data-theme');
      html.setAttribute('data-theme', current === 'dark' ? 'light' : 'dark');
    }
  </script>
</body>
</html>
