---
layout: calculator
title: "Convertitore Grammi Once | g ↔ oz Online Gratis"
description: "Converti grammi in once e once in grammi facilmente. Perfetto per ricette, cucina e pesate precise. Calcolatore gratuito con conversione istantanea."
category: "convertitori-unita"
subcategory: "peso"
related:
  - convertitore-chilogrammi-libbre
---

<div class="calculator-container">
  <h2>Convertitore Grammi Once</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('g-to-oz')">Grammi → Once</button>
    <button class="tab-btn" onclick="switchTab('oz-to-g')">Once → Grammi</button>
  </div>
  
  <div id="g-to-oz" class="converter-panel active">
    <div class="input-group">
      <label for="g-input">Grammi (g)</label>
      <input type="number" id="g-input" placeholder="Inserisci grammi" step="0.1" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertGToOz()">Converti in Once</button>
    
    <div id="g-result" class="result-box"></div>
  </div>
  
  <div id="oz-to-g" class="converter-panel">
    <div class="input-group">
      <label for="oz-input">Once (oz)</label>
      <input type="number" id="oz-input" placeholder="Inserisci once" step="0.1" min="0">
    </div>
    
    <button class="calculate-btn" onclick="convertOzToG()">Converti in Grammi</button>
    
    <div id="oz-result" class="result-box"></div>
  </div>
</div>

<script>
function switchTab(direction) {
  const gPanel = document.getElementById('g-to-oz');
  const ozPanel = document.getElementById('oz-to-g');
  const buttons = document.querySelectorAll('.tab-btn');
  
  if (direction === 'g-to-oz') {
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
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const ounces = grams * 0.035274;
  resultDiv.innerHTML = `<p class="result-value">${grams.toFixed(1)} g = <strong>${ounces.toFixed(2)} once</strong></p>`;
}

function convertOzToG() {
  const ounces = parseFloat(document.getElementById('oz-input').value);
  const resultDiv = document.getElementById('oz-result');
  
  if (isNaN(ounces) || ounces < 0) {
    resultDiv.innerHTML = '<p class="error">Inserisci un valore valido (numero positivo)</p>';
    return;
  }
  
  const grams = ounces * 28.3495;
  resultDiv.innerHTML = `<p class="result-value">${ounces.toFixed(2)} oz = <strong>${grams.toFixed(1)} grammi</strong></p>`;
}

// Calcolo automatico al caricamento
window.addEventListener('load', function() {
  document.getElementById('g-input').value = '100';
  convertGToOz();
});
</script>

## Come usare il convertitore grammi once

Questo strumento di conversione è stato progettato per essere intuitivo e veloce. Seleziona la direzione di conversione utilizzando le tab in alto, digita il valore nella casella di input e premi il pulsante di conversione. Il risultato viene mostrato immediatamente con la precisione appropriata per l'uso culinario.

### Quando serve convertire grammi in once

La conversione tra grammi e once è fondamentale principalmente in cucina e pasticceria. Le ricette americane utilizzano sistematicamente once per indicare le quantità degli ingredienti, mentre in Europa si preferisce il sistema metrico con i grammi. Chi ama sperimentare ricette internazionali si trova spesso nella necessità di convertire queste misure per ottenere risultati precisi.

Nella preparazione di dolci e prodotti da forno, la precisione è cruciale. Una piccola differenza nelle quantità di farina, zucchero o burro può compromettere la riuscita della ricetta. Convertire accuratamente le once in grammi o viceversa garantisce di seguire correttamente le proporzioni indicate dalla ricetta originale.

Anche nell'ambito del fitness e della nutrizione, molte app e programmi alimentari americani indicano le porzioni in once. Chi segue una dieta specifica o monitora l'apporto proteico necessita di convertire questi valori in grammi per pesare correttamente gli alimenti sulla propria bilancia metrica.

Nel settore dei metalli preziosi e della gioielleria, le once troy sono utilizzate per pesare oro, argento e pietre preziose. Anche se l'oncia troy è leggermente diversa dall'oncia standard, la conversione di base rimane simile e questo strumento fornisce un'ottima approssimazione per calcoli generali.

### Formula di conversione

**Da grammi a once:** 1 g = 0.035274 once
**Da once a grammi:** 1 oncia = 28.3495 g

L'oncia avoirdupois, utilizzata per pesi generali e in cucina, è definita come esattamente 28.349523125 grammi. Questa definizione standardizzata garantisce conversioni precise e universalmente riconosciute. Il fattore di conversione è fisso e non cambia.

### Tabella conversione rapida grammi - once

| Grammi | Once | | Once | Grammi |
|--------|------|---|------|--------|
| 10 g | 0.35 oz | | 1 oz | 28.35 g |
| 25 g | 0.88 oz | | 2 oz | 56.70 g |
| 50 g | 1.76 oz | | 4 oz | 113.40 g |
| 100 g | 3.53 oz | | 8 oz | 226.80 g |
| 250 g | 8.82 oz | | 16 oz | 453.59 g |
| 500 g | 17.64 oz | | 32 oz | 907.18 g |

### Ingredienti comuni in cucina

| Ingrediente | Grammi | Once |
|-------------|--------|------|
| Farina | 125 g | 4.4 oz |
| Zucchero | 200 g | 7.1 oz |
| Burro | 113 g | 4 oz |
| Cacao in polvere | 30 g | 1.1 oz |
| Cioccolato | 170 g | 6 oz |
| Farina di mandorle | 100 g | 3.5 oz |

## Convertitori correlati

Potrebbero interessarti anche questi strumenti:

- [Convertitore Chilogrammi Libbre](/calcolatori/convertitore-chilogrammi-libbre/) - per pesi più grandi

Altri convertitori utili:

- [Convertitore Chilometri Miglia](/calcolatori/convertitore-chilometri-miglia/) - per distanze
- [Convertitore Metri Piedi](/calcolatori/convertitore-metri-piedi/) - per lunghezze
- [Convertitore Centimetri Pollici](/calcolatori/convertitore-centimetri-pollici/) - per misure piccole

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
