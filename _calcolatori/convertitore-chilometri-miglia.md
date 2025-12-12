---
layout: calculator
title: "Convertitore Chilometri Miglia | km ↔ mi | Online Gratis"
description: "Converti chilometri in miglia e miglia in km istantaneamente. Calcolatore gratuito con tabella di conversione rapida."
category: "convertitori-unita"
subcategory: "lunghezza"
---

<div class="page-hero">
  <h1>🚗 Convertitore Chilometri Miglia</h1>
  <p>Converti velocemente tra km e miglia</p>
</div>

<!-- ADV SPOT 1: Banner principale above fold -->
<div class="ad-container ad-primary">
  <div class="ad-placeholder ad-main">
    <span class="ad-text">Banner 728×90</span>
  </div>
</div>

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
      <span class="button-icon">⚡</span>Converti in Miglia
    </button>
    <div id="km-result" class="result-box"></div>
  </div>
  
  <div id="mi-to-km" class="converter-panel">
    <div class="input-wrapper">
      <label for="mi-input">Miglia (mi)</label>
      <input type="number" id="mi-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertMiToKm()">
      <span class="button-icon">⚡</span>Converti in Chilometri
    </button>
    <div id="mi-result" class="result-box"></div>
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
  const kmPanel = document.getElementById('km-to-mi');
  const miPanel = document.getElementById('mi-to-km');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (tabId === 'km-to-mi') {
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
      <div class="result-main">
        ${km.toFixed(2)} km = <strong>${miles.toFixed(2)} miglia</strong>
      </div>
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
      <div class="result-main">
        ${miles.toFixed(2)} mi = <strong>${km.toFixed(2)} chilometri</strong>
      </div>
    </div>
  `;
}

window.addEventListener('load', function() {
  document.getElementById('km-input').value = '10';
  convertKmToMi();
});
</script>

<div class="content-section">
<h2>Come usare il convertitore chilometri miglia</h2>
<p>Questo strumento ti permette di convertire facilmente tra chilometri e miglia in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.</p>

<h3>Quando serve convertire km in miglia</h3>
<p>La conversione tra chilometri e miglia è essenziale in molte situazioni quotidiane. Se stai pianificando un viaggio negli Stati Uniti o nel Regno Unito, dove le distanze sono espresse in miglia, dovrai convertire le distanze dal sistema metrico. Anche per comprendere i limiti di velocità, le distanze su cartelli stradali o le specifiche di veicoli importati, questa conversione risulta fondamentale.</p>

<p>Gli sportivi che seguono programmi di allenamento internazionali spesso devono convertire distanze di corsa o ciclismo. Allo stesso modo, chi segue mappe e indicazioni stradali di paesi che usano il sistema imperiale necessita di questa conversione per pianificare correttamente i propri spostamenti.</p>

<h3>Formula di conversione</h3>
<p><strong>Da chilometri a miglia:</strong> 1 km = 0.621371 miglia<br>
<strong>Da miglia a chilometri:</strong> 1 miglio = 1.60934 km</p>

<p>Queste formule derivano dal fatto che un miglio internazionale è definito esattamente come 1,609.344 metri, mentre un chilometro equivale a 1,000 metri. La conversione è quindi una proporzione fissa e non cambia nel tempo.</p>

<h3>Tabella conversione rapida km - miglia</h3>
<div class="conversion-table">
<table>
<tr><th>Chilometri</th><th>Miglia</th><th></th><th>Miglia</th><th>Chilometri</th></tr>
<tr><td>1 km</td><td>0.62 mi</td><td></td><td>1 mi</td><td>1.61 km</td></tr>
<tr><td>5 km</td><td>3.11 mi</td><td></td><td>5 mi</td><td>8.05 km</td></tr>
<tr><td>10 km</td><td>6.21 mi</td><td></td><td>10 mi</td><td>16.09 km</td></tr>
<tr><td>20 km</td><td>12.43 mi</td><td></td><td>20 mi</td><td>32.19 km</td></tr>
<tr><td>50 km</td><td>31.07 mi</td><td></td><td>50 mi</td><td>80.47 km</td></tr>
<tr><td>100 km</td><td>62.14 mi</td><td></td><td>100 mi</td><td>160.93 km</td></tr>
<tr><td>200 km</td><td>124.27 mi</td><td></td><td>200 mi</td><td>321.87 km</td></tr>
</table>
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
  <span class="related-title">Cm ↔ Pollici</span>
</a>
<a href="/smart-converter-tools/calcolatori/convertitore-chilogrammi-libbre/" class="related-card">
  <span class="related-icon">⚖️</span>
  <span class="related-title">Kg ↔ Libbre</span>
</a>
</div>
</div>
