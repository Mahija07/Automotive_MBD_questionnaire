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

# 🚗 AutoDev Vault by Mahija

<div class="intro">
  A comprehensive technical vault for Automotive engineers.<br>
  Dive into Model-Based Dev, Simulink, Coding, Testing & more!
</div>

<div class="card-grid">

  <!-- Model-Based Development -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>🧠 Model-Based Development</h2>
        <p>Simulink | Stateflow | TLC | MIL | SIL</p>
      </div>
      <div class="card-back">
        <h3>Explore Subtopics</h3>
        <ul class="sub-links">
          <li><a href="Model_Based_Development_QnA/mbd/">Overview</a></li>
          <li><a href="Model_Based_Development_QnA/simulink_QnA/simulink/">Simulink</a></li>
          <li><a href="Model_Based_Development_QnA/stateflow_QnA/stateflow/">Stateflow</a></li>
          <li><a href="Model_Based_Development_QnA/TLC_QnA/TLC/">TLC</a></li>
          <li><a href="Model_Based_Development_QnA/MIL_QnA/MIL/">MIL</a></li>
          <li><a href="Model_Based_Development_QnA/SIL_QnA/SIL/">SIL</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Code-Based Development -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>💻 Code-Based Development</h2>
        <p>Embedded C | MISRA | Unit Testing | Coding Guidelines</p>
      </div>
      <div class="card-back">
        <h3>Explore Subtopics</h3>
        <ul class="sub-links">
          <li><a href="Code_Based_Development_QnA/cbd/">All Topics</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- AUTOSAR -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>⚙️ AUTOSAR & RTE</h2>
        <p>SWCs | Ports | RTE | ComStack | Interfaces</p>
      </div>
      <div class="card-back">
        <h3>Explore Subtopics</h3>
        <ul class="sub-links">
          <li><a href="AUTOSAR_QnA/autsar/">All Topics</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Software Quality -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>🧪 Software Quality & Safety</h2>
        <p>POLYSPACE | SONARQUBE | MISRA C | ISO-26262</p>
      </div>
      <div class="card-back">
        <h3>Explore Subtopics</h3>
        <ul class="sub-links">
          <li><a href="Polyspace_QnA/polyspace/">Polyspace</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Tools & Scripting -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>🛠️ Tools & Scripting</h2>
        <p>MATLAB | Python | Git | VSCode | Automation</p>
      </div>
      <div class="card-back">
        <h3>Coming Soon</h3>
        <ul class="sub-links">
          <li><a href="coming_soon/">Preview Tools</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Testing & Safety -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>✅ Testing & Safety</h2>
        <p>GoogleTest | ISO 26262 | JIRA | Safety Standards</p>
      </div>
      <div class="card-back">
        <h3>Coming Soon</h3>
        <ul class="sub-links">
          <li><a href="coming_soon_test/">Preview Topics</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- System Design & Integration -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>🔧 System Design & Integration</h2>
        <p>Prevision | Zonal Architecture | MagicDraw</p>
      </div>
      <div class="card-back">
        <h3>Coming Soon</h3>
        <ul class="sub-links">
          <li><a href="coming_soon_sys/">Preview Topics</a></li>
        </ul>
      </div>
    </div>
  </div>

</div>


 <footer>
    Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages
  </footer>
