---
layout: calculator
title: "Convertitore Centimetri Pollici | cm ↔ inch Online"
description: "Converti centimetri in pollici e pollici in cm gratis. Calcolatore preciso per abbigliamento, TV, monitor e misure generiche. Conversione istantanea."
category: "convertitori-unita"
subcategory: "lunghezza"
---

<div class="calculator-container">
  <h2>Convertitore Centimetri Pollici</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('cm-to-in')">Centimetri → Pollici</button>
    <button class="tab-btn" onclick="switchTab('in-to-cm')">Pollici → Centimetri</button>
  </div>
  
  <div id="cm-to-in" class="converter-panel active">
    <div class="input-group">
      <label for="cm-input">Centimetri (cm)</label>
      <input type="number" id="cm-input" placeholder="Inserisci centimetri" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertCmToIn()">Converti in Pollici</button>
    
    <div id="cm-result" class="result-box"></div>
  </div>
  
  <div id="in-to-cm" class="converter-panel">
    <div class="input-group">
      <label for="in-input">Pollici (inch)</label>
      <input type="number" id="in-input" placeholder="Inserisci pollici" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertInToCm()">Converti in Centimetri</button>
    
    <div id="in-result" class="result-box"></div>
  </div>
</div>

<script>
function switchTab(direction) {
  const cmPanel = document.getElementById('cm-to-in');
  const inPanel = document.getElementById('in-to-cm');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (direction === 'cm-to-in') {
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
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const inches = cm * 0.393701;
  resultDiv.innerHTML = `<p class="result-value">${cm.toFixed(2)} cm = <strong>${inches.toFixed(2)} pollici</strong></p>`;
}

function convertInToCm() {
  const inches = parseFloat(document.getElementById('in-input').value);
  const resultDiv = document.getElementById('in-result');
  
  if (isNaN(inches) || inches < 0) {
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const cm = inches * 2.54;
  resultDiv.innerHTML = `<p class="result-value">${inches.toFixed(2)} in = <strong>${cm.toFixed(2)} centimetri</strong></p>`;
}

// Calcolo automatico al caricamento
window.addEventListener('load', function() {
  document.getElementById('cm-input').value = '10';
  convertCmToIn();
});
</script>

## Come usare il convertitore centimetri pollici

Questo strumento di conversione è progettato per essere semplice ed immediato. Seleziona la direzione di conversione usando le tab in alto (da cm a pollici o viceversa), inserisci il valore nella casella di input e clicca sul pulsante di conversione. Il risultato appare istantaneamente con precisione di due cifre decimali.

### Quando serve convertire cm in pollici

La conversione tra centimetri e pollici è particolarmente utile in diversi ambiti della vita quotidiana. Quando si acquistano televisori, monitor o tablet, le dimensioni dello schermo sono spesso indicate in pollici, ma per comprendere meglio le dimensioni reali è utile convertirle in centimetri. Lo stesso vale per pneumatici, ruote di biciclette e altri componenti che utilizzano misure in pollici.

Nel mondo della moda e dell'abbigliamento, le taglie americane e britanniche sono spesso espresse in pollici, mentre in Europa si usa il sistema metrico. Convertire misure di vita, fianchi, lunghezza pantaloni o maniche diventa quindi essenziale per acquistare capi che calzino perfettamente. Anche per lavori di bricolage e fai-da-te, quando si usano utensili o materiali importati, questa conversione è fondamentale.

### Formula di conversione

**Da centimetri a pollici:** 1 cm = 0.393701 pollici
**Da pollici a centimetri:** 1 pollice = 2.54 cm

Il pollice è definito esattamente come 2.54 centimetri dal 1959, quando fu stabilita una definizione internazionale unificata. Questa equivalenza precisa rende la conversione sempre accurata e universalmente riconosciuta in tutti i paesi che utilizzano entrambi i sistemi di misura.

### Tabella conversione rapida cm - pollici

| Centimetri | Pollici | | Pollici | Centimetri |
|------------|---------|---|---------|------------|
| 1 cm | 0.39 in | | 1 in | 2.54 cm |
| 5 cm | 1.97 in | | 5 in | 12.70 cm |
| 10 cm | 3.94 in | | 10 in | 25.40 cm |
| 20 cm | 7.87 in | | 20 in | 50.80 cm |
| 50 cm | 19.69 in | | 50 in | 127.00 cm |
| 100 cm | 39.37 in | | 100 in | 254.00 cm |

### Dimensioni schermi comuni

| Pollici | Centimetri | Uso tipico |
|---------|------------|------------|
| 24" | 60.96 cm | Monitor PC |
| 32" | 81.28 cm | TV piccola |
| 43" | 109.22 cm | TV media |
| 55" | 139.70 cm | TV grande |
| 65" | 165.10 cm | TV molto grande |

## Convertitori correlati

Potrebbero interessarti anche questi strumenti di conversione:

- [Convertitore Metri Piedi](/smart-converter-tools/calcolatori/convertitore-metri-piedi/) - per misure più grandi
- [Convertitore Chilometri Miglia](/smart-converter-tools/calcolatori/convertitore-chilometri-miglia/) - per distanze
- [Convertitore Chilogrammi Libbre](/smart-converter-tools/calcolatori/convertitore-chilogrammi-libbre/) - per convertire pesi
- [Convertitore Grammi Once](/smart-converter-tools/calcolatori/convertitore-grammi-once/) - per ricette e cucina

<style>
.converter-tabs {
  display: flex;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.tab-btn {
  flex: 1;
  padding: 0.75rem;
  border: 2px solid #e0e0e0;
  background: white;
  cursor: pointer;
  border-radius: 4px;
  font-size: 1rem;
  transition: all 0.3s;
}

.tab-btn.active {
  background: #667eea;
  color: white;
  border-color: #667eea;
}

.converter-panel {
  display: none;
}

.converter-panel.active {
  display: block;
}
</style>
