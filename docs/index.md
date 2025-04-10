# 📚 AutoDev Vault 

<!-- index.md - Fully redesigned layout -->
<style>
  :root {
    --bg-dark: #0f0f1a;
    --card-dark: #1e1e2f;
    --text-light: #f8f8ff;
    --accent-pink: #ff5ebc;
    --accent-yellow: #fcd34d;
    --accent-red: #ff6b6b;
    --card-hover: #2a2a40;
  }

  body {
    background-color: var(--bg-dark);
    color: var(--text-light);
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
  }

  .header {
    text-align: center;
    padding: 2rem 1rem 1rem;
  }

  .header h1 {
    font-size: 2.8rem;
    color: var(--accent-pink);
    margin: 0;
  }

  .intro {
    text-align: center;
    font-size: 1.2rem;
    margin: 0.5rem auto 2rem;
    color: var(--text-light);
  }

  .card-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(280px, 1fr));
    gap: 2rem;
    padding: 2rem;
    max-width: 1200px;
    margin: auto;
  }

  .card-flip {
    perspective: 1200px;
    width: 100%;
    height: 260px;
  }

  .card-inner {
    position: relative;
    width: 100%;
    height: 110%;
    transition: transform 0.8s;
    transform-style: preserve-3d;
  }

  .card-flip:hover .card-inner {
    transform: rotateY(180deg);
  }

  .card-front, .card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    padding: 1.5rem;
    background-color: var(--card-dark);
    border: 1px solid var(--accent-pink);
    border-radius: 1rem;
    backface-visibility: hidden;
    display: flex;
    flex-direction: column;
    justify-content: center;
    box-sizing: border-box;
  }

  .card-back {
    transform: rotateY(180deg);
  }

  .card-front h2, .card-back h3 {
    color: var(--accent-pink);
    margin-bottom: 1rem;
    font-size: 1.2rem;
  }

  .card-front p, .card-back ul {
    font-size: 0.8rem;
    color: var(--text-light);
    line-height: 1.4;
  }

  .card-back ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .card-back ul li {
    margin-bottom: 0.3rem;
  }

  .card-back ul li a {
    color: var(--accent-yellow);
    text-decoration: none;
    font-weight: 500;
  }

  .card-back ul li a:hover {
    color: var(--accent-red);
    text-decoration: underline;
  }

  footer {
    text-align: center;
    padding: 2rem 1rem;
    color: #aaa;
    font-size: 0.9rem;
    border-top: 1px solid #333;
    margin-top: 3rem;
  }
</style>

<div class="car-dance">
  <span class="car car1">🚗</span>
  <span class="car car2">🚙</span>
  <span class="car car3">🏎️</span>
  <span class="car car4">🚘</span>
  <span class="car car5">🚕</span>
  <span class="car car6">🚓</span>
  <span class="car car7">🛻</span>
  <span class="car car8">🚐</span>
  <span class="car car9">🚔</span>
  <span class="car car10">🚖</span>
  <span class="car car11">🚍</span>
  <span class="car car12">🚛</span>
  <span class="car car13">🚜</span>
  <span class="car car14">🚚</span>
  <span class="car car15">🚎</span>
</div>


<div class="header">
  <div class="intro">
    A curated space for Automotive Engineers to explore MBD, Simulink, AUTOSAR, Testing & more.
  </div>
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
        <h4>Explore Subtopics</h4>
        <ul>
          <li><a href="Model_Based_Development_QnA/mbd/">📚 Overview</a></li>
          <li><a href="Model_Based_Development_QnA/Simulink_QnA/simulink/">📚 Simulink</a></li>
          <li><a href="Model_Based_Development_QnA/Stateflow_QnA/stateflow/">📚 Stateflow</a></li>
          <li><a href="Model_Based_Development_QnA/TLC_QnA/TLC/">📚 TLC</a></li>
          <li><a href="Model_Based_Development_QnA/MIL_QnA/MIL/">📚 MIL</a></li>
          <li><a href="Model_Based_Development_QnA/SIL_QnA/SIL/">📚 SIL</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- AUTOSAR & RTE -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>⚙️ AUTOSAR & RTE</h2>
        <p> | Ports | RTE | ComStack | Interfaces</p>
      </div>
      <div class="card-back">
        <h4>Explore Subtopics</h4>
        <ul>
          <li><a href="AUTOSAR_QnA/Autosar/">📚 Overview</a></li>
          <li><a href="AUTOSAR_QnA/swc/">📚 SWC's</a></li>
          <li><a href="AUTOSAR_QnA/rte/">📚 RTE</a></li>
          <li><a href="AUTOSAR_QnA/comstack/">📚 ComStack</a></li>
          <li><a href="AUTOSAR_QnA/interfaces/">📚 Interfaces</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Code-Based Development -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>💻 Code-Based Development</h2>
        <p>Embedded C </p>
      </div>
      <div class="card-back">
        <h4>Explore Subtopics</h4>
        <ul>
          <li><a href="Code_Based_Development_QnA/cbd/">📚 Overview</a></li>
          <li><a href="Code_Based_Development_QnA/embeddedc/">📚 Embedded C</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Software Quality -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>🧪 Software Quality & Safety</h2>
        <p>Polyspace | SonarQube | MISRA C | ISO 26262</p>
      </div>
      <div class="card-back">
        <h4>Explore Subtopics</h4>
        <ul>
          <li><a href="Polyspace_QnA/sqss/">📚 Overview</a></li>
          <li><a href="Polyspace_QnA/polyspace/">📚 Polyspace</a></li>
          <li><a href="Polyspace_QnA/sonarqube/">📚 SonarQube</a></li>
          <li><a href="Polyspace_QnA/Standards/MISRA_C_Guidelines/">📚 MISRA C</a></li>
          <li><a href="Polyspace_QnA/Standards/ISO-26262/">📚 ISO 26262</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- Tools & Scripting -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>🛠️ Tools & Scripting</h2>
        <p>MATLAB | M-Scripting | Git | VSCode </p>
      </div>
      <div class="card-back">
        <h4>Explore Subtopics</h4>
        <ul>
          <li><a href="Tools_Scripting_QnA/tools/">📚 Overview</a></li>
          <li><a href="Tools_Scripting_QnA/matlab/">📚 MATLAB</a></li>
          <li><a href="Tools_Scripting_QnA/mscripting/">📚 M-Scripting</a></li>
          <li><a href="Tools_Scripting_QnA/git/">📚 Git</a></li>
          <li><a href="Tools_Scripting_QnA/vscode/">📚 VS Code</a></li>
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
        <h4>Explore Subtopics</h4>
        <ul>
          <li><a href="Testing_Safety_QnA/testing/">📚 Overview</a></li>
          <li><a href="Testing_Safety_QnA/gtest/">📚 GoogleTest</a></li>
          <li><a href="Testing_Safety_QnA/jira/">📚 JIRA</a></li>
          <li><a href="Testing_Safety_QnA/safety_standards/">📚 Safety Standards</a></li>
        </ul>
      </div>
    </div>
  </div>

  <!-- System Design -->
  <div class="card-flip">
    <div class="card-inner">
      <div class="card-front">
        <h2>🔧 System Design & Integration</h2>
        <p>Prevision | Zonal Architecture | MagicDraw</p>
      </div>
      <div class="card-back">
        <h4>Explore Subtopics</h4>
        <ul>
          <li><a href="System_Design_QnA/system/">📚 Overview</a></li>
          <li><a href="System_Design_QnA/magicdraw/magicdraw_qna/">📚 MagicDraw</a></li>
          <li><a href="System_Design_QnA/preevision/preevision_qna/">📚 Prevision</a></li>
          <li><a href="System_Design_QnA/zonal_architecture/zonal_architecture_qna/">📚 Zonal Architecture</a></li>
        </ul>
      </div>
    </div>
  </div>

</div>
<!-- we need to work on linux, communication protocols(can lin, ethernet, uds), different kind of features in a vehicle and how and why they are categorized in a diffrent different ways, how we consider different zonal modules and the whole process from what where when to how a vehicle works from user end to resource side, including services and actuators and if somehwere the microservices are that too and what is ECU extract and why it happens, software requirements and system requirements, types of coverage and what does it mean how to cover that in MIL and for GTest also, think for Q1, Q2 and Q3 level testing for a vehicle -->

<footer>
  <p>📬 Want to reach out? <a href="feedback/">Give Feedback or Contact Me</a></p>
  <p>Made with ❤️ by Mahija · Powered by MkDocs & GitHub Pages</p>
</footer>
