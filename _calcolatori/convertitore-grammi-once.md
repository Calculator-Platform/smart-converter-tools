---
layout: calculator
title: "Convertitore Grammi Once | g ↔ oz | Online Gratis"
description: "Converti grammi in once e once in grammi istantaneamente. Calcolatore gratuito con tabella di conversione rapida."
category: "convertitori-unita"
subcategory: "peso"
emoji: "⚖️"
---

<div class="page-hero">
  <h1>🍳 Convertitore Grammi Once</h1>
  <p>Converti velocemente tra grammi e once</p>
</div>

<!-- ADV SPOT 1: Banner principale above fold -->
<div class="ad-container ad-primary">
  <div class="ad-placeholder ad-main">
    <span class="ad-text">Banner 728×90</span>
  </div>
</div>

<div class="calculator-box">
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('g-to-oz')">
      <span class="tab-label">Grammi → Once</span>
    </button>
    <button class="tab-btn" onclick="switchTab('oz-to-g')">
      <span class="tab-label">Once → Grammi</span>
    </button>
  </div>
  
  <div id="g-to-oz" class="converter-panel active">
    <div class="input-wrapper">
      <label for="g-input">Grammi (g)</label>
      <input type="number" id="g-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertGToOz()">
      <span class="button-icon">⚡</span>Converti in Once
    </button>
    <div id="g-result" class="result-box"></div>
  </div>
  
  <div id="oz-to-g" class="converter-panel">
    <div class="input-wrapper">
      <label for="oz-input">Once (oz)</label>
      <input type="number" id="oz-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertOzToG()">
      <span class="button-icon">⚡</span>Converti in Grammi
    </button>
    <div id="oz-result" class="result-box"></div>
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
  const gPanel = document.getElementById('g-to-oz');
  const ozPanel = document.getElementById('oz-to-g');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (tabId === 'g-to-oz') {
    gPanel.classList.add('active');
    ozPanel.classList.remove('active');
    buttons[0].classList.add('active');
    buttons[1].classList.remove('active');
  } else {
    ozPanel.classList.add('active');
    gPanel.classList.remove('active');
    buttons[1].classList.add('active');
    buttons[0].classList.remove('active');
  }
}

function convertGToOz() {
  const grams = parseFloat(document.getElementById('g-input').value);
  const resultDiv = document.getElementById('g-result');
  
  if (isNaN(grams) || grams < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const ounces = grams * 0.035274;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${grams.toFixed(2)} g = <strong>${ounces.toFixed(2)} once</strong>
      </div>
    </div>
  `;
}

function convertOzToG() {
  const ounces = parseFloat(document.getElementById('oz-input').value);
  const resultDiv = document.getElementById('oz-result');
  
  if (isNaN(ounces) || ounces < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const grams = ounces * 28.3495;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${ounces.toFixed(2)} oz = <strong>${grams.toFixed(2)} grammi</strong>
      </div>
    </div>
  `;
}

window.addEventListener('load', function() {
  document.getElementById('g-input').value = '100';
  convertGToOz();
});
</script>

<div class="content-section">
<h2>Come usare il convertitore grammi once</h2>
<p>Questo strumento ti permette di convertire facilmente tra grammi e once in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.</p>

<h3>Quando serve convertire grammi in once</h3>
<p>La conversione tra grammi e once è fondamentale in cucina quando si seguono ricette americane o britanniche. Le ricette di pasticceria richiedono particolare precisione nelle dosi, e molte sono scritte in once. Anche per il dosaggio di integratori alimentari e prodotti nutrizionali, le etichette spesso riportano informazioni in once.</p>

<p>Nel settore dei preziosi, l'oro e l'argento vengono pesati in once troy (leggermente diverse dalle once standard). Per la spedizione di piccoli pacchi internazionali, conoscere il peso in once può essere utile per calcolare i costi verso destinazioni che usano il sistema imperiale.</p>

<h3>Formula di conversione</h3>
<p><strong>Da grammi a once:</strong> 1 g = 0.035274 once<br>
<strong>Da once a grammi:</strong> 1 oncia = 28.3495 g</p>

<p>La conversione si basa sulla definizione internazionale che stabilisce 1 oncia (ounce) pari a esattamente 28.349523125 grammi. Questo valore è parte del sistema avoirdupois, lo standard più comune per pesare alimenti e oggetti di uso quotidiano.</p>

<h3>Tabella conversione rapida grammi - once</h3>
<div class="conversion-table">
<table>
<tr><th>Grammi</th><th>Once</th><th></th><th>Once</th><th>Grammi</th></tr>
<tr><td>10 g</td><td>0.35 oz</td><td></td><td>1 oz</td><td>28.35 g</td></tr>
<tr><td>50 g</td><td>1.76 oz</td><td></td><td>2 oz</td><td>56.70 g</td></tr>
<tr><td>100 g</td><td>3.53 oz</td><td></td><td>4 oz</td><td>113.40 g</td></tr>
<tr><td>250 g</td><td>8.82 oz</td><td></td><td>8 oz</td><td>226.80 g</td></tr>
<tr><td>500 g</td><td>17.64 oz</td><td></td><td>16 oz</td><td>453.59 g</td></tr>
<tr><td>1000 g</td><td>35.27 oz</td><td></td><td>32 oz</td><td>907.18 g</td></tr>
</table>
</div>
</div>
