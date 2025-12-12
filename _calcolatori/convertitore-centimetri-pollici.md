---
layout: calculator
title: "Convertitore Centimetri Pollici | cm ↔ inch | Online Gratis"
description: "Converti centimetri in pollici e pollici in cm istantaneamente. Calcolatore gratuito con tabella di conversione rapida."
category: "convertitori-unita"
subcategory: "lunghezza"
---

<div class="page-hero">
  <h1>📱 Convertitore Centimetri Pollici</h1>
  <p>Converti velocemente tra cm e pollici</p>
</div>

<div class="calculator-box">
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('cm-to-in')">
      <span class="tab-label">Centimetri → Pollici</span>
    </button>
    <button class="tab-btn" onclick="switchTab('in-to-cm')">
      <span class="tab-label">Pollici → Centimetri</span>
    </button>
  </div>
  
  <div id="cm-to-in" class="converter-panel active">
    <div class="input-wrapper">
      <label for="cm-input">Centimetri (cm)</label>
      <input type="number" id="cm-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertCmToIn()">
      <span class="button-icon">⚡</span>Converti in Pollici
    </button>
    <div id="cm-result" class="result-box"></div>
  </div>
  
  <div id="in-to-cm" class="converter-panel">
    <div class="input-wrapper">
      <label for="in-input">Pollici (inch)</label>
      <input type="number" id="in-input" placeholder="Inserisci valore" step="0.01" min="0">
    </div>
    <button class="calc-button" onclick="convertInToCm()">
      <span class="button-icon">⚡</span>Converti in Centimetri
    </button>
    <div id="in-result" class="result-box"></div>
  </div>
</div>

<script>
function switchTab(tabId) {
  const cmPanel = document.getElementById('cm-to-in');
  const inPanel = document.getElementById('in-to-cm');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (tabId === 'cm-to-in') {
    cmPanel.classList.add('active');
    inPanel.classList.remove('active');
    buttons[0].classList.add('active');
    buttons[1].classList.remove('active');
  } else {
    inPanel.classList.add('active');
    cmPanel.classList.remove('active');
    buttons[1].classList.add('active');
    buttons[0].classList.remove('active');
  }
}

function convertCmToIn() {
  const cm = parseFloat(document.getElementById('cm-input').value);
  const resultDiv = document.getElementById('cm-result');
  
  if (isNaN(cm) || cm < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const inches = cm * 0.393701;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${cm.toFixed(2)} cm = <strong>${inches.toFixed(2)} pollici</strong>
      </div>
    </div>
  `;
}

function convertInToCm() {
  const inches = parseFloat(document.getElementById('in-input').value);
  const resultDiv = document.getElementById('in-result');
  
  if (isNaN(inches) || inches < 0) {
    resultDiv.innerHTML = '<div class="error-message">⚠️ Inserisci un numero valido</div>';
    return;
  }
  
  const cm = inches * 2.54;
  resultDiv.innerHTML = `
    <div class="result-success">
      <div class="result-main">
        ${inches.toFixed(2)} inch = <strong>${cm.toFixed(2)} centimetri</strong>
      </div>
    </div>
  `;
}

window.addEventListener('load', function() {
  document.getElementById('cm-input').value = '10';
  convertCmToIn();
});
</script>

<div class="content-section">

## Come usare il convertitore centimetri pollici

Questo strumento ti permette di convertire facilmente tra centimetri e pollici in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.

### Quando serve convertire centimetri in pollici

La conversione tra centimetri e pollici è essenziale per misure di schermi TV e monitor, dove le dimensioni sono sempre espresse in pollici. Anche nel settore dell'abbigliamento, molti capi importati utilizzano taglie in pollici che necessitano conversione. Per progetti di fai-da-te e bricolage con materiali provenienti da paesi che usano il sistema imperiale, questa conversione è indispensabile.

Chi lavora con design grafico e stampa deve spesso convertire tra centimetri e pollici per adattare i progetti a standard internazionali. Anche per l'altezza delle persone, alcuni paesi esprimono la statura in piedi e pollici anziché in centimetri.

### Formula di conversione

**Da centimetri a pollici:** 1 cm = 0.393701 pollici  
**Da pollici a centimetri:** 1 pollice = 2.54 cm

La conversione è basata sulla definizione internazionale che stabilisce esattamente 1 pollice = 2.54 centimetri. Questa definizione è stata fissata nel 1959 ed è utilizzata in tutto il mondo per garantire uniformità nelle misurazioni.

### Tabella conversione rapida cm - pollici

<div class="conversion-table">

| Centimetri | Pollici | | Pollici | Centimetri |
|------------|---------|---|---------|------------|
| 1 cm | 0.39 in | | 1 in | 2.54 cm |
| 5 cm | 1.97 in | | 5 in | 12.70 cm |
| 10 cm | 3.94 in | | 10 in | 25.40 cm |
| 20 cm | 7.87 in | | 20 in | 50.80 cm |
| 50 cm | 19.69 in | | 50 in | 127.00 cm |
| 100 cm | 39.37 in | | 100 in | 254.00 cm |

</div>

</div>

<div class="related-tools">

### Convertitori correlati

<div class="related-grid">
  <a href="/smart-converter-tools/calcolatori/convertitore-metri-piedi/" class="related-card">
    <span class="related-icon">📐</span>
    <span class="related-title">Metri ↔ Piedi</span>
  </a>
  <a href="/smart-converter-tools/calcolatori/convertitore-chilometri-miglia/" class="related-card">
    <span class="related-icon">🚗</span>
    <span class="related-title">Km ↔ Miglia</span>
  </a>
  <a href="/smart-converter-tools/calcolatori/convertitore-chilogrammi-libbre/" class="related-card">
    <span class="related-icon">⚖️</span>
    <span class="related-title">Kg ↔ Libbre</span>
  </a>
</div>

</div>
