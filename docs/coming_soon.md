<style>
.coming-soon-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 80px 20px;
  text-align: center;
  font-family: 'Segoe UI', sans-serif;
  animation: fadeIn 2s ease-in;
}

.coming-soon-title {
  font-size: 3rem;
  color: #ff4081;
  margin-bottom: 1rem;
}

.coming-soon-subtitle {
  font-size: 1.3rem;
  color: #666;
  margin-bottom: 2rem;
}

.loader {
  width: 80px;
  height: 80px;
  border: 8px solid #f3f3f3;
  border-top: 8px solid #ff4081;
  border-radius: 50%;
  animation: spin 1.2s linear infinite;
  margin-bottom: 1rem;
}

.upcoming-concepts {
  text-align: left;
  max-width: 500px;
  margin-top: 40px;
  font-size: 1.1rem;
  color: #333;
}

.upcoming-concepts ul {
  list-style-type: "📌 ";
  padding-left: 20px;
}

@keyframes spin {
  to { transform: rotate(360deg); }
}

@keyframes fadeIn {
  from { opacity: 0; }
  to   { opacity: 1; }
}
</style>

<div class="coming-soon-container">
  <div class="loader"></div>
  <div class="coming-soon-title">🚧 Coming Soon</div>
  <div class="coming-soon-subtitle">
    We're working on something amazing.<br>Check back again very soon!
  </div>

  <div class="upcoming-concepts">
    <strong>📚 Upcoming Concepts:</strong>
    <ul>
      <li>QT</li>
      <li>Bluetooth</li>
      <li>RTOS (Real-Time Operating Systems)</li>
      <li>PCB Design</li>
      <li>Hardware Interfaces</li>
      <li>Validation & Testing</li>
      <li>WiFi Integration</li>
      <li>Linux Kernel</li>
      <li>TCP/IP Networking</li>
      <li>OpenWRT</li>
      <li>Verification & Validation Engineer Role</li>
      <li>OEM, Tier 1 & Tier 2 Suppliers</li>
      <li>Vehicle Manufacturing Layers</li>
      <li>Firmware Development</li>
      <li>Test Automation</li>
      <li>Python in Automotive</li>
      <li>Powertrain Control</li>
      <li>Battery Management Systems (BMS)</li>
      <li>HMI & Infotainment Systems</li>
      <li>CAN Bus Communication</li>
      <li>ASPICE Process Model</li>
      <li>TargetLink</li>
    </ul>
  </div>
</div>
