---
layout: calculator
title: "Convertitore Centimetri Pollici  |  cm ↔ inch  |  Online Gratis"
description: "Converti centimetri in pollici e pollici in cm istantaneamente. Calcolatore gratuito con tabella di conversione rapida."
category: "convertitori-unita"
subcategory: "lunghezza"
---

<div class="page-hero">
  <div class="hero-icon">📱</div>
  <h1>Convertitore Centimetri Pollici</h1>
  <p>Converti velocemente tra cm e pollici</p>
</div>

<!-- ADV SPOT 1: Banner principale above fold -->
<div class="ad-container ad-primary">
  <span class="ad-label">Pubblicità</span>
  <div class="ad-placeholder ad-main">
    <span class="ad-text">Banner 336×280</span>
  </div>
</div>

<div class="calculator-box">
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('cm-to-in')"><span class="tab-label">Centimetri → Pollici</span></button>
    <button class="tab-btn" onclick="switchTab('in-to-cm')"><span class="tab-label">Pollici → Centimetri</span></button>
  </div>
  
  <div id="cm-to-in" class="converter-panel active">
    <div class="input-wrapper"><label for="cm-input">Centimetri (cm)</label><input type="number" id="cm-input" placeholder="Inserisci valore" step="0.01" min="0"></div>
    <button class="calc-button" onclick="convertCmToIn()"><span class="button-icon">⚡</span>Converti in Pollici</button>
    <div id="cm-result" class="result-box"></div>
  </div>
  
  <div id="in-to-cm" class="converter-panel">
    <div class="input-wrapper"><label for="in-input">Pollici (inch)</label><input type="number" id="in-input" placeholder="Inserisci valore" step="0.01" min="0"></div>
    <button class="calc-button" onclick="convertInToCm()"><span class="button-icon">⚡</span>Converti in Centimetri</button>
    <div id="in-result" class="result-box"></div>
  </div>
</div>

<!-- ADV SPOT 2: Banner secondario dopo calculator -->
<div class="ad-container ad-secondary">
  <span class="ad-label">Pubblicità</span>
  <div class="ad-placeholder ad-second">
    <span class="ad-text">Banner 728×90</span>
  </div>
</div>

<script>
function switchTab(d){const k=document.getElementById('cm-to-in');const m=document.getElementById('in-to-cm');const b=document.querySelectorAll('.tab-btn');if(d==='cm-to-in'){k.classList.add('active');m.classList.remove('active');b[0].classList.add('active');b[1].classList.remove('active')}else{m.classList.add('active');k.classList.remove('active');b[1].classList.add('active');b[0].classList.remove('active')}}
function convertCmToIn(){const cm=parseFloat(document.getElementById('cm-input').value);const r=document.getElementById('cm-result');if(isNaN(cm)||cm<0){r.innerHTML='<div class="error-message">⚠️ Inserisci un numero valido</div>';return}const inch=cm*0.393701;r.innerHTML=`<div class="result-success"><div class="result-main">${cm.toFixed(2)} cm = <strong>${inch.toFixed(2)} pollici</strong></div></div>`}
function convertInToCm(){const inch=parseFloat(document.getElementById('in-input').value);const r=document.getElementById('in-result');if(isNaN(inch)||inch<0){r.innerHTML='<div class="error-message">⚠️ Inserisci un numero valido</div>';return}const cm=inch*2.54;r.innerHTML=`<div class="result-success"><div class="result-main">${inch.toFixed(2)} inch = <strong>${cm.toFixed(2)} centimetri</strong></div></div>`}
window.addEventListener('load',function(){document.getElementById('cm-input').value='10';convertCmToIn()});
</script>

<div class="content-section">
<h2>Come usare il convertitore centimetri pollici</h2>
<p>Questo strumento ti permette di convertire facilmente tra centimetri e pollici in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.</p>

<h3>Quando serve convertire centimetri in pollici</h3>
<p>La conversione tra centimetri e pollici è essenziale per misure di schermi TV e monitor, dove le dimensioni sono sempre espresse in pollici. Anche nel settore dell'abbigliamento, molti capi importati utilizzano taglie in pollici che necessitano conversione. Per progetti di fai-da-te e bricolage con materiali provenienti da paesi che usano il sistema imperiale, questa conversione è indispensabile.</p>

<p>Chi lavora con design grafico e stampa deve spesso convertire tra centimetri e pollici per adattare i progetti a standard internazionali. Anche per l'altezza delle persone, alcuni paesi esprimono la statura in piedi e pollici anziché in centimetri.</p>

<h3>Formula di conversione</h3>
<p><strong>Da centimetri a pollici:</strong> 1 cm = 0.393701 pollici<br>
<strong>Da pollici a centimetri:</strong> 1 pollice = 2.54 cm</p>

<p>La conversione è basata sulla definizione internazionale che stabilisce esattamente 1 pollice = 2.54 centimetri. Questa definizione è stata fissata nel 1959 ed è utilizzata in tutto il mondo per garantire uniformità nelle misurazioni.</p>

<h3>Tabella conversione rapida cm - pollici</h3>
<div class="conversion-table">
<table>
<tr><th>Centimetri</th><th>Pollici</th><th></th><th>Pollici</th><th>Centimetri</th></tr>
<tr><td>1 cm</td><td>0.39 in</td><td></td><td>1 in</td><td>2.54 cm</td></tr>
<tr><td>5 cm</td><td>1.97 in</td><td></td><td>5 in</td><td>12.70 cm</td></tr>
<tr><td>10 cm</td><td>3.94 in</td><td></td><td>10 in</td><td>25.40 cm</td></tr>
<tr><td>20 cm</td><td>7.87 in</td><td></td><td>20 in</td><td>50.80 cm</td></tr>
<tr><td>50 cm</td><td>19.69 in</td><td></td><td>50 in</td><td>127.00 cm</td></tr>
<tr><td>100 cm</td><td>39.37 in</td><td></td><td>100 in</td><td>254.00 cm</td></tr>
</table>
</div>
</div>

<div class="related-tools">
<h3>Convertitori correlati</h3>
<div class="related-grid">
<a href="/smart-converter-tools/calcolatori/convertitore-metri-piedi/" class="related-card"><span class="related-icon">📐</span><span class="related-title">Metri ↔ Piedi</span></a>
<a href="/smart-converter-tools/calcolatori/convertitore-chilometri-miglia/" class="related-card"><span class="related-icon">🚗</span><span class="related-title">Km ↔ Miglia</span></a>
<a href="/smart-converter-tools/calcolatori/convertitore-chilogrammi-libbre/" class="related-card"><span class="related-icon">⚖️</span><span class="related-title">Kg ↔ Libbre</span></a>
</div>
</div>

<style>
:root{--primary-purple:#667eea;--primary-purple-dark:#764ba2;--accent-green:#10b981;--gray-50:#f7fafc;--gray-100:#edf2f7;--gray-200:#e2e8f0;--gray-300:#cbd5e0;--gray-400:#a0aec0;--gray-600:#4a5568;--gray-700:#2d3748;--gray-800:#1a202c}

.page-hero{background:linear-gradient(135deg,#667eea 0%,#764ba2 50%,#f093fb 100%);padding:1.25rem 1rem;text-align:center;margin:0 -1.5rem 1.5rem -1.5rem;box-shadow:0 4px 20px rgba(102,126,234,0.3)}
.hero-icon{font-size:2.5rem;margin-bottom:0.5rem}
.page-hero h1{color:white;font-size:1.5rem;font-weight:700;margin:0 0 0.4rem 0;line-height:1.2}
.page-hero p{color:white;font-size:0.9rem;margin:0;opacity:0.95}
.calculator-box{background:white;border:2px solid var(--gray-200);border-radius:12px;padding:1.25rem;box-shadow:0 4px 16px rgba(0,0,0,0.08);max-width:600px;margin:0 auto 1.5rem}
.converter-tabs{display:grid;grid-template-columns:1fr 1fr;gap:0.4rem;margin-bottom:1.25rem}
.tab-btn{background:var(--gray-50);border:2px solid var(--gray-200);border-radius:8px;padding:0.65rem 0.5rem;cursor:pointer;font-family:'Montserrat',sans-serif;font-size:0.85rem;font-weight:600;color:var(--gray-600);transition:all 0.3s;position:relative;overflow:hidden}
.tab-btn::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,var(--primary-purple),var(--accent-green));transform:scaleX(0);transition:transform 0.3s}
.tab-btn.active::before{transform:scaleX(1)}
.tab-btn.active{background:white;border-color:var(--primary-purple);color:var(--primary-purple)}
.tab-label{display:block;text-align:center}
.converter-panel{display:none}
.converter-panel.active{display:block}
.input-wrapper{margin-bottom:0.9rem}
.input-wrapper label{display:block;color:var(--gray-700);font-size:0.85rem;font-weight:600;margin-bottom:0.4rem;text-align:center}
.input-wrapper input{width:100%;padding:0.9rem;font-size:1rem;font-family:'Montserrat',sans-serif;font-weight:500;text-align:center;border:2px solid var(--gray-200);border-radius:8px;background:var(--gray-50);color:var(--gray-800);transition:all 0.3s;min-height:48px}
.input-wrapper input:focus{outline:none;border-color:var(--primary-purple);background:white;box-shadow:0 0 0 3px rgba(102,126,234,0.1)}
.calc-button{width:100%;padding:1rem;font-size:1rem;font-weight:700;font-family:'Montserrat',sans-serif;color:white;background:linear-gradient(135deg,var(--primary-purple) 0%,var(--primary-purple-dark) 100%);border:none;border-radius:8px;cursor:pointer;transition:all 0.3s;box-shadow:0 4px 12px rgba(102,126,234,0.3);display:flex;align-items:center;justify-content:center;gap:0.5rem;margin-bottom:0.9rem;min-height:52px}
.calc-button:hover{transform:translateY(-2px);box-shadow:0 6px 18px rgba(102,126,234,0.4)}
.button-icon{font-size:1.1rem}
.result-box{min-height:55px;display:flex;align-items:center;justify-content:center}
.result-success{background:linear-gradient(135deg,#ecfdf5 0%,#d1fae5 100%);border:2px solid var(--accent-green);border-radius:8px;padding:0.9rem;text-align:center;animation:slideIn 0.3s ease}
.result-main{color:var(--gray-800);font-size:1rem}
.result-main strong{color:var(--accent-green);font-weight:700}
.error-message{background:#fef2f2;border:2px solid #fca5a5;border-radius:8px;padding:0.9rem;color:#991b1b;text-align:center;font-weight:600}
@keyframes slideIn{from{opacity:0;transform:translateY(-8px)}to{opacity:1;transform:translateY(0)}}

.content-section{margin:1.5rem auto;line-height:1.7;max-width:800px}
.content-section h2{color:var(--gray-800);font-size:1.3rem;font-weight:700;margin-bottom:0.8rem;padding-bottom:0.4rem;border-bottom:3px solid var(--primary-purple);display:inline-block}
.content-section h3{color:var(--gray-700);font-size:1.1rem;font-weight:600;margin:1.2rem 0 0.6rem}
.content-section p{color:var(--gray-600);margin-bottom:0.9rem;font-size:0.95rem}

.conversion-table{overflow-x:auto;margin:1rem 0}
.conversion-table table{width:100%;border-collapse:collapse;background:white;border:2px solid var(--gray-200);border-radius:8px}
.conversion-table th{background:var(--primary-purple);color:white;padding:0.75rem;font-weight:600;font-size:0.9rem}
.conversion-table td{padding:0.65rem;border-bottom:1px solid var(--gray-200);color:var(--gray-700);font-size:0.9rem;text-align:center}
.conversion-table tr:last-child td{border-bottom:none}
.conversion-table tr:nth-child(even){background:var(--gray-50)}

.related-tools{margin:2rem auto;max-width:800px}
.related-tools h3{color:var(--gray-800);font-size:1.2rem;font-weight:700;margin-bottom:0.9rem}
.related-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:0.8rem}
.related-card{background:white;border:2px solid var(--gray-200);border-radius:10px;padding:0.9rem;text-decoration:none;display:flex;align-items:center;gap:0.65rem;transition:all 0.3s}
.related-card:hover{border-color:var(--primary-purple);transform:translateY(-2px);box-shadow:0 6px 12px rgba(102,126,234,0.15)}
.related-icon{font-size:1.6rem;flex-shrink:0}
.related-title{color:var(--gray-700);font-weight:600;font-size:0.9rem}

.ad-container{display:flex;flex-direction:column;align-items:center;margin:1.25rem auto;max-width:100%}
.ad-primary{margin:1.25rem auto 1.5rem}
.ad-secondary{margin:1.5rem auto}
.ad-label{font-size:0.65rem;color:var(--gray-400);text-transform:uppercase;letter-spacing:0.05em;margin-bottom:0.4rem;font-weight:600}
.ad-placeholder{background:linear-gradient(135deg,var(--gray-50) 0%,var(--gray-100) 100%);border:2px dashed var(--gray-300);border-radius:8px;display:flex;align-items:center;justify-content:center}

.ad-main{width:336px;height:280px;max-width:100%}
.ad-second{width:728px;height:90px;max-width:100%}
.ad-text{color:var(--gray-400);font-size:0.8rem;font-weight:500}

@media (max-width:768px){
.page-hero{padding:1rem 0.8rem;margin:0 -1rem 1.25rem -1rem}
.hero-icon{font-size:2.2rem}
.page-hero h1{font-size:1.35rem}
.page-hero p{font-size:0.85rem}
.calculator-box{padding:1rem}
.related-grid{grid-template-columns:1fr}
.ad-main{width:300px;height:250px}
.ad-second{width:300px;height:250px}
}
</style>
