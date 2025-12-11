---
layout: calculator
title: "Convertitore Metri Piedi | m ↔ ft Online Gratis"
description: "Converti metri in piedi e pollici istantaneamente. Include conversione piedi-pollici separati. Calcolatore gratuito e preciso per edilizia e misure."
category: "convertitori-unita"
subcategory: "lunghezza"
---

<div class="calculator-container">
  <h2>Convertitore Metri Piedi</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('m-to-ft')">Metri → Piedi</button>
    <button class="tab-btn" onclick="switchTab('ft-to-m')">Piedi → Metri</button>
  </div>
  
  <div id="m-to-ft" class="converter-panel active">
    <div class="input-group">
      <label for="m-input">Metri (m)</label>
      <input type="number" id="m-input" placeholder="Inserisci metri" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertMToFt()">Converti in Piedi</button>
    
    <div id="m-result" class="result-box"></div>
  </div>
  
  <div id="ft-to-m" class="converter-panel">
    <div class="input-group">
      <label for="ft-input">Piedi (ft)</label>
      <input type="number" id="ft-input" placeholder="Inserisci piedi" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertFtToM()">Converti in Metri</button>
    
    <div id="ft-result" class="result-box"></div>
  </div>
</div>

<script>
function switchTab(direction) {
  const mPanel = document.getElementById('m-to-ft');
  const ftPanel = document.getElementById('ft-to-m');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (direction === 'm-to-ft') {
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
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const feet = meters * 3.28084;
  const totalInches = feet * 12;
  const wholeFeet = Math.floor(feet);
  const inches = (feet - wholeFeet) * 12;
  
  resultDiv.innerHTML = `
    <p class="result-value">${meters.toFixed(2)} m = <strong>${feet.toFixed(2)} piedi</strong></p>
    <p class="result-alt">oppure ${wholeFeet} piedi e ${inches.toFixed(1)} pollici</p>
  `;
}

function convertFtToM() {
  const feet = parseFloat(document.getElementById('ft-input').value);
  const resultDiv = document.getElementById('ft-result');
  
  if (isNaN(feet) || feet < 0) {
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const meters = feet * 0.3048;
  resultDiv.innerHTML = `<p class="result-value">${feet.toFixed(2)} ft = <strong>${meters.toFixed(2)} metri</strong></p>`;
}

// Calcolo automatico al caricamento
window.addEventListener('load', function() {
  document.getElementById('m-input').value = '10';
  convertMToFt();
});
</script>

## Come usare il convertitore metri piedi

Questo convertitore permette di trasformare misure in metri a piedi e viceversa con estrema precisione. Usa le tab per selezionare la direzione di conversione, inserisci il valore numerico e ottieni immediatamente il risultato. La conversione da metri a piedi mostra anche il formato alternativo in piedi e pollici separati, particolarmente utile in edilizia.

### Quando serve convertire metri in piedi

La conversione tra metri e piedi è fondamentale in molti contesti professionali e quotidiani. Nel settore edile e dell'architettura, chi lavora con progetti internazionali deve frequentemente convertire misure tra sistema metrico e imperiale. I disegni tecnici americani usano piedi e pollici, mentre quelli europei utilizzano metri e centimetri.

Anche per la casa, quando si acquistano mobili o materiali da paesi che usano sistemi di misura diversi, questa conversione è essenziale. Le specifiche di altezza, larghezza e profondità possono essere espresse in piedi, e convertirle in metri aiuta a verificare che gli oggetti si adattino agli spazi disponibili. Chi pratica sport come il salto in alto o la pallacanestro incontra spesso misure in piedi che devono essere convertite.

### Formula di conversione

**Da metri a piedi:** 1 m = 3.28084 piedi
**Da piedi a metri:** 1 piede = 0.3048 m

Il piede internazionale è definito esattamente come 0.3048 metri dal 1959. Questa definizione standardizzata garantisce che le conversioni siano sempre precise e universalmente accettate. La conversione è quindi una proporzione matematica fissa.

### Tabella conversione rapida metri - piedi

| Metri | Piedi | | Piedi | Metri |
|-------|-------|---|-------|-------|
| 1 m | 3.28 ft | | 1 ft | 0.30 m |
| 2 m | 6.56 ft | | 5 ft | 1.52 m |
| 3 m | 9.84 ft | | 10 ft | 3.05 m |
| 5 m | 16.40 ft | | 20 ft | 6.10 m |
| 10 m | 32.81 ft | | 50 ft | 15.24 m |
| 20 m | 65.62 ft | | 100 ft | 30.48 m |
| 50 m | 164.04 ft | | 200 ft | 60.96 m |

## Convertitori correlati

Potrebbero interessarti anche questi strumenti di conversione:

- [Convertitore Chilometri Miglia](/smart-converter-tools/calcolatori/convertitore-chilometri-miglia/) - per distanze lunghe
- [Convertitore Centimetri Pollici](/smart-converter-tools/calcolatori/convertitore-centimetri-pollici/) - per misure più piccole
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

.result-alt {
  font-size: 0.9rem;
  color: #666;
  margin-top: 0.5rem;
}
</style>
