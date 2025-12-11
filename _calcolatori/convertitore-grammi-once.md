---
layout: calculator
title: "Convertitore Grammi Once | g ↔ oz Online"
description: "Converti grammi in once e once in grammi. Calcolatore preciso per cucina, ricette americane, gioielli e pesi piccoli."
category: "convertitori-unita"
subcategory: "peso"
related:
  - convertitore-chilogrammi-libbre
  - convertitore-litri-galloni
  - calcolo-percentuale
cross_category:
  - calcolo-sconto
---

<div class="calculator-container">
  <h2>Convertitore Grammi Once</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('g-to-oz')">g → oz</button>
    <button class="tab-btn" onclick="switchTab('oz-to-g')">oz → g</button>
  </div>
  
  <div id="g-to-oz" class="converter-panel active">
    <div class="input-group">
      <label for="grammi">Grammi (g)</label>
      <input type="number" id="grammi" placeholder="Inserisci grammi" value="100" step="1">
    </div>
    
    <button class="btn-calculate" onclick="convertGToOz()">Converti g → oz</button>
    
    <div id="result-g-oz" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-g-oz"></p>
    </div>
  </div>
  
  <div id="oz-to-g" class="converter-panel">
    <div class="input-group">
      <label for="once">Once (oz)</label>
      <input type="number" id="once" placeholder="Inserisci once" value="4" step="0.1">
    </div>
    
    <button class="btn-calculate" onclick="convertOzToG()">Converti oz → g</button>
    
    <div id="result-oz-g" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-oz-g"></p>
    </div>
  </div>
</div>

<script>
function switchTab(direction) {
  const tabs = document.querySelectorAll('.tab-btn');
  const panels = document.querySelectorAll('.converter-panel');
  
  tabs.forEach(tab => tab.classList.remove('active'));
  panels.forEach(panel => panel.classList.remove('active'));
  
  if (direction === 'g-to-oz') {
    tabs[0].classList.add('active');
    document.getElementById('g-to-oz').classList.add('active');
  } else {
    tabs[1].classList.add('active');
    document.getElementById('oz-to-g').classList.add('active');
  }
}

function convertGToOz() {
  const grammi = parseFloat(document.getElementById('grammi').value);
  
  if (isNaN(grammi) || grammi < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 grammo = 0.035274 once
  const once = (grammi * 0.035274).toFixed(2);
  
  document.getElementById('resultText-g-oz').innerHTML = 
    `<strong>${grammi.toFixed(0)} g</strong> = <strong>${once} oz</strong><br>` +
    `<small>Fattore di conversione: 1 g = 0.035274 once</small>`;
  
  document.getElementById('result-g-oz').style.display = 'block';
}

function convertOzToG() {
  const once = parseFloat(document.getElementById('once').value);
  
  if (isNaN(once) || once < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 oncia = 28.3495 grammi
  const grammi = (once * 28.3495).toFixed(1);
  
  document.getElementById('resultText-oz-g').innerHTML = 
    `<strong>${once.toFixed(1)} oz</strong> = <strong>${grammi} g</strong><br>` +
    `<small>Fattore di conversione: 1 oncia = 28.3495 grammi</small>`;
  
  document.getElementById('result-oz-g').style.display = 'block';
}

window.onload = function() {
  convertGToOz();
};
</script>

<style>
.converter-tabs {
  display: flex;
  gap: 10px;
  margin-bottom: 20px;
}

.tab-btn {
  flex: 1;
  padding: 12px;
  background: #f0f0f0;
  border: 2px solid #e0e0e0;
  border-radius: 8px;
  cursor: pointer;
  font-size: 16px;
  font-weight: 600;
  transition: all 0.3s ease;
}

.tab-btn:hover {
  background: #e8e8e8;
}

.tab-btn.active {
  background: #0066FF;
  color: white;
  border-color: #0066FF;
}

.converter-panel {
  display: none;
}

.converter-panel.active {
  display: block;
}
</style>

## Come Usare il Convertitore Grammi Once

Il **convertitore grammi once** è perfetto per cucina, ricette americane, gioielleria e piccoli pesi. Converti facilmente tra il sistema metrico (grammi) e il sistema imperiale (once).

### Funzionalità del Convertitore

- **Bidirezionale**: converti da grammi a once e viceversa
- **Precisione culinaria**: ideale per dosaggi ricette
- **Calcolo immediato**: risultati istantanei
- **Interfaccia pulita**: semplice e veloce
- **Mobile-ready**: funziona su tutti i dispositivi

### Formula Conversione g-oz

La conversione tra grammi e once segue questi rapporti:

- **1 grammo = 0,035274 once**
- **1 oncia = 28,3495 grammi**

L'oncia (ounce, simbolo oz) è usata principalmente per ingredienti, alimenti e oggetti piccoli nel sistema imperiale americano.

### Quando Serve Convertire Grammi in Once

**Ricette americane**: Molte ricette USA indicano ingredienti in once. Se una ricetta richiede 8 oz di farina, corrispondono a circa 227 grammi. Convertire correttamente garantisce la riuscita del piatto.

**Cucina e bakery**: Le bilance americane misurano in once. Una porzione di formaggio da 2 oz equivale a circa 57 grammi. I pasticceri devono saper convertire per seguire ricette internazionali.

**Gioielli e metalli preziosi**: Oro e argento si pesano in once troy (leggermente diverse). Un'oncia troy = 31,1 grammi. Per investimenti in metalli preziosi serve conoscere questa conversione.

**Nutrizione e porzioni**: Le etichette alimentari americane indicano porzioni in once. Una porzione da 1 oz di noci equivale a circa 28 grammi, utile per contare calorie.

**Caffè e tè**: I baristi americani dosano caffè in once. Una tazza standard da 6 oz corrisponde a circa 170 grammi di liquido.

### Conversioni Comuni Grammi-Once

| Grammi | Once | Uso Tipico |
|--------|------|------------|
| 15 g | 0,5 oz | Cucchiaio ingrediente |
| 28 g | 1 oz | Porzione snack |
| 100 g | 3,5 oz | Porzione carne |
| 200 g | 7 oz | Tazza farina |
| 250 g | 8,8 oz | Stick burro |
| 500 g | 17,6 oz | Confezione pasta |

### Oncia Troy vs Oncia Avoirdupois

Esistono due tipi di once:

**Oncia avoirdupois** (oz): 28,35 grammi, usata per cibo e oggetti comuni. È quella del nostro convertitore.

**Oncia troy** (oz t): 31,10 grammi, usata solo per metalli preziosi. Un'oncia d'oro si riferisce sempre a once troy.

La differenza è significativa: comprare oro pensando alle once comuni ti fa perdere circa il 10% del peso!

### Misure Cucina USA in Once

Le misure volumetriche americane (cups, tablespoon) hanno anche equivalenze in once di peso:

- **1 cup farina = 4,5 oz = 128 g**
- **1 cup zucchero = 7 oz = 200 g**
- **1 tablespoon = 0,5 oz = 14 g**
- **1 stick burro = 4 oz = 113 g**

Attenzione: queste equivalenze peso-volume variano per ogni ingrediente. Una tazza di farina pesa meno di una tazza di zucchero.

## Strumenti Correlati

- [Convertitore Chilogrammi Libbre](/calcolatori/convertitore-chilogrammi-libbre/) - pesi maggiori
- [Convertitore Litri Galloni](/calcolatori/convertitore-litri-galloni/) - liquidi
- [Calcolo Percentuale](/calcolatori/calcolo-percentuale/) - proporzioni ricette
