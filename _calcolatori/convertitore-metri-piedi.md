---
layout: calculator
title: "Convertitore Metri Piedi | m ↔ ft | Online Gratis"
description: "Converti metri in piedi e piedi in metri istantaneamente. Calcolatore gratuito con tabella di conversione rapida."
category: "convertitori-unita"
subcategory: "lunghezza"
emoji: "📐"
---

<div class="page-hero">
  <h1>📐 Convertitore Metri Piedi</h1>
  <p>Converti velocemente tra metri e piedi</p>
</div>

<!-- ADV SPOT 1: Banner principale above fold -->
<div class="ad-container ad-primary">
  <div class="ad-placeholder ad-main">
    <span class="ad-text">Banner 728×90</span>
  </div>
</div>

<div class="calculator-box">
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('m-to-ft')">
      <span class="tab-label">Metri → Piedi</span>
    </button>
    <button class="tab-btn" onclick="switchTab('ft-to-m')">
      <span class="tab-label">Piedi → Metri</span>
    </button>
  </div>
  
  <div id="m-to-ft" class="converter-panel active">
    <div class="input-wrapper">
      <label for="m-input">Metri (m)</label>
      <input type="number" id="m-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertMToFt()">
      <span class="button-icon">⚡</span>Converti in Piedi
    </button>
    <div id="m-result" class="result-box"></div>
  </div>
  
  <div id="ft-to-m" class="converter-panel">
    <div class="input-wrapper">
      <label for="ft-input">Piedi (ft)</label>
      <input type="number" id="ft-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertFtToM()">
      <span class="button-icon">⚡</span>Converti in Metri
    </button>
    <div id="ft-result" class="result-box"></div>
  </div>
</div>

<!-- ADV SPOT 2: Banner secondario dopo calculator -->
<div class="ad-container ad-secondary">
  <div class="ad-placeholder ad-second">
    <span class="ad-text">Banner 728×90</span>
  </div>
</div>

<script>
function switchTab(tabId) {
  const mPanel = document.getElementById('m-to-ft');
  const ftPanel = document.getElementById('ft-to-m');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (tabId === 'm-to-ft') {
    mPanel.classList.add('active');
    ftPanel.classList.remove('active');
    buttons[0].classList.add('active');
    buttons[1].classList.remove('active');
  } else {
    ftPanel.classList.add('active');
    mPanel.classList.remove('active');
    buttons[1].classList.add('active');
    buttons[0].classList.remove('active');
  }
}

function convertMToFt() {
  const meters = parseFloat(document.getElementById('m-input').value);
  const resultDiv = document.getElementById('m-result');
  
  if (isNaN(meters) || meters < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const feet = meters * 3.28084;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${meters.toFixed(2)} m = <strong>${feet.toFixed(2)} piedi</strong>
      </div>
    </div>
  `;
}

function convertFtToM() {
  const feet = parseFloat(document.getElementById('ft-input').value);
  const resultDiv = document.getElementById('ft-result');
  
  if (isNaN(feet) || feet < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const meters = feet * 0.3048;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${feet.toFixed(2)} ft = <strong>${meters.toFixed(2)} metri</strong>
      </div>
    </div>
  `;
}

window.addEventListener('load', function() {
  document.getElementById('m-input').value = '10';
  convertMToFt();
});
</script>

<div class="content-section">
<h2>Come usare il convertitore metri piedi</h2>
<p>Questo strumento ti permette di convertire facilmente tra metri e piedi in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.</p>

<h3>Quando serve convertire metri in piedi</h3>
<p>La conversione tra metri e piedi è essenziale per misurazioni di altezze, come quella degli edifici o delle montagne, quando si consultano fonti internazionali. Nel settore immobiliare, le dimensioni delle stanze sono spesso espresse in piedi nei paesi anglosassoni. Per l'altezza delle persone, molti paesi usano i piedi anziché i metri.</p>

<p>In aviazione, le altitudini sono sempre espresse in piedi, anche per voli che operano in paesi che usano il sistema metrico. Anche nel settore nautico e delle immersioni subacquee, le profondità vengono spesso misurate in piedi. Per progetti di costruzione e architettura con standard internazionali, la conversione tra metri e piedi è fondamentale.</p>

<h3>Formula di conversione</h3>
<p><strong>Da metri a piedi:</strong> 1 m = 3.28084 piedi<br>
<strong>Da piedi a metri:</strong> 1 piede = 0.3048 m</p>

<p>La conversione si basa sulla definizione internazionale che stabilisce 1 piede (foot) pari esattamente a 0.3048 metri. Questa definizione è stata stabilita nel 1959 come parte dell'accordo internazionale sui sistemi di misurazione, garantendo uniformità nelle conversioni in tutto il mondo.</p>

<h3>Tabella conversione rapida metri - piedi</h3>
<div class="conversion-table">
<table>
<tr><th>Metri</th><th>Piedi</th><th></th><th>Piedi</th><th>Metri</th></tr>
<tr><td>1 m</td><td>3.28 ft</td><td></td><td>1 ft</td><td>0.30 m</td></tr>
<tr><td>2 m</td><td>6.56 ft</td><td></td><td>5 ft</td><td>1.52 m</td></tr>
<tr><td>5 m</td><td>16.40 ft</td><td></td><td>10 ft</td><td>3.05 m</td></tr>
<tr><td>10 m</td><td>32.81 ft</td><td></td><td>20 ft</td><td>6.10 m</td></tr>
<tr><td>50 m</td><td>164.04 ft</td><td></td><td>50 ft</td><td>15.24 m</td></tr>
<tr><td>100 m</td><td>328.08 ft</td><td></td><td>100 ft</td><td>30.48 m</td></tr>
</table>
</div>
</div>
