<style>
:root {
  --bg-dark: #0f0f1a;
  --card-dark: #1e1e2f;
  --text-dark: #f8f8ff;
  --accent-pink: #ff5ebc;
  --accent-yellow: #fcd34d;
  --accent-red: #ff6b6b;
  --card-hover: #2a2a40;
}

[data-md-color-scheme="slate"] {
  --md-primary-fg-color: var(--accent-pink);
  --md-accent-fg-color: var(--accent-yellow);
}

body {
  background-color: var(--bg-dark);
  color: var(--text-dark);
}

h1 {
  color: var(--accent-pink);
  text-align: center;
  margin-top: 2rem;
  font-size: 2.5rem;
}

.intro {
  text-align: center;
  font-size: 1.2rem;
  margin-bottom: 2rem;
  color: var(--text-dark);
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
  padding: 2rem;
}

.card {
  background-color: var(--card-dark);
  border: 1px solid var(--accent-pink);
  border-radius: 12px;
  padding: 1.5rem;
  text-decoration: none;
  color: var(--text-dark);
  transition: transform 0.3s ease, background 0.3s ease;
  font-family: 'Segoe UI', sans-serif;
}

.card:hover {
  background-color: var(--card-hover);
  transform: translateY(-5px);
  border-color: var(--accent-yellow);
}

.card h2 {
  margin-top: 0;
  color: var(--accent-pink);
  font-size: 1.3rem;
}

.card p {
  font-size: 0.95rem;
  line-height: 1.4;
}
</style>

# 🚗 AutoDev Vault

<div class="intro">
  A comprehensive technical vault for Automotive engineers.<br>
  Dive into Model-Based Dev, Simulink, Coding, Testing & more!
</div>

 <footer>
    Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages
  </footer>

<div class="grid">

<a href="Model_Based_Development_QnA/mbd/" class="card">
  <h2>🧠 Model-Based Development</h2>
  <p>Simulink | Stateflow | TLC | MIL | SIL | Integration</p>
</a>

<a href="Code_Based_Development_QnA/cbd/" class="card">
  <h2>💻 Code-Based Development</h2>
  <p>Embedded C | MISRA | Unit Testing | Coding Guidelines</p>
</a>

<a href="Simulink_QnA/simulink/" class="card">
  <h2>📊 Simulink</h2>
  <p>Modeling | Sample times | Solver Configs | Masking</p>
</a>

<a href="Stateflow_QnA/stateflow/" class="card">
  <h2>🔄 Stateflow</h2>
  <p>States | Events | Transitions | Temporal Logic</p>
</a>

<a href="AUTOSAR_QnA/autsar/" class="card">
  <h2>⚙️ AUTOSAR & RTE</h2>
  <p>SWCs | Ports | RTE | ComStack | Interfaces</p>
</a>

<a href="Polyspace_QnA/polyspace/" class="card">
  <h2>🧪 Polyspace & SonarQube</h2>
  <p>Static Analysis | Runtime Errors | MISRA Violations</p>
</a>

<a href="Tools_Scripting_QnA/tools/" class="card">
  <h2>🛠️ Tools & Scripting</h2>
  <p>MATLAB | Python | Git | VSCode | Automation</p>
</a>

<a href="Testing_Safety_QnA/testing/" class="card">
  <h2>✅ Testing & Safety</h2>
  <p>GoogleTest | ISO 26262 | JIRA | Safety Standards</p>
</a>

<a href="System_Design_QnA/system/" class="card">
  <h2>🔧 System Design & Integration</h2>
  <p>Prevision | Zonal Architecture | MagicDraw</p>
</a>

</div>
