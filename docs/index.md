<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AutoDev Vault</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono&family=Poppins:wght@600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-dark: #0f172a;
      --card-dark: #1e293b;
      --text-dark: #e2e8f0;
      --accent-dark: #38bdf8;
    }

    html[data-theme="dark"] {
      --bg: var(--bg-dark);
      --card: var(--card-dark);
      --text: var(--text-dark);
      --accent: var(--accent-dark);
    }

    body {
      margin: 0;
      font-family: 'Roboto Mono', monospace;
      background-color: var(--bg);
      color: var(--text);
    }

    header {
      background-color: var(--card);
      padding: 2rem;
      text-align: center;
      border-bottom: 2px solid var(--accent);
    }

    header h1 {
      font-family: 'Poppins', sans-serif;
      font-size: 3rem;
      color: var(--accent);
      margin: 0;
    }

    header p {
      font-size: 1.1rem;
      margin-top: 0.5rem;
      max-width: 800px;
      margin-left: auto;
      margin-right: auto;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2rem;
      padding: 2rem;
      max-width: 1200px;
      margin: auto;
    }

    .card {
      background-color: var(--card);
      border-left: 4px solid var(--accent);
      border-radius: 10px;
      padding: 1.5rem;
      text-decoration: none;
      color: inherit;
      transition: all 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
      background-color: #273549;
    }

    .card h2 {
      font-size: 1.3rem;
      color: var(--accent);
      margin-bottom: 0.5rem;
    }

    .card p {
      font-size: 0.95rem;
      color: var(--text);
    }

    footer {
      text-align: center;
      padding: 2rem 1rem;
      font-size: 0.85rem;
      color: #888;
    }
  </style>
</head>
<body>

  <header>
    <h1>🚗 AutoDev Vault</h1>
    <p>Interview Q&A vault for Automotive Software Engineers. Master topics in MBD, Simulink, Stateflow, Code Gen, Testing, Safety, and more.</p>
  </header>

  <main class="grid">
    <a class="card" href="mbd.md">
      <h2>⚙️ Model-Based Development</h2>
      <p>Simulink | Stateflow | TLC | MIL | SIL | Integration</p>
    </a>
    <a class="card" href="cbd.md">
      <h2>💻 Code-Based Development</h2>
      <p>C, Embedded C, MISRA, coding guidelines and best practices</p>
    </a>
    <a class="card" href="simulink.md">
      <h2>📊 Simulink</h2>
      <p>Modeling techniques, solver configs, subsystems, sample times</p>
    </a>
    <a class="card" href="stateflow.md">
      <h2>🔁 Stateflow</h2>
      <p>State machines, transitions, temporal logic, junctions</p>
    </a>
    <a class="card" href="autsar.md">
      <h2>🧩 AUTOSAR & RTE</h2>
      <p>SWCs, RTE, ports, interfaces, ComStack, BSWs</p>
    </a>
    <a class="card" href="polyspace.md">
      <h2>📋 Polyspace & SonarQube</h2>
      <p>Static analysis, code verification, runtime error checks</p>
    </a>
    <a class="card" href="tools.md">
      <h2>🛠 Tools & Scripting</h2>
      <p>MATLAB, Python, Git, Bash, VSCode, automation scripting</p>
    </a>
    <a class="card" href="testing.md">
      <h2>✅ Testing & Safety</h2>
      <p>ISO 26262, Google Test, JAMA, JIRA, functional safety</p>
    </a>
    <a class="card" href="system.md">
      <h2>🔧 System Design</h2>
      <p>Preevision, MagicDraw, Zonal Architecture, Integration</p>
    </a>
  </main>

  <footer>
    © 2025 AutoDev Vault · Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages
  </footer>

</body>
</html>
