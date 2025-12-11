---
layout: calculator
title: "Convertitore Metri Piedi | m ↔ ft Online Gratis"
description: "Converti metri in piedi e piedi in metri. Calcolatore preciso per altezze, distanze e misure. Conversione m-ft istantanea."
category: "convertitori-unita"
subcategory: "lunghezza"
related:
  - convertitore-chilometri-miglia
  - convertitore-centimetri-pollici
  - convertitore-metri-quadri-piedi-quadri
  - calcolo-area-rettangolo
cross_category:
  - calcolo-percentuale
  - calcolo-sconto
---

<div class="calculator-container">
  <h2>Convertitore Metri Piedi</h2>
  
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('m-to-ft')">m → ft</button>
    <button class="tab-btn" onclick="switchTab('ft-to-m')">ft → m</button>
  </div>
  
  <div id="m-to-ft" class="converter-panel active">
    <div class="input-group">
      <label for="metri">Metri (m)</label>
      <input type="number" id="metri" placeholder="Inserisci metri" value="1.80" step="0.01">
    </div>
    
    <button class="btn-calculate" onclick="convertMToFt()">Converti m → ft</button>
    
    <div id="result-m-ft" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-m-ft"></p>
    </div>
  </div>
  
  <div id="ft-to-m" class="converter-panel">
    <div class="input-group">
      <label for="piedi">Piedi (ft)</label>
      <input type="number" id="piedi" placeholder="Inserisci piedi" value="6" step="0.01">
    </div>
    
    <button class="btn-calculate" onclick="convertFtToM()">Converti ft → m</button>
    
    <div id="result-ft-m" class="result" style="display:none;">
      <h3>Risultato:</h3>
      <p id="resultText-ft-m"></p>
    </div>
  </div>
</div>

<script>
function switchTab(direction) {
  const tabs = document.querySelectorAll('.tab-btn');
  const panels = document.querySelectorAll('.converter-panel');
  
  tabs.forEach(tab => tab.classList.remove('active'));
  panels.forEach(panel => panel.classList.remove('active'));
  
  if (direction === 'm-to-ft') {
    tabs[0].classList.add('active');
    document.getElementById('m-to-ft').classList.add('active');
  } else {
    tabs[1].classList.add('active');
    document.getElementById('ft-to-m').classList.add('active');
  }
}

function convertMToFt() {
  const metri = parseFloat(document.getElementById('metri').value);
  
  if (isNaN(metri) || metri < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 metro = 3.28084 piedi
  const piedi = (metri * 3.28084).toFixed(2);
  
  // Calcola anche piedi e pollici separati
  const ft = Math.floor(piedi);
  const inches = Math.round((piedi - ft) * 12);
  
  document.getElementById('resultText-m-ft').innerHTML = 
    `<strong>${metri.toFixed(2)} m</strong> = <strong>${piedi} ft</strong><br>` +
    `<small>Equivale a: ${ft} piedi e ${inches} pollici (${ft}'${inches}")</small><br>` +
    `<small>Fattore: 1 metro = 3.28084 piedi</small>`;
  
  document.getElementById('result-m-ft').style.display = 'block';
}

function convertFtToM() {
  const piedi = parseFloat(document.getElementById('piedi').value);
  
  if (isNaN(piedi) || piedi < 0) {
    alert('Inserisci un valore valido');
    return;
  }
  
  // 1 piede = 0.3048 metri
  const metri = (piedi * 0.3048).toFixed(2);
  const cm = (piedi * 30.48).toFixed(0);
  
  document.getElementById('resultText-ft-m').innerHTML = 
    `<strong>${piedi.toFixed(2)} ft</strong> = <strong>${metri} m</strong><br>` +
    `<small>Equivale a: ${cm} centimetri</small><br>` +
    `<small>Fattore: 1 piede = 0.3048 metri</small>`;
  
  document.getElementById('result-ft-m').style.display = 'block';
}

window.onload = function() {
  convertMToFt();
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

## Come Usare il Convertitore Metri Piedi

Il nostro **convertitore metri piedi** è lo strumento perfetto per trasformare misure di altezza e lunghezza tra il sistema metrico (metri) e il sistema imperiale (piedi). La conversione è bidirezionale e include anche la suddivisione in piedi e pollici per maggiore precisione.

### Funzionalità Principali

- **Doppia conversione**: passa da metri a piedi e viceversa con un clic
- **Formato piedi-pollici**: oltre ai piedi decimali, mostra anche il formato tradizionale (es: 5'11")
- **Alta precisione**: calcoli accurati per uso professionale e personale
- **Interfaccia intuitiva**: risultati chiari e immediati
- **Responsive**: funziona su qualsiasi dispositivo

### Formula di Conversione Metro-Piede

La conversione tra metri e piedi si basa su equivalenze matematiche precise:

- **1 metro = 3,28084 piedi**
- **1 piede = 0,3048 metri = 30,48 centimetri**

Queste proporzioni derivano dalla definizione internazionale del metro (basato sulla velocità della luce) e del piede inglese (foot), standardizzato a 12 pollici.

### Quando Serve Convertire Metri in Piedi

Ecco i casi d'uso più frequenti per questo tipo di conversione:

**Altezza delle persone**: Negli Stati Uniti, Regno Unito e altri paesi anglofoni, l'altezza si misura in piedi e pollici. Se sei alto 1,80 m, corrispondi a circa 5 piedi e 11 pollici (5'11"). Questo è fondamentale per documenti, profili online o conversazioni con persone che usano il sistema imperiale.

**Immobili e architettura**: Le planimetrie americane riportano dimensioni in piedi. Una stanza di 4 metri per 5 metri corrisponde a circa 13 ft × 16 ft. Architetti e interior designer devono saper convertire rapidamente tra i due sistemi quando lavorano con progetti internazionali.

**Sport**: In discipline come il salto in alto, salto con l'asta e lancio del peso, i record mondiali vengono spesso comunicati in piedi oltre che in metri. Il record del salto in alto maschile è 2,45 m, pari a 8 piedi e 0,5 pollici.

**Aviazione**: L'altitudine degli aerei viene misurata in piedi in quasi tutto il mondo. Un volo a crociera a 10.000 metri corrisponde a circa 32.800 piedi, solitamente arrotondati a 33.000 ft.

**Nautica e subacquea**: Le profondità marine si esprimono spesso in piedi, specialmente in ambito subacqueo ricreativo. Una immersione a 18 metri (limite per Open Water Diver) corrisponde a circa 60 piedi.

### Sistema Piedi-Pollici: Come Funziona

Nel sistema imperiale, le misure inferiori ai 10-12 piedi si esprimono spesso come combinazione di piedi e pollici:

- **1 piede = 12 pollici (inches)**
- Notazione: 5'11" significa 5 piedi e 11 pollici
- L'altezza media italiana maschile (1,77 m) equivale a 5'9,5"
- L'altezza media femminile italiana (1,65 m) equivale a 5'5"

Il nostro convertitore mostra automaticamente questa suddivisione quando converti da metri a piedi, rendendo più facile comunicare altezze nel formato americano tradizionale.

### Conversioni Comuni Metri-Piedi

Ecco una tabella con le equivalenze più utili:

| Metri | Piedi | Piedi-Pollici | Uso Tipico |
|-------|-------|---------------|------------|
| 1,50 m | 4,92 ft | 4'11" | Altezza bambino |
| 1,65 m | 5,41 ft | 5'5" | Altezza media donna |
| 1,75 m | 5,74 ft | 5'9" | Altezza media uomo |
| 1,80 m | 5,91 ft | 5'11" | Altezza sopra media |
| 2,00 m | 6,56 ft | 6'7" | Altezza giocatore basket |
| 3,00 m | 9,84 ft | 9'10" | Altezza soffitto |
| 10,00 m | 32,81 ft | 32'10" | Altezza edificio 3 piani |

### Differenze tra Piede Internazionale e Piede Survey USA

Esistono due definizioni leggermente diverse di piede:

**International foot** (piede internazionale): 0,3048 metri esatti, usato nella maggior parte del mondo e negli standard scientifici. È quello utilizzato dal nostro convertitore.

**US survey foot** (piede catastale USA): 0,30480061 metri, usato in alcune applicazioni di geodesia e cartografia negli Stati Uniti. La differenza è minima (2 parti per milione) ma può accumularsi su grandi distanze.

Per la stragrande maggioranza degli usi quotidiani, questa distinzione è irrilevante. Solo in contesti di misurazione territoriale ad alta precisione è necessario specificare quale definizione si sta usando.

### Curiosità sul Piede come Unità di Misura

Il piede ha origini antichissime: deriva letteralmente dalla lunghezza media del piede umano. Nel corso dei secoli, ogni paese aveva la propria versione:

- **Piede romano**: circa 29,6 cm
- **Piede inglese**: 30,48 cm (quello moderno)
- **Piede di Parigi**: 32,5 cm
- **Piede veneziano**: 34,8 cm

Nel 1959, paesi anglofoni hanno standardizzato il piede internazionale a esattamente 0,3048 metri per eliminare confusione nelle misurazioni internazionali.

## Strumenti Correlati

Potrebbe interessarti anche:
- [Convertitore Centimetri Pollici](/calcolatori/convertitore-centimetri-pollici/) - per misure più piccole
- [Convertitore Chilometri Miglia](/calcolatori/convertitore-chilometri-miglia/) - per distanze lunghe
- [Convertitore Metri Quadri Piedi Quadri](/calcolatori/convertitore-metri-quadri-piedi-quadri/) - per superfici
- [Calcolo Area Rettangolo](/calcolatori/calcolo-area-rettangolo/) - calcola aree in m² o ft²
