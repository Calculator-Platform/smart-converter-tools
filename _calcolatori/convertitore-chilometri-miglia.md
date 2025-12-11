---
layout: calculator
title: "Convertitore Chilometri Miglia | km ↔ mi Online Gratis"
description: "Converti chilometri in miglia e miglia in km istantaneamente. Calcolatore gratuito con tabella di conversione rapida. Semplice e preciso."
category: "convertitori-unita"
subcategory: "lunghezza"
---

<div class="calculator-container">
  <h2>Convertitore Chilometri Miglia</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('km-to-mi')">Chilometri → Miglia</button>
    <button class="tab-btn" onclick="switchTab('mi-to-km')">Miglia → Chilometri</button>
  </div>
  
  <div id="km-to-mi" class="converter-panel active">
    <div class="input-group">
      <label for="km-input">Chilometri (km)</label>
      <input type="number" id="km-input" placeholder="Inserisci chilometri" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertKmToMi()">Converti in Miglia</button>
    
    <div id="km-result" class="result-box"></div>
  </div>
  
  <div id="mi-to-km" class="converter-panel">
    <div class="input-group">
      <label for="mi-input">Miglia (mi)</label>
      <input type="number" id="mi-input" placeholder="Inserisci miglia" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertMiToKm()">Converti in Chilometri</button>
    
    <div id="mi-result" class="result-box"></div>
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
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const miles = km * 0.621371;
  resultDiv.innerHTML = `<p class="result-value">${km.toFixed(2)} km = <strong>${miles.toFixed(2)} miglia</strong></p>`;
}

function convertMiToKm() {
  const miles = parseFloat(document.getElementById('mi-input').value);
  const resultDiv = document.getElementById('mi-result');
  
  if (isNaN(miles) || miles < 0) {
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const km = miles * 1.60934;
  resultDiv.innerHTML = `<p class="result-value">${miles.toFixed(2)} mi = <strong>${km.toFixed(2)} chilometri</strong></p>`;
}

// Calcolo automatico al caricamento
window.addEventListener('load', function() {
  document.getElementById('km-input').value = '10';
  convertKmToMi();
});
</script>

## Come usare il convertitore chilometri miglia

Questo strumento ti permette di convertire facilmente tra chilometri e miglia in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.

### Quando serve convertire km in miglia

La conversione tra chilometri e miglia è essenziale in molte situazioni quotidiane. Se stai pianificando un viaggio negli Stati Uniti o nel Regno Unito, dove le distanze sono espresse in miglia, dovrai convertire le distanze dal sistema metrico. Anche per comprendere i limiti di velocità, le distanze su cartelli stradali o le specifiche di veicoli importati, questa conversione risulta fondamentale.

Gli sportivi che seguono programmi di allenamento internazionali spesso devono convertire distanze di corsa o ciclismo. Allo stesso modo, chi segue mappe e indicazioni stradali di paesi che usano il sistema imperiale necessita di questa conversione per pianificare correttamente i propri spostamenti.

### Formula di conversione

**Da chilometri a miglia:** 1 km = 0.621371 miglia
**Da miglia a chilometri:** 1 miglio = 1.60934 km

Queste formule derivano dal fatto che un miglio internazionale è definito esattamente come 1,609.344 metri, mentre un chilometro equivale a 1,000 metri. La conversione è quindi una proporzione fissa e non cambia nel tempo.

### Tabella conversione rapida km - miglia

| Chilometri | Miglia | | Miglia | Chilometri |
|------------|--------|---|--------|------------|
| 1 km | 0.62 mi | | 1 mi | 1.61 km |
| 5 km | 3.11 mi | | 5 mi | 8.05 km |
| 10 km | 6.21 mi | | 10 mi | 16.09 km |
| 20 km | 12.43 mi | | 20 mi | 32.19 km |
| 50 km | 31.07 mi | | 50 mi | 80.47 km |
| 100 km | 62.14 mi | | 100 mi | 160.93 km |
| 200 km | 124.27 mi | | 200 mi | 321.87 km |

## Convertitori correlati

Potrebbero interessarti anche questi strumenti di conversione:

- [Convertitore Metri Piedi](/smart-converter-tools/calcolatori/convertitore-metri-piedi/) - converti metri in piedi e pollici
- [Convertitore Centimetri Pollici](/smart-converter-tools/calcolatori/convertitore-centimetri-pollici/) - converti cm in pollici
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
