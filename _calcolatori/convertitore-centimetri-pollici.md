---
layout: calculator
title: "Convertitore Centimetri Pollici | cm ↔ in Online"
description: "Converti centimetri in pollici e pollici in centimetri. Calcolatore preciso per misure, schermi TV, ruote e dimensioni oggetti."
category: "convertitori-unita"
subcategory: "lunghezza"
related:
  - convertitore-metri-piedi
  - convertitore-chilometri-miglia
  - convertitore-metri-quadri-piedi-quadri
  - calcolo-area-rettangolo
cross_category:
  - calcolo-percentuale
  - calcolo-sconto
---

<div class="calculator-container">
  <h2>Convertitore Centimetri Pollici</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('cm-to-in')">cm → pollici</button>
    <button class="tab-btn" onclick="switchTab('in-to-cm')">pollici → cm</button>
  </div>
  
  <div id="cm-to-in" class="converter-panel active">
    <div class="input-group">
      <label for="cm">Centimetri (cm)</label>
      <input type="number" id="cm" placeholder="Inserisci centimetri" value="50" step="0.1">
    </div>
    
    <button class="btn-calculate" onclick="convertCmToIn()">Converti cm → pollici</button>
    
    <div id="result-cm-in" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-cm-in"></p>
    </div>
  </div>
  
  <div id="in-to-cm" class="converter-panel">
    <div class="input-group">
      <label for="pollici">Pollici (in / ")</label>
      <input type="number" id="pollici" placeholder="Inserisci pollici" value="20" step="0.1">
    </div>
    
    <button class="btn-calculate" onclick="convertInToCm()">Converti pollici → cm</button>
    
    <div id="result-in-cm" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-in-cm"></p>
    </div>
  </div>
</div>

<script>
function switchTab(direction) {
  const tabs = document.querySelectorAll('.tab-btn');
  const panels = document.querySelectorAll('.converter-panel');
  
  tabs.forEach(tab => tab.classList.remove('active'));
  panels.forEach(panel => panel.classList.remove('active'));
  
  if (direction === 'cm-to-in') {
    tabs[0].classList.add('active');
    document.getElementById('cm-to-in').classList.add('active');
  } else {
    tabs[1].classList.add('active');
    document.getElementById('in-to-cm').classList.add('active');
  }
}

function convertCmToIn() {
  const cm = parseFloat(document.getElementById('cm').value);
  
  if (isNaN(cm) || cm < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 cm = 0.393701 pollici
  const pollici = (cm * 0.393701).toFixed(2);
  
  document.getElementById('resultText-cm-in').innerHTML = 
    `<strong>${cm.toFixed(1)} cm</strong> = <strong>${pollici} pollici (in)</strong><br>` +
    `<small>Notazione: ${pollici}"</small><br>` +
    `<small>Fattore: 1 cm = 0.393701 pollici</small>`;
  
  document.getElementById('result-cm-in').style.display = 'block';
}

function convertInToCm() {
  const pollici = parseFloat(document.getElementById('pollici').value);
  
  if (isNaN(pollici) || pollici < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 pollice = 2.54 cm
  const cm = (pollici * 2.54).toFixed(2);
  const mm = (pollici * 25.4).toFixed(1);
  
  document.getElementById('resultText-in-cm').innerHTML = 
    `<strong>${pollici.toFixed(2)} pollici</strong> = <strong>${cm} cm</strong><br>` +
    `<small>Equivale a: ${mm} millimetri</small><br>` +
    `<small>Fattore: 1 pollice = 2.54 cm</small>`;
  
  document.getElementById('result-in-cm').style.display = 'block';
}

window.onload = function() {
  convertCmToIn();
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

## Come Usare il Convertitore Centimetri Pollici

Il nostro **convertitore centimetri pollici** è lo strumento ideale per trasformare misure piccole tra il sistema metrico (centimetri) e il sistema imperiale (pollici). Perfetto per dimensioni di oggetti, schermi, foto, vestiti e componenti tecnici.

### Caratteristiche del Convertitore

- **Conversione bidirezionale**: da cm a pollici e da pollici a cm
- **Precisione al decimo**: risultati accurati per uso tecnico
- **Notazione standard**: mostra anche il simbolo " (pollice)
- **Conversione millimetri**: include anche l'equivalente in mm
- **Interfaccia veloce**: calcolo istantaneo

### Formula di Conversione cm-pollici

La conversione tra centimetri e pollici segue proporzioni matematiche precise:

- **1 centimetro = 0,393701 pollici**
- **1 pollice = 2,54 centimetri esatti**

Il pollice (inch, simbolo ") fa parte del sistema imperiale e corrisponde esattamente a 2,54 cm per definizione internazionale dal 1959.

### Quando Serve Convertire Centimetri in Pollici

Ecco i contesti più comuni dove questa conversione è necessaria:

**Schermi TV e monitor**: Le dimensioni degli schermi si misurano sempre in pollici diagonali. Un TV da 50 pollici ha una diagonale di 127 cm. Quando confronti modelli o scegli la dimensione giusta per la tua stanza, devi convertire da pollici a cm per capire le dimensioni reali.

**Ruote e cerchi auto**: Le dimensioni dei pneumatici e cerchioni si esprimono in pollici. Un cerchio da 17 pollici ha un diametro di circa 43 cm. Questa misura è standard a livello mondiale nel settore automotive.

**Fotografia e stampa**: Le dimensioni delle foto si indicano spesso in pollici: 4×6" (10×15 cm), 5×7" (13×18 cm), 8×10" (20×25 cm). Quando ordini stampe online da siti americani o prepari file per la stampa, serve conoscere le equivalenze.

**Abbigliamento e calzature**: Le taglie americane di vestiti e scarpe usano i pollici. La circonferenza vita, lunghezza pantaloni e numero di scarpe hanno spesso riferimenti in pollici che vanno convertiti per trovare la taglia europea corrispondente.

**Componentistica tecnica**: Viti, bulloni, tubi e molti componenti industriali seguono standard in pollici (frazioni come 1/4", 1/2", 3/4"). Meccanici e tecnici devono saper convertire per usare chiavi e attrezzi corretti.

**Elettronica e rack**: Gli armadi server e i rack audio seguono lo standard da 19 pollici (48,26 cm). Le altezze si misurano in "unità rack" (1U = 1,75 pollici = 4,45 cm).

### Misure TV: Guida alle Dimensioni in Pollici

Ecco una tabella delle diagonali TV più comuni:

| Pollici | Centimetri | Larghezza circa | Ideale per stanza |
|---------|------------|-----------------|-------------------|
| 32" | 81 cm | 71 cm | Camera da letto |
| 40" | 102 cm | 89 cm | Cucina, studio |
| 43" | 109 cm | 96 cm | Soggiorno piccolo |
| 50" | 127 cm | 111 cm | Soggiorno medio |
| 55" | 140 cm | 123 cm | Soggiorno grande |
| 65" | 165 cm | 144 cm | Home theater |
| 75" | 191 cm | 166 cm | Sala ampia |

Ricorda che queste misure si riferiscono alla diagonale dello schermo, non alla larghezza totale. Il TV sarà leggermente più largo e più alto a causa della cornice.

### Conversioni Comuni Centimetri-Pollici

Ecco le equivalenze più utili da conoscere:

| Centimetri | Pollici | Uso Tipico |
|------------|---------|------------|
| 2,54 cm | 1" | Larghezza pollice |
| 5 cm | 2" | Foto tessera |
| 10 cm | 4" | Smartphone piccolo |
| 15 cm | 6" | E-reader, tablet mini |
| 25 cm | 10" | Tablet standard |
| 30 cm | 12" | Laptop piccolo |
| 40 cm | 16" | Cerchione auto |
| 55 cm | 22" | Monitor desktop |

### Il Pollice: Storia e Origine

Il pollice come unità di misura ha origini molto antiche. Il nome deriva dal latino "pollex" (pollice della mano). Tradizionalmente, un pollice corrispondeva alla larghezza del pollice umano alla base dell'unghia.

Nel Medioevo, in Inghilterra, il re Edoardo II standardizzò il pollice come "la lunghezza di tre chicchi d'orzo secchi posti uno accanto all'altro". Nel 1959, i paesi anglofoni hanno adottato il pollice internazionale di esattamente 2,54 cm per uniformare le misure.

Oggi il pollice sopravvive principalmente in tre ambiti: schermi elettronici, pneumatici/cerchi auto e componentistica industriale. In tutti gli altri contesti, il sistema metrico ha sostituito le misure imperiali.

### Frazioni di Pollice: Come Leggerle

Nel sistema imperiale, i pollici si suddividono in frazioni piuttosto che decimali:

- **1/2" = 0,5 pollici = 1,27 cm**
- **1/4" = 0,25 pollici = 0,635 cm**
- **1/8" = 0,125 pollici = 0,317 cm**
- **1/16" = 0,0625 pollici = 0,158 cm**

Queste frazioni sono comuni in falegnameria, meccanica e edilizia americana. Un tubo da "3/4 di pollice" misura 1,905 cm di diametro.

### Confronto Pollice vs Centimetro

Il centimetro fa parte del sistema metrico decimale, logico e coerente: tutto si moltiplica o divide per 10. Il pollice appartiene al sistema imperiale, meno intuitivo ma ancora molto diffuso nei paesi anglofoni per tradizione.

Vantaggi del centimetro:
- Facile da calcolare (base 10)
- Coerente con tutte le altre unità metriche
- Standard scientifico internazionale

Vantaggi del pollice:
- Frazioni semplici (1/2, 1/4, 1/8)
- Standard consolidato in alcuni settori
- Misura umana (larghezza pollice)

## Strumenti Correlati

Potrebbe interessarti anche:
- [Convertitore Metri Piedi](/calcolatori/convertitore-metri-piedi/) - per lunghezze maggiori
- [Convertitore Chilometri Miglia](/calcolatori/convertitore-chilometri-miglia/) - per distanze lunghe
- [Calcolo Area Rettangolo](/calcolatori/calcolo-area-rettangolo/) - calcola superfici
- [Calcolo Percentuale](/calcolatori/calcolo-percentuale/) - calcoli percentuali
