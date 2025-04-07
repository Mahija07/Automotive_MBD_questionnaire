<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AutoDev Vault</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600&family=Roboto&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-dark: #121212;
      --card-dark: #1e1e2f;
      --text-dark: #f5f5f5;
      --accent-dark: #00d9ff;
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
      position: sticky;
      top: 0;
      z-index: 1000;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
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

    .intro {
      text-align: center;
      padding: 2rem 1rem 1rem;
      max-width: 900px;
      margin: auto;
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
      box-shadow: 0 12px 32px rgba(0,0,0,0.3);
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

  <section class="intro">
    <p>Welcome to the Automotive MBD Questionnaire Vault 🚀<br/>Perfect your interviews, dive into MBD, Simulink, Stateflow, and more!</p>
  </section>

  <section class="topics">
    <a class="card" href="MBD.md"><h3>⚙️ Model-Based Development</h3><p>Simulink | Stateflow | TLC | SIL | MIL</p></a>
    <a class="card" href="CBD.md"><h3>💻 Code-Based Development</h3><p>C | Embedded C | MISRA | Unit Testing</p></a>
    <a class="card" href="Simulink.md"><h3>📊 Simulink</h3><p>Subsystems | Masking | Solvers</p></a>
    <a class="card" href="Stateflow.md"><h3>🔁 Stateflow</h3><p>Events | States | Logic | Transitions</p></a>
    <a class="card" href="autsar.md"><h3>🧩 AUTOSAR & RTE</h3><p>Modules | RTE | Com Stack</p></a>
    <a class="card" href="polyspace.md"><h3>📋 PolySpace & SonarQube</h3><p>Static Analysis & Compliance</p></a>
    <a class="card" href="tools.md"><h3>🛠 Tools & Scripting</h3><p>MATLAB | M-Scripting | Python | Git | VSCode</p></a>
    <a class="card" href="testing.md"><h3>✅ Testing & Safety</h3><p>Google Test | ISO-26262 | JAMA | JIRA</p></a>
    <a class="card" href="system.md"><h3>🔧 System Design & Integration</h3><p>Preevision | MagicDraw | Zonal Modules</p></a>
  </section>

  <footer>
    Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages
  </footer>

  <button class="back-to-top" onclick="scrollToTop()">↑</button>

  <script>
    function toggleTheme() {
      const html = document.documentElement;
      const current = html.getAttribute('data-theme');
      html.setAttribute('data-theme', current === 'dark' ? 'light' : 'dark');
    }

    const backToTop = document.querySelector('.back-to-top');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 300) {
        backToTop.classList.add('show');
      } else {
        backToTop.classList.remove('show');
      }
    });

    function scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }
  </script>
</body>
</html>
