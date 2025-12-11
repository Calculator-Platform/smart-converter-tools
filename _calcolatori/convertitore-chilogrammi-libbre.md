---
layout: calculator
title: "Convertitore Chilogrammi Libbre | kg ↔ lb Online"
description: "Converti chilogrammi in libbre e libbre in kg gratis. Calcolatore preciso per peso corporeo, bagagli, ricette e molto altro. Conversione istantanea."
category: "convertitori-unita"
subcategory: "peso"
---

<div class="calculator-container">
  <h2>Convertitore Chilogrammi Libbre</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('kg-to-lb')">Chilogrammi → Libbre</button>
    <button class="tab-btn" onclick="switchTab('lb-to-kg')">Libbre → Chilogrammi</button>
  </div>
  
  <div id="kg-to-lb" class="converter-panel active">
    <div class="input-group">
      <label for="kg-input">Chilogrammi (kg)</label>
      <input type="number" id="kg-input" placeholder="Inserisci chilogrammi" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertKgToLb()">Converti in Libbre</button>
    
    <div id="kg-result" class="result-box"></div>
  </div>
  
  <div id="lb-to-kg" class="converter-panel">
    <div class="input-group">
      <label for="lb-input">Libbre (lb)</label>
      <input type="number" id="lb-input" placeholder="Inserisci libbre" step="0.01" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertLbToKg()">Converti in Chilogrammi</button>
    
    <div id="lb-result" class="result-box"></div>
  </div>
</div>

<script>
function switchTab(direction) {
  const kgPanel = document.getElementById('kg-to-lb');
  const lbPanel = document.getElementById('lb-to-kg');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (direction === 'kg-to-lb') {
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
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const pounds = kg * 2.20462;
  resultDiv.innerHTML = `<p class="result-value">${kg.toFixed(2)} kg = <strong>${pounds.toFixed(2)} libbre</strong></p>`;
}

function convertLbToKg() {
  const pounds = parseFloat(document.getElementById('lb-input').value);
  const resultDiv = document.getElementById('lb-result');
  
  if (isNaN(pounds) || pounds < 0) {
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const kg = pounds * 0.453592;
  resultDiv.innerHTML = `<p class="result-value">${pounds.toFixed(2)} lb = <strong>${kg.toFixed(2)} chilogrammi</strong></p>`;
}

// Calcolo automatico al caricamento
window.addEventListener('load', function() {
  document.getElementById('kg-input').value = '70';
  convertKgToLb();
});
</script>

## Come usare il convertitore chilogrammi libbre

Questo convertitore permette di trasformare rapidamente pesi da chilogrammi a libbre e viceversa. Usa le tab in alto per scegliere la direzione di conversione, inserisci il valore numerico nella casella corrispondente e clicca il pulsante di conversione. Il risultato viene calcolato istantaneamente con precisione al centesimo.

### Quando serve convertire kg in libbre

La conversione tra chilogrammi e libbre è necessaria in moltissime situazioni pratiche. Quando si viaggia verso paesi che utilizzano il sistema imperiale, come Stati Uniti o Regno Unito, i limiti di peso per i bagagli sono spesso espressi in libbre. Convertire il peso del proprio bagaglio da chilogrammi a libbre aiuta a verificare di rientrare nei limiti consentiti dalle compagnie aeree.

Nel mondo del fitness e dello sport, molti programmi di allenamento internazionali utilizzano libbre per indicare i pesi da sollevare o il peso corporeo target. Chi pratica bodybuilding, powerlifting o segue diete americane deve frequentemente convertire tra questi due sistemi. Anche per ricette di cucina internazionali, specialmente quelle americane, gli ingredienti sono spesso indicati in libbre.

In ambito commerciale, quando si acquistano prodotti da fornitori esteri o si spediscono pacchi all'estero, conoscere il peso in libbre oltre che in chilogrammi è fondamentale per calcolare correttamente i costi di spedizione e rispettare le normative doganali.

### Formula di conversione

**Da chilogrammi a libbre:** 1 kg = 2.20462 libbre
**Da libbre a chilogrammi:** 1 libbra = 0.453592 kg

La libbra internazionale è definita esattamente come 0.45359237 chilogrammi dal 1959. Questa definizione standardizzata garantisce che le conversioni siano sempre precise e riconosciute universalmente. Il fattore di conversione deriva dal rapporto tra le due unità di misura.

### Tabella conversione rapida kg - libbre

| Chilogrammi | Libbre | | Libbre | Chilogrammi |
|-------------|--------|---|--------|-------------|
| 1 kg | 2.20 lb | | 1 lb | 0.45 kg |
| 5 kg | 11.02 lb | | 5 lb | 2.27 kg |
| 10 kg | 22.05 lb | | 10 lb | 4.54 kg |
| 20 kg | 44.09 lb | | 20 lb | 9.07 kg |
| 50 kg | 110.23 lb | | 50 lb | 22.68 kg |
| 70 kg | 154.32 lb | | 100 lb | 45.36 kg |
| 100 kg | 220.46 lb | | 150 lb | 68.04 kg |

### Pesi corporei comuni

| Chilogrammi | Libbre | Categoria |
|-------------|--------|-----------|
| 50 kg | 110 lb | Peso leggero |
| 60 kg | 132 lb | Peso medio-leggero |
| 70 kg | 154 lb | Peso medio |
| 80 kg | 176 lb | Peso medio-pesante |
| 90 kg | 198 lb | Peso pesante |
| 100 kg | 220 lb | Peso molto pesante |

## Convertitori correlati

Potrebbero interessarti anche questi strumenti:

- [Convertitore Grammi Once](/smart-converter-tools/calcolatori/convertitore-grammi-once/) - per ricette e cucina
- [Convertitore Chilometri Miglia](/smart-converter-tools/calcolatori/convertitore-chilometri-miglia/) - per distanze
- [Convertitore Metri Piedi](/smart-converter-tools/calcolatori/convertitore-metri-piedi/) - per lunghezze
- [Convertitore Centimetri Pollici](/smart-converter-tools/calcolatori/convertitore-centimetri-pollici/) - per misure piccole

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
