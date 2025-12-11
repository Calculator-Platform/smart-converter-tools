---
layout: calculator
title: "Convertitore Chilometri Miglia | km ↔ mi Online"
description: "Converti chilometri in miglia e viceversa con il nostro calcolatore gratuito. Conversione istantanea km-mi per viaggi, sport e distanze."
category: "convertitori-unita"
subcategory: "lunghezza"
related:
  - convertitore-metri-piedi
  - convertitore-centimetri-pollici
  - convertitore-metri-quadri-piedi-quadri
  - calcolo-percentuale
cross_category:
  - calcolo-area-rettangolo
  - calcolo-sconto
---

<div class="calculator-container">
  <h2>Convertitore Chilometri Miglia</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('km-to-mi')">km → mi</button>
    <button class="tab-btn" onclick="switchTab('mi-to-km')">mi → km</button>
  </div>
  
  <div id="km-to-mi" class="converter-panel active">
    <div class="input-group">
      <label for="km">Chilometri (km)</label>
      <input type="number" id="km" placeholder="Inserisci chilometri" value="10" step="0.01">
    </div>
    
    <button class="btn-calculate" onclick="convertKmToMi()">Converti km → mi</button>
    
    <div id="result-km-mi" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-km-mi"></p>
    </div>
  </div>
  
  <div id="mi-to-km" class="converter-panel">
    <div class="input-group">
      <label for="mi">Miglia (mi)</label>
      <input type="number" id="mi" placeholder="Inserisci miglia" value="10" step="0.01">
    </div>
    
    <button class="btn-calculate" onclick="convertMiToKm()">Converti mi → km</button>
    
    <div id="result-mi-km" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-mi-km"></p>
    </div>
  </div>
</div>

<script>
function switchTab(direction) {
  const tabs = document.querySelectorAll('.tab-btn');
  const panels = document.querySelectorAll('.converter-panel');
  
  tabs.forEach(tab => tab.classList.remove('active'));
  panels.forEach(panel => panel.classList.remove('active'));
  
  if (direction === 'km-to-mi') {
    tabs[0].classList.add('active');
    document.getElementById('km-to-mi').classList.add('active');
  } else {
    tabs[1].classList.add('active');
    document.getElementById('mi-to-km').classList.add('active');
  }
}

function convertKmToMi() {
  const km = parseFloat(document.getElementById('km').value);
  
  if (isNaN(km) || km < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 km = 0.621371 miglia
  const miglia = (km * 0.621371).toFixed(2);
  
  document.getElementById('resultText-km-mi').innerHTML = 
    `<strong>${km.toFixed(2)} km</strong> = <strong>${miglia} mi</strong><br>` +
    `<small>Fattore di conversione: 1 km = 0.621371 miglia</small>`;
  
  document.getElementById('result-km-mi').style.display = 'block';
}

function convertMiToKm() {
  const mi = parseFloat(document.getElementById('mi').value);
  
  if (isNaN(mi) || mi < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 miglio = 1.60934 km
  const km = (mi * 1.60934).toFixed(2);
  
  document.getElementById('resultText-mi-km').innerHTML = 
    `<strong>${mi.toFixed(2)} mi</strong> = <strong>${km} km</strong><br>` +
    `<small>Fattore di conversione: 1 miglio = 1.60934 km</small>`;
  
  document.getElementById('result-mi-km').style.display = 'block';
}

// Calcola automaticamente al caricamento
window.onload = function() {
  convertKmToMi();
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

## Come Usare il Convertitore Chilometri Miglia

Il nostro **convertitore chilometri miglia** ti permette di trasformare istantaneamente distanze tra il sistema metrico (chilometri) e il sistema imperiale (miglia). Lo strumento è bidirezionale: puoi convertire sia da km a miglia che da miglia a km con un solo clic.

### Caratteristiche del Convertitore

- **Conversione bidirezionale**: passa facilmente da km a mi e viceversa con i tab in alto
- **Precisione elevata**: risultati accurati fino a due cifre decimali
- **Calcolo istantaneo**: ottieni il risultato in tempo reale mentre digiti
- **Completamente gratuito**: nessuna registrazione o download richiesto
- **Mobile-friendly**: funziona perfettamente su smartphone e tablet

### Come Funziona la Conversione km-mi

La conversione tra chilometri e miglia si basa su fattori matematici fissi:

- **1 chilometro = 0.621371 miglia**
- **1 miglio = 1.60934 chilometri**

Questi rapporti derivano dalla definizione internazionale delle unità di misura: il miglio terrestre (statute mile) misura esattamente 1.609,344 metri, mentre il chilometro corrisponde a 1.000 metri.

### Quando Serve Convertire Chilometri in Miglia

Ecco le situazioni più comuni in cui risulta utile questo convertitore:

**Viaggi internazionali**: Se visiti paesi che usano il sistema imperiale come Stati Uniti, Regno Unito o Canada, dovrai convertire le distanze per capire quanto sono lontane le destinazioni. Un cartello stradale che indica 50 miglia equivale a circa 80 chilometri.

**Sport e fitness**: Nel running e ciclismo, molte gare internazionali usano le miglia (specialmente negli USA). Una maratona è 26,2 miglia, che corrispondono a 42,195 km. Se ti alleni seguendo piani americani, dovrai convertire le distanze.

**Acquisto auto importate**: Le auto americane mostrano il contachilometri in miglia. Se importi un veicolo dagli Stati Uniti con 50.000 miglia, significa che ha percorso circa 80.500 km.

**Navigazione aerea e marittima**: Anche se l'aviazione usa principalmente le miglia nautiche (diverse dalle miglia terrestri), per comunicare con passeggeri non esperti le distanze vengono spesso espresse in miglia o chilometri standard.

**Dati scientifici e storici**: Molti documenti, mappe e pubblicazioni anglosassoni riportano distanze in miglia. Per confrontarle con dati europei serve la conversione.

### Differenza tra Miglia Terrestri e Miglia Nautiche

È importante distinguere due tipi di miglia:

**Miglio terrestre (statute mile)**: È il miglio usato su strada, pari a 1,609 km. È quello che vedi sui cartelli stradali negli USA e UK.

**Miglio nautico (nautical mile)**: Usato in navigazione marittima e aerea, equivale a 1,852 km. È leggermente più lungo perché basato sulla circonferenza terrestre.

Il nostro convertitore utilizza il **miglio terrestre**, quello più comune per distanze stradali e sport.

### Esempi Pratici di Conversione

Ecco alcune conversioni utili da memorizzare:

- **5 km = 3,1 miglia** (distanza tipica corsa amatoriale)
- **10 km = 6,2 miglia** (gara podistica molto popolare)
- **21 km = 13,1 miglia** (mezza maratona)
- **42 km = 26,2 miglia** (maratona completa)
- **100 km = 62,1 miglia** (ultramaratona)
- **160 km = 99,4 miglia** (circa 100 miglia)

### Tabella Rapida di Conversione

| Chilometri | Miglia | Uso Comune |
|------------|--------|------------|
| 1 km | 0,62 mi | Breve passeggiata |
| 5 km | 3,1 mi | Corsa fitness |
| 10 km | 6,2 mi | Gara podistica |
| 21 km | 13,1 mi | Mezza maratona |
| 42 km | 26,2 mi | Maratona |
| 100 km | 62 mi | Ultramaratona |
| 160 km | 100 mi | Century ride (ciclismo) |

### Perché Stati Uniti e UK Usano le Miglia

Il sistema imperiale, che include le miglia, è ancora in uso negli Stati Uniti e parzialmente nel Regno Unito per ragioni storiche. Mentre la maggior parte del mondo ha adottato il sistema metrico decimale (più semplice e coerente), alcuni paesi anglosassoni mantengono le vecchie unità di misura per tradizione e per il costo elevato di convertire tutta la segnaletica stradale.

Il Regno Unito è in una situazione ibrida: usa miglia per le distanze stradali ma litri per i carburanti e metri per molte altre misurazioni.

## Strumenti Correlati

Potrebbe interessarti anche:
- [Convertitore Metri Piedi](/calcolatori/convertitore-metri-piedi/) - conversione altezze e lunghezze brevi
- [Convertitore Centimetri Pollici](/calcolatori/convertitore-centimetri-pollici/) - misure piccole cm↔in
- [Calcolo Percentuale](/calcolatori/calcolo-percentuale/) - calcola aumenti e riduzioni percentuali
