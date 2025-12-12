---
layout: calculator
title: "Convertitore Grammi Once  |  g ↔ oz  |  Online Gratis"
description: "Converti grammi in once e once in grammi istantaneamente. Calcolatore gratuito con tabella di conversione rapida."
category: "convertitori-unita"
subcategory: "peso"
---

<div class="page-hero">
  <div class="hero-icon">🍳</div>
  <h1>Convertitore Grammi Once</h1>
  <p>Converti velocemente tra grammi e once</p>
</div>

<!-- ADV SPOT 1: Banner principale above fold -->
<div class="ad-container ad-primary">
  <div class="ad-placeholder ad-main">
    <span class="ad-text">Banner 728×90</span>
  </div>
<div class="calculator-box">
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('g-to-oz')"><span class="tab-label">Grammi → Once</span></button>
    <button class="tab-btn" onclick="switchTab('oz-to-g')"><span class="tab-label">Once → Grammi</span></button>
  </div>
  
  <div id="g-to-oz" class="converter-panel active">
    <div class="input-wrapper"><label for="g-input">Grammi (g)</label><input type="number" id="g-input" placeholder="Inserisci valore" step="0.01" min="0"></div>
    <button class="calc-button" onclick="convertGToOz()"><span class="button-icon">⚡</span>Converti in Once</button>
    <div id="g-result" class="result-box"></div>
  </div>
  
  <div id="oz-to-g" class="converter-panel">
    <div class="input-wrapper"><label for="oz-input">Once (oz)</label><input type="number" id="oz-input" placeholder="Inserisci valore" step="0.01" min="0"></div>
    <button class="calc-button" onclick="convertOzToG()"><span class="button-icon">⚡</span>Converti in Grammi</button>
    <div id="oz-result" class="result-box"></div>
  </div>
</div>

<!-- ADV SPOT 2: Banner secondario dopo calculator -->
<div class="ad-container ad-secondary">
  <div class="ad-placeholder ad-second">
    <span class="ad-text">Banner 728×90</span>
  </div>

<script>
function switchTab(d){const k=document.getElementById('g-to-oz');const m=document.getElementById('oz-to-g');const b=document.querySelectorAll('.tab-btn');if(d==='g-to-oz'){k.classList.add('active');m.classList.remove('active');b[0].classList.add('active');b[1].classList.remove('active')}else{m.classList.add('active');k.classList.remove('active');b[1].classList.add('active');b[0].classList.remove('active')}}
function convertGToOz(){const g=parseFloat(document.getElementById('g-input').value);const r=document.getElementById('g-result');if(isNaN(g)||g<0){r.innerHTML='<div class="error-message">⚠️ Inserisci un numero valido</div>';return}const oz=g*0.035274;r.innerHTML=`<div class="result-success"><div class="result-main">${g.toFixed(2)} g = <strong>${oz.toFixed(2)} once</strong></div></div>`}
function convertOzToG(){const oz=parseFloat(document.getElementById('oz-input').value);const r=document.getElementById('oz-result');if(isNaN(oz)||oz<0){r.innerHTML='<div class="error-message">⚠️ Inserisci un numero valido</div>';return}const g=oz*28.3495;r.innerHTML=`<div class="result-success"><div class="result-main">${oz.toFixed(2)} oz = <strong>${g.toFixed(2)} grammi</strong></div></div>`}
window.addEventListener('load',function(){document.getElementById('g-input').value='100';convertGToOz()});
</script>

<div class="content-section">
<h2>Come usare il convertitore grammi once</h2>
<p>Questo strumento ti permette di convertire facilmente tra grammi e once in entrambe le direzioni. Seleziona la direzione di conversione usando le tab in alto, inserisci il valore e premi "Converti". Il risultato viene mostrato istantaneamente con precisione di due decimali.</p>

<h3>Quando serve convertire grammi in once</h3>
<p>La conversione tra grammi e once è fondamentale in cucina quando si seguono ricette americane o britanniche. Le ricette di pasticceria richiedono particolare precisione nelle dosi, e molte sono scritte in once. Anche per il dosaggio di integratori alimentari e prodotti nutrizionali, le etichette spesso riportano informazioni in once.</p>

<p>Nel settore dei preziosi, l'oro e l'argento vengono pesati in once troy (leggermente diverse dalle once standard). Per la spedizione di piccoli pacchi internazionali, conoscere il peso in once può essere utile per calcolare i costi verso destinazioni che usano il sistema imperiale.</p>

<h3>Formula di conversione</h3>
<p><strong>Da grammi a once:</strong> 1 g = 0.035274 once<br>
<strong>Da once a grammi:</strong> 1 oncia = 28.3495 g</p>

<p>La conversione si basa sulla definizione internazionale che stabilisce 1 oncia (ounce) pari a esattamente 28.349523125 grammi. Questo valore è parte del sistema avoirdupois, lo standard più comune per pesare alimenti e oggetti di uso quotidiano.</p>

<h3>Tabella conversione rapida grammi - once</h3>
<div class="conversion-table">
<table>
<tr><th>Grammi</th><th>Once</th><th></th><th>Once</th><th>Grammi</th></tr>
<tr><td>10 g</td><td>0.35 oz</td><td></td><td>1 oz</td><td>28.35 g</td></tr>
<tr><td>50 g</td><td>1.76 oz</td><td></td><td>2 oz</td><td>56.70 g</td></tr>
<tr><td>100 g</td><td>3.53 oz</td><td></td><td>4 oz</td><td>113.40 g</td></tr>
<tr><td>250 g</td><td>8.82 oz</td><td></td><td>8 oz</td><td>226.80 g</td></tr>
<tr><td>500 g</td><td>17.64 oz</td><td></td><td>16 oz</td><td>453.59 g</td></tr>
<tr><td>1000 g</td><td>35.27 oz</td><td></td><td>32 oz</td><td>907.18 g</td></tr>
</table>
</div>
</div>

<div class="related-tools">
<h3>Convertitori correlati</h3>
<div class="related-grid">
<a href="/smart-converter-tools/calcolatori/convertitore-chilogrammi-libbre/" class="related-card"><span class="related-icon">⚖️</span><span class="related-title">Kg ↔ Libbre</span></a>
<a href="/smart-converter-tools/calcolatori/convertitore-centimetri-pollici/" class="related-card"><span class="related-icon">📱</span><span class="related-title">Cm ↔ Pollici</span></a>
<a href="/smart-converter-tools/calcolatori/convertitore-metri-piedi/" class="related-card"><span class="related-icon">📐</span><span class="related-title">Metri ↔ Piedi</span></a>
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

.ad-main{width:728px;height:90px;max-width:100%}
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
