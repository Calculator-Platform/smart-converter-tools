---
layout: calculator
title: "Convertitore Chilogrammi Libbre | kg ↔ lb | Online Gratis"
description: "Converti chilogrammi in libbre e libbre in kg istantaneamente. Calcolatore gratuito con tabella di conversione rapida."
category: "convertitori-unita"
subcategory: "peso"
---

<div class="page-hero">
  <h1>⚖️ Convertitore Chilogrammi Libbre</h1>
  <p>Converti velocemente tra kg e libbre</p>
</div>

<!-- ADV SPOT 1: Banner principale above fold -->
<div class="ad-container ad-primary">
  <div class="ad-placeholder ad-main">
    <span class="ad-text">Banner 728×90</span>
  </div>
</div>

<div class="calculator-box">
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('kg-to-lb')">
      <span class="tab-label">Chilogrammi → Libbre</span>
    </button>
    <button class="tab-btn" onclick="switchTab('lb-to-kg')">
      <span class="tab-label">Libbre → Chilogrammi</span>
    </button>
  </div>
  
  <div id="kg-to-lb" class="converter-panel active">
    <div class="input-wrapper">
      <label for="kg-input">Chilogrammi (kg)</label>
      <input type="number" id="kg-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertKgToLb()">
      <span class="button-icon">⚡</span>Converti in Libbre
    </button>
    <div id="kg-result" class="result-box"></div>
  </div>
  
  <div id="lb-to-kg" class="converter-panel">
    <div class="input-wrapper">
      <label for="lb-input">Libbre (lb)</label>
      <input type="number" id="lb-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertLbToKg()">
      <span class="button-icon">⚡</span>Converti in Chilogrammi
    </button>
    <div id="lb-result" class="result-box"></div>
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
  const kgPanel = document.getElementById('kg-to-lb');
  const lbPanel = document.getElementById('lb-to-kg');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (tabId === 'kg-to-lb') {
    kgPanel.classList.add('active');
    lbPanel.classList.remove('active');
    buttons[0].classList.add('active');
    buttons[1].classList.remove('active');
  } else {
    lbPanel.classList.add('active');
    kgPanel.classList.remove('active');
    buttons[1].classList.add('active');
    buttons[0].classList.remove('active');
  }
}

function convertKgToLb() {
  const kg = parseFloat(document.getElementById('kg-input').value);
  const resultDiv = document.getElementById('kg-result');
  
  if (isNaN(kg) || kg < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const lb = kg * 2.20462;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${kg.toFixed(2)} kg = <strong>${lb.toFixed(2)} libbre</strong>
      </div>
    </div>
  `;
}

function convertLbToKg() {
  const lb = parseFloat(document.getElementById('lb-input').value);
  const resultDiv = document.getElementById('lb-result');
  
  if (isNaN(lb) || lb < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const kg = lb * 0.453592;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${lb.toFixed(2)} lb = <strong>${kg.toFixed(2)} chilogrammi</strong>
      </div>
    </div>
  `;
}

window.addEventListener('load', function() {
  document.getElementById('kg-input').value = '10';
  convertKgToLb();
});
</script>

<div class="content-section">
<h2>Come usare il convertitore chilogrammi libbre</h2>
<p>Questo strumento ti permette di convertire facilmente tra chilogrammi e libbre in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.</p>

<h3>Quando serve convertire chilogrammi in libbre</h3>
<p>La conversione tra chilogrammi e libbre è fondamentale per il peso corporeo quando si consultano programmi di fitness o diete internazionali. Per i bagagli aerei, molte compagnie usano limiti in libbre per i voli negli Stati Uniti. Nelle ricette di cucina americana, gli ingredienti sono spesso indicati in libbre e once.</p>

<p>Chi pratica sollevamento pesi deve convertire i pesi delle attrezzature quando segue programmi di allenamento internazionali. Anche nelle spedizioni internazionali, conoscere il peso in libbre è essenziale per calcolare correttamente i costi di trasporto verso paesi che usano il sistema imperiale.</p>

<h3>Formula di conversione</h3>
<p><strong>Da chilogrammi a libbre:</strong> 1 kg = 2.20462 libbre<br>
<strong>Da libbre a chilogrammi:</strong> 1 libbra = 0.453592 kg</p>

<p>La conversione è basata sulla definizione internazionale che stabilisce 1 libbra (pound) pari esattamente a 0.45359237 chilogrammi. Questa relazione deriva dalla standardizzazione dei pesi e misure stabilita nel 1959.</p>

<h3>Tabella conversione rapida kg - libbre</h3>
<div class="conversion-table">
<table>
<tr><th>Chilogrammi</th><th>Libbre</th><th></th><th>Libbre</th><th>Chilogrammi</th></tr>
<tr><td>1 kg</td><td>2.20 lb</td><td></td><td>1 lb</td><td>0.45 kg</td></tr>
<tr><td>5 kg</td><td>11.02 lb</td><td></td><td>5 lb</td><td>2.27 kg</td></tr>
<tr><td>10 kg</td><td>22.05 lb</td><td></td><td>10 lb</td><td>4.54 kg</td></tr>
<tr><td>20 kg</td><td>44.09 lb</td><td></td><td>20 lb</td><td>9.07 kg</td></tr>
<tr><td>50 kg</td><td>110.23 lb</td><td></td><td>50 lb</td><td>22.68 kg</td></tr>
<tr><td>100 kg</td><td>220.46 lb</td><td></td><td>100 lb</td><td>45.36 kg</td></tr>
</table>
</div>
</div>

<div class="related-tools">
<h3>Convertitori correlati</h3>
<div class="related-grid">
<a href="/smart-converter-tools/calcolatori/convertitore-grammi-once/" class="related-card">
  <span class="related-icon">🍳</span>
  <span class="related-title">Grammi ↔ Once</span>
</a>
<a href="/smart-converter-tools/calcolatori/convertitore-chilometri-miglia/" class="related-card">
  <span class="related-icon">🚗</span>
  <span class="related-title">Km ↔ Miglia</span>
</a>
<a href="/smart-converter-tools/calcolatori/convertitore-metri-piedi/" class="related-card">
  <span class="related-icon">📐</span>
  <span class="related-title">Metri ↔ Piedi</span>
</a>
</div>
</div>
