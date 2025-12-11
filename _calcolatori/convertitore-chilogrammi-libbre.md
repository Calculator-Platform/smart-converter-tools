---
layout: calculator
title: "Convertitore Chilogrammi Libbre | kg ↔ lb Online"
description: "Converti chilogrammi in libbre e libbre in kg. Calcolatore preciso per peso corporeo, bagagli, pesi palestra e spedizioni."
category: "convertitori-unita"
subcategory: "peso"
related:
  - convertitore-grammi-once
  - convertitore-metri-piedi
  - convertitore-chilometri-miglia
  - calcolo-percentuale
cross_category:
  - calcolo-sconto
  - calcolo-area-rettangolo
---

<div class="calculator-container">
  <h2>Convertitore Chilogrammi Libbre</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('kg-to-lb')">kg → lb</button>
    <button class="tab-btn" onclick="switchTab('lb-to-kg')">lb → kg</button>
  </div>
  
  <div id="kg-to-lb" class="converter-panel active">
    <div class="input-group">
      <label for="kg">Chilogrammi (kg)</label>
      <input type="number" id="kg" placeholder="Inserisci kg" value="70" step="0.1">
    </div>
    
    <button class="btn-calculate" onclick="convertKgToLb()">Converti kg → lb</button>
    
    <div id="result-kg-lb" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-kg-lb"></p>
    </div>
  </div>
  
  <div id="lb-to-kg" class="converter-panel">
    <div class="input-group">
      <label for="lb">Libbre (lb)</label>
      <input type="number" id="lb" placeholder="Inserisci libbre" value="150" step="0.1">
    </div>
    
    <button class="btn-calculate" onclick="convertLbToKg()">Converti lb → kg</button>
    
    <div id="result-lb-kg" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-lb-kg"></p>
    </div>
  </div>
</div>

<script>
function switchTab(direction) {
  const tabs = document.querySelectorAll('.tab-btn');
  const panels = document.querySelectorAll('.converter-panel');
  
  tabs.forEach(tab => tab.classList.remove('active'));
  panels.forEach(panel => panel.classList.remove('active'));
  
  if (direction === 'kg-to-lb') {
    tabs[0].classList.add('active');
    document.getElementById('kg-to-lb').classList.add('active');
  } else {
    tabs[1].classList.add('active');
    document.getElementById('lb-to-kg').classList.add('active');
  }
}

function convertKgToLb() {
  const kg = parseFloat(document.getElementById('kg').value);
  
  if (isNaN(kg) || kg < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 kg = 2.20462 libbre
  const lb = (kg * 2.20462).toFixed(2);
  
  document.getElementById('resultText-kg-lb').innerHTML = 
    `<strong>${kg.toFixed(1)} kg</strong> = <strong>${lb} lb</strong><br>` +
    `<small>Fattore di conversione: 1 kg = 2.20462 libbre</small>`;
  
  document.getElementById('result-kg-lb').style.display = 'block';
}

function convertLbToKg() {
  const lb = parseFloat(document.getElementById('lb').value);
  
  if (isNaN(lb) || lb < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 libbra = 0.453592 kg
  const kg = (lb * 0.453592).toFixed(2);
  
  document.getElementById('resultText-lb-kg').innerHTML = 
    `<strong>${lb.toFixed(1)} lb</strong> = <strong>${kg} kg</strong><br>` +
    `<small>Fattore di conversione: 1 libbra = 0.453592 kg</small>`;
  
  document.getElementById('result-lb-kg').style.display = 'block';
}

window.onload = function() {
  convertKgToLb();
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

## Come Usare il Convertitore Chilogrammi Libbre

Il **convertitore chilogrammi libbre** è lo strumento essenziale per trasformare misure di peso e massa tra il sistema metrico (chilogrammi) e il sistema imperiale (libbre). Ideale per fitness, viaggi, cucina e commercio internazionale.

### Caratteristiche Principali

- **Doppia conversione**: da kg a libbre e viceversa
- **Precisione professionale**: calcoli accurati per ogni esigenza
- **Interfaccia immediata**: risultati istantanei
- **Formato mobile-friendly**: funziona su tutti i dispositivi
- **Calcolo automatico**: aggiornamento in tempo reale

### Formula di Conversione kg-lb

La conversione tra chilogrammi e libbre segue questi rapporti matematici:

- **1 chilogrammo = 2,20462 libbre**
- **1 libbra = 0,453592 chilogrammi**

La libbra (pound, simbolo lb) è l'unità di massa principale del sistema imperiale, usata principalmente negli USA e in alcuni paesi anglofoni.

### Quando Serve Convertire Chilogrammi in Libbre

**Peso corporeo e fitness**: Negli Stati Uniti il peso si misura in libbre. Se pesi 70 kg, corrispondi a circa 154 libbre. App fitness, bilance e programmi di allenamento americani usano esclusivamente libbre.

**Bagagli aerei**: Le compagnie aeree americane indicano i limiti bagaglio in libbre. Un limite di 50 libbre equivale a 22,7 kg. Superare il limite può costare caro, quindi è essenziale convertire prima di partire.

**Sollevamento pesi e palestra**: I pesi olimpici americani sono in libbre (45 lb, 35 lb, 25 lb). I record mondiali vengono comunicati in entrambe le unità. Un bilanciere olimpico pesa 45 lb (20,4 kg).

**Spedizioni internazionali**: I corrieri esprimono tariffe in base al peso in kg o lb. Convertire correttamente evita sorprese sul costo finale.

**Neonati e pediatria**: Negli USA il peso dei bambini si misura in libbre e once. Un neonato di 3,5 kg pesa circa 7 lb 11 oz.

### Conversioni Comuni kg-lb

| Chilogrammi | Libbre | Contesto |
|-------------|--------|----------|
| 1 kg | 2,2 lb | Piccolo oggetto |
| 5 kg | 11 lb | Manubrio leggero |
| 10 kg | 22 lb | Bagaglio a mano |
| 20 kg | 44 lb | Valigia standard |
| 50 kg | 110 lb | Persona snella |
| 70 kg | 154 lb | Peso medio uomo |
| 100 kg | 220 lb | Atleta pesante |

### Differenza tra Libbra e Oncia

Nel sistema imperiale, per pesi piccoli si usano le once:
- **1 libbra = 16 once (oz)**
- **1 oncia = 28,35 grammi**

Il peso si esprime spesso come "libbre e once", ad esempio 7 lb 8 oz (sette libbre e otto once). Questo formato è comune per pesare neonati, alimenti e piccoli oggetti.

### Storia della Libbra

Il termine "libbra" deriva dal latino "libra pondo" (bilancia-peso), da cui anche il simbolo "lb". In epoca romana, la libra equivaleva a circa 327 grammi. La libbra moderna inglese fu standardizzata nel 1878 e corrisponde esattamente a 0,45359237 kg per definizione internazionale.

### Peso vs Massa: Chiarimento Scientifico

Tecnicamente, chilogrammi misurano la **massa** mentre le libbre possono misurare sia massa che peso (forza). Nel linguaggio comune si usano intercambiabilmente, ma:

- **Massa (kg)**: quantità di materia, costante ovunque
- **Peso (N o lb-force)**: forza gravitazionale, varia con gravità

Sulla Luna, la tua massa resta 70 kg ma il peso scende a circa 25 lb perché la gravità è minore. Nel nostro convertitore trattiamo libbre come unità di massa terrestre.

## Strumenti Correlati

Potrebbe interessarti anche:
- [Convertitore Grammi Once](/calcolatori/convertitore-grammi-once/) - per pesi piccoli
- [Convertitore Metri Piedi](/calcolatori/convertitore-metri-piedi/) - per altezze
- [Calcolo Percentuale](/calcolatori/calcolo-percentuale/) - calcola variazioni peso
- [Calcolo Sconto](/calcolatori/calcolo-sconto/) - per sconti su prodotti
