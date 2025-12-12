---
layout: calculator
title: "Convertitore Chilometri Miglia  |  km ↔ mi  |  Online Gratis"
description: "Converti chilometri in miglia e miglia in km istantaneamente. Calcolatore gratuito con tabella di conversione rapida. Semplice e preciso."
category: "convertitori-unita"
subcategory: "lunghezza"
---

<!-- ADV SPOT 1: Banner top (Desktop: 728x90, Mobile: nascosto) -->
<div class="ad-container ad-top">
  <span class="ad-label">Pubblicità</span>
  <div class="ad-placeholder ad-leaderboard">
    <span class="ad-text">Banner 728×90</span>
  </div>
</div>

<div class="calculator-wrapper">
  <div class="calculator-icon">🚗</div>
  
  <h1 class="calculator-title">Convertitore Chilometri Miglia</h1>
  <p class="calculator-subtitle">Converti velocemente tra km e miglia in entrambe le direzioni</p>
  
  <div class="calculator-box">
    <div class="converter-tabs">
      <button class="tab-btn active" onclick="switchTab('km-to-mi')">
        <span class="tab-label">Chilometri → Miglia</span>
      </button>
      <button class="tab-btn" onclick="switchTab('mi-to-km')">
        <span class="tab-label">Miglia → Chilometri</span>
      </button>
    </div>
    
    <div id="km-to-mi" class="converter-panel active">
      <div class="input-wrapper">
        <label for="km-input">Chilometri (km)</label>
        <input type="number" id="km-input" placeholder="Inserisci valore" step="0.01" min="0">
      </div>
      
      <button class="calc-button" onclick="convertKmToMi()">
        <span class="button-icon">⚡</span>
        Converti in Miglia
      </button>
      
      <div id="km-result" class="result-box"></div>
    </div>
    
    <div id="mi-to-km" class="converter-panel">
      <div class="input-wrapper">
        <label for="mi-input">Miglia (mi)</label>
        <input type="number" id="mi-input" placeholder="Inserisci valore" step="0.01" min="0">
      </div>
      
      <button class="calc-button" onclick="convertMiToKm()">
        <span class="button-icon">⚡</span>
        Converti in Chilometri
      </button>
      
      <div id="mi-result" class="result-box"></div>
    </div>
  </div>
</div>

<!-- ADV SPOT 2: Banner principale sotto calculator (336x280) -->
<div class="ad-container ad-primary">
  <span class="ad-label">Pubblicità</span>
  <div class="ad-placeholder ad-rectangle">
    <span class="ad-text">Banner 336×280</span>
  </div>
</div>

<script>
function switchTab(direction) {
  const kmPanel = document.getElementById('km-to-mi');
  const miPanel = document.getElementById('mi-to-km');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (direction === 'km-to-mi') {
    kmPanel.classList.add('active');
    miPanel.classList.remove('active');
    buttons[0].classList.add('active');
    buttons[1].classList.remove('active');
  } else {
    miPanel.classList.add('active');
    kmPanel.classList.remove('active');
    buttons[1].classList.add('active');
    buttons[0].classList.remove('active');
  }
}

function convertKmToMi() {
  const km = parseFloat(document.getElementById('km-input').value);
  const resultDiv = document.getElementById('km-result');
  
  if (isNaN(km) || km < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const miles = km * 0.621371;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">${km.toFixed(2)} km = <strong>${miles.toFixed(2)} miglia</strong></div>
    </div>
  `;
}

function convertMiToKm() {
  const miles = parseFloat(document.getElementById('mi-input').value);
  const resultDiv = document.getElementById('mi-result');
  
  if (isNaN(miles) || miles < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const km = miles * 1.60934;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">${miles.toFixed(2)} mi = <strong>${km.toFixed(2)} chilometri</strong></div>
    </div>
  `;
}

window.addEventListener('load', function() {
  document.getElementById('km-input').value = '10';
  convertKmToMi();
});
</script>

<div class="content-section">
  <h2>Come usare il convertitore</h2>
  <p>Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.</p>

  <h3>Quando serve convertire km in miglia</h3>
  <p>La conversione tra chilometri e miglia è essenziale per viaggi internazionali, sport e comprensione di specifiche tecniche. Se stai pianificando un viaggio negli Stati Uniti o nel Regno Unito, dove le distanze sono espresse in miglia, dovrai convertire le distanze dal sistema metrico.</p>

  <h3>Formula di conversione</h3>
  <p><strong>Da chilometri a miglia:</strong> 1 km = 0.621371 miglia<br>
  <strong>Da miglia a chilometri:</strong> 1 miglio = 1.60934 km</p>
</div>

<div class="content-section">
  <h3>Tabella conversione rapida</h3>
  
  <div class="conversion-tables">
    <div class="conversion-table">
      <h4>Chilometri → Miglia</h4>
      <table>
        <tr><td>1 km</td><td>0.62 mi</td></tr>
        <tr><td>5 km</td><td>3.11 mi</td></tr>
        <tr><td>10 km</td><td>6.21 mi</td></tr>
        <tr><td>20 km</td><td>12.43 mi</td></tr>
        <tr><td>50 km</td><td>31.07 mi</td></tr>
        <tr><td>100 km</td><td>62.14 mi</td></tr>
      </table>
    </div>
    
    <div class="conversion-table">
      <h4>Miglia → Chilometri</h4>
      <table>
        <tr><td>1 mi</td><td>1.61 km</td></tr>
        <tr><td>5 mi</td><td>8.05 km</td></tr>
        <tr><td>10 mi</td><td>16.09 km</td></tr>
        <tr><td>20 mi</td><td>32.19 km</td></tr>
        <tr><td>50 mi</td><td>80.47 km</td></tr>
        <tr><td>100 mi</td><td>160.93 km</td></tr>
      </table>
    </div>
  </div>
</div>

<div class="related-tools">
  <h3>Convertitori correlati</h3>
  <div class="related-grid">
    <a href="/smart-converter-tools/calcolatori/convertitore-metri-piedi/" class="related-card">
      <span class="related-icon">📐</span>
      <span class="related-title">Metri ↔ Piedi</span>
    </a>
    <a href="/smart-converter-tools/calcolatori/convertitore-centimetri-pollici/" class="related-card">
      <span class="related-icon">📱</span>
      <span class="related-title">Centimetri ↔ Pollici</span>
    </a>
    <a href="/smart-converter-tools/calcolatori/convertitore-chilogrammi-libbre/" class="related-card">
      <span class="related-icon">⚖️</span>
      <span class="related-title">Kg ↔ Libbre</span>
    </a>
    <a href="/smart-converter-tools/calcolatori/convertitore-grammi-once/" class="related-card">
      <span class="related-icon">🍳</span>
      <span class="related-title">Grammi ↔ Once</span>
    </a>
  </div>
</div>

<style>
:root {
  --primary-purple: #667eea;
  --primary-purple-dark: #764ba2;
  --accent-green: #10b981;
  --gray-50: #f7fafc;
  --gray-100: #edf2f7;
  --gray-200: #e2e8f0;
  --gray-300: #cbd5e0;
  --gray-400: #a0aec0;
  --gray-600: #4a5568;
  --gray-700: #2d3748;
  --gray-800: #1a202c;
}

.calculator-wrapper {
  max-width: 600px;
  margin: 0 auto 2rem auto;
}

.calculator-icon {
  font-size: 3rem;
  text-align: center;
  margin-bottom: 1rem;
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.1));
}

.calculator-title {
  color: var(--gray-800);
  font-size: 1.75rem;
  font-weight: 700;
  text-align: center;
  margin-bottom: 0.5rem;
  line-height: 1.3;
}

.calculator-subtitle {
  color: var(--gray-600);
  font-size: 1rem;
  text-align: center;
  margin-bottom: 1.5rem;
  line-height: 1.5;
}

.calculator-box {
  background: white;
  border: 2px solid var(--gray-200);
  border-radius: 16px;
  padding: 1.5rem;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
}

.converter-tabs {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.tab-btn {
  background: var(--gray-50);
  border: 2px solid var(--gray-200);
  border-radius: 10px;
  padding: 0.75rem;
  cursor: pointer;
  font-family: 'Montserrat', sans-serif;
  font-size: 0.9rem;
  font-weight: 600;
  color: var(--gray-600);
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.tab-btn::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: linear-gradient(90deg, var(--primary-purple), var(--accent-green));
  transform: scaleX(0);
  transition: transform 0.3s ease;
}

.tab-btn.active::before {
  transform: scaleX(1);
}

.tab-btn.active {
  background: white;
  border-color: var(--primary-purple);
  color: var(--primary-purple);
}

.tab-label {
  display: block;
  text-align: center;
}

.converter-panel {
  display: none;
}

.converter-panel.active {
  display: block;
}

.input-wrapper {
  margin-bottom: 1rem;
}

.input-wrapper label {
  display: block;
  color: var(--gray-700);
  font-size: 0.9rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
  text-align: center;
}

.input-wrapper input {
  width: 100%;
  padding: 1rem;
  font-size: 1.1rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: 500;
  text-align: center;
  border: 2px solid var(--gray-200);
  border-radius: 10px;
  background: var(--gray-50);
  color: var(--gray-800);
  transition: all 0.3s ease;
  min-height: 52px;
}

.input-wrapper input:focus {
  outline: none;
  border-color: var(--primary-purple);
  background: white;
  box-shadow: 0 0 0 4px rgba(102, 126, 234, 0.1);
}

.input-wrapper input::placeholder {
  color: var(--gray-400);
}

.calc-button {
  width: 100%;
  padding: 1.1rem;
  font-size: 1.05rem;
  font-weight: 700;
  font-family: 'Montserrat', sans-serif;
  color: white;
  background: linear-gradient(135deg, var(--primary-purple) 0%, var(--primary-purple-dark) 100%);
  border: none;
  border-radius: 10px;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 12px rgba(102, 126, 234, 0.3);
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  margin-bottom: 1rem;
  min-height: 56px;
}

.calc-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(102, 126, 234, 0.4);
}

.calc-button:active {
  transform: translateY(0);
}

.button-icon {
  font-size: 1.2rem;
}

.result-box {
  min-height: 60px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.result-success {
  background: linear-gradient(135deg, #ecfdf5 0%, #d1fae5 100%);
  border: 2px solid var(--accent-green);
  border-radius: 10px;
  padding: 1rem;
  text-align: center;
  animation: slideIn 0.3s ease;
}

.result-main {
  color: var(--gray-800);
  font-size: 1.1rem;
  line-height: 1.4;
}

.result-main strong {
  color: var(--accent-green);
  font-weight: 700;
}

.error-message {
  background: #fef2f2;
  border: 2px solid #fca5a5;
  border-radius: 10px;
  padding: 1rem;
  color: #991b1b;
  text-align: center;
  font-weight: 600;
}

@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.content-section {
  margin: 2rem 0;
  line-height: 1.7;
}

.content-section h2 {
  color: var(--gray-800);
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 3px solid var(--primary-purple);
  display: inline-block;
}

.content-section h3 {
  color: var(--gray-700);
  font-size: 1.2rem;
  font-weight: 600;
  margin: 1.5rem 0 0.75rem 0;
}

.content-section p {
  color: var(--gray-600);
  margin-bottom: 1rem;
}

.conversion-tables {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin: 1.5rem 0;
}

.conversion-table {
  background: var(--gray-50);
  border-radius: 12px;
  padding: 1.25rem;
  border: 1px solid var(--gray-200);
}

.conversion-table h4 {
  color: var(--gray-700);
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 1rem;
  text-align: center;
}

.conversion-table table {
  width: 100%;
  border-collapse: collapse;
}

.conversion-table td {
  padding: 0.6rem;
  border-bottom: 1px solid var(--gray-200);
  font-size: 0.95rem;
}

.conversion-table td:first-child {
  color: var(--gray-700);
  font-weight: 600;
}

.conversion-table td:last-child {
  color: var(--primary-purple);
  font-weight: 600;
  text-align: right;
}

.conversion-table tr:last-child td {
  border-bottom: none;
}

.related-tools {
  margin: 2.5rem 0;
}

.related-tools h3 {
  color: var(--gray-800);
  font-size: 1.3rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.related-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
}

.related-card {
  background: white;
  border: 2px solid var(--gray-200);
  border-radius: 12px;
  padding: 1rem;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 0.75rem;
  transition: all 0.3s ease;
}

.related-card:hover {
  border-color: var(--primary-purple);
  transform: translateY(-2px);
  box-shadow: 0 8px 16px rgba(102, 126, 234, 0.15);
}

.related-icon {
  font-size: 1.8rem;
  flex-shrink: 0;
}

.related-title {
  color: var(--gray-700);
  font-weight: 600;
  font-size: 0.95rem;
}

.ad-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 2rem auto;
  max-width: 100%;
}

.ad-top {
  margin: 1rem auto 2rem auto;
}

.ad-primary {
  margin: 2.5rem auto;
}

.ad-label {
  font-size: 0.65rem;
  color: var(--gray-400);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-bottom: 0.5rem;
  font-weight: 600;
}

.ad-placeholder {
  background: linear-gradient(135deg, var(--gray-50) 0%, var(--gray-100) 100%);
  border: 2px dashed var(--gray-300);
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.ad-leaderboard {
  width: 728px;
  height: 90px;
  max-width: 100%;
}

.ad-rectangle {
  width: 336px;
  height: 280px;
  max-width: 100%;
}

.ad-text {
  color: var(--gray-400);
  font-size: 0.85rem;
  font-weight: 500;
}

@media (max-width: 768px) {
  .calculator-icon {
    font-size: 2.5rem;
  }
  
  .calculator-title {
    font-size: 1.5rem;
  }
  
  .calculator-subtitle {
    font-size: 0.95rem;
  }
  
  .calculator-box {
    padding: 1.25rem;
  }
  
  .tab-btn {
    font-size: 0.85rem;
    padding: 0.65rem;
  }
  
  .ad-top {
    display: none;
  }
  
  .conversion-tables {
    grid-template-columns: 1fr;
  }
  
  .related-grid {
    grid-template-columns: 1fr;
  }
}
</style>
