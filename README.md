<div class="space">
  <div class="sun">☀️</div>
  <div class="orbit orbit1"><div class="planet" title="HTML">🌐</div></div>
  <div class="orbit orbit2"><div class="planet" title="CSS">🎨</div></div>
  <div class="orbit orbit3"><div class="planet" title="JS">⚡</div></div>
  <div class="orbit orbit4"><div class="planet" title="React">⚛️</div></div>
  <div class="orbit orbit5"><div class="planet" title="Java">☕</div></div>
  <div class="orbit orbit6"><div class="planet" title="Git">🐙</div></div>
</div>

<style>
.space {
  position: relative;
  width: 400px;
  height: 400px;
  margin: auto;
  background: radial-gradient(circle, #000010, #000022);
  border-radius: 50%;
  overflow: hidden;
}

.sun {
  position: absolute;
  top: 50%;
  left: 50%;
  font-size: 40px;
  transform: translate(-50%, -50%);
}

.orbit {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 100%;
  height: 100%;
  transform-origin: center;
  animation: rotate linear infinite;
}

.orbit1 { animation-duration: 10s; }
.orbit2 { animation-duration: 15s; }
.orbit3 { animation-duration: 20s; }
.orbit4 { animation-duration: 25s; }
.orbit5 { animation-duration: 30s; }
.orbit6 { animation-duration: 35s; }

.planet {
  position: absolute;
  top: 0;
  left: 50%;
  font-size: 25px;
  transform: translateX(-50%);
  transition: transform 0.3s, scale 0.3s;
}

.planet:hover {
  transform: translateX(-50%) scale(1.5);
  filter: drop-shadow(0 0 10px #fff);
}

@keyframes rotate {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}
</style>
