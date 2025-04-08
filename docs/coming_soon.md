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
  <div class="coming-soon-subtitle">We're working on something amazing.<br>Check back again very soon!</div>
</div>
