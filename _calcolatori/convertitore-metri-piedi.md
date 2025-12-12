---
layout: calculator
title: "Convertitore Metri Piedi  |  m ↔ ft  |  Online Gratis"
description: "Converti metri in piedi e piedi in metri istantaneamente. Calcolatore gratuito con conversione piedi-pollici."
---

<div class="page-hero">
  <div class="hero-icon">📐</div>
  <h1>Convertitore Metri Piedi</h1>
  <p>Converti velocemente tra m e ft</p>
</div>

<div class="ad-container ad-primary">
  <span class="ad-label">Pubblicità</span>
  <div class="ad-placeholder ad-rectangle">
    <span class="ad-text">Banner 336×280</span>
  </div>
</div>

<div class="calculator-box">
  <div class="converter-tabs">
    <button class="tab-btn active" onclick="switchTab('a')"><span class="tab-label">Metri → Piedi</span></button>
    <button class="tab-btn" onclick="switchTab('b')"><span class="tab-label">Piedi → Metri</span></button>
  </div>
  
  <div id="a" class="converter-panel active">
    <div class="input-wrapper"><label for="in1">Metri (m)</label><input type="number" id="in1" placeholder="Inserisci valore" step="0.01" min="0"></div>
    <button class="calc-button" onclick="conv1()"><span class="button-icon">⚡</span>Converti in Piedi</button>
    <div id="res1" class="result-box"></div>
  </div>
  
  <div id="b" class="converter-panel">
    <div class="input-wrapper"><label for="in2">Piedi (ft)</label><input type="number" id="in2" placeholder="Inserisci valore" step="0.01" min="0"></div>
    <button class="calc-button" onclick="conv2()"><span class="button-icon">⚡</span>Converti in Metri</button>
    <div id="res2" class="result-box"></div>
  </div>
</div>

<script>
function switchTab(t){const a=document.getElementById('a');const b=document.getElementById('b');const btns=document.querySelectorAll('.tab-btn');if(t==='a'){a.classList.add('active');b.classList.remove('active');btns[0].classList.add('active');btns[1].classList.remove('active')}else{b.classList.add('active');a.classList.remove('active');btns[1].classList.add('active');btns[0].classList.remove('active')}}
function conv1(){const v=parseFloat(document.getElementById('in1').value);const r=document.getElementById('res1');if(isNaN(v)||v<0){r.innerHTML='<div class="error-message">⚠️ Inserisci un numero valido</div>';return}const res=v*3.28084;const wf=Math.floor(res);const inch=(res-wf)*12;r.innerHTML=`<div class="result-success"><div class="result-main">${v.toFixed(2)} m = <strong>${res.toFixed(2)} piedi</strong></div><p style="font-size:0.85rem;color:#666;margin-top:0.4rem">oppure ${wf} ft ${inch.toFixed(1)} pollici</p></div>`}
function conv2(){const v=parseFloat(document.getElementById('in2').value);const r=document.getElementById('res2');if(isNaN(v)||v<0){r.innerHTML='<div class="error-message">⚠️ Inserisci un numero valido</div>';return}const res=v*0.3048;r.innerHTML=`<div class="result-success"><div class="result-main">${v.toFixed(2)} ft = <strong>${res.toFixed(2)} metri</strong></div></div>`}
window.addEventListener('load',function(){document.getElementById('in1').value='10';conv1()});
</script>

<div class="content-section">
<h2>Come usare il convertitore</h2>
<p>Seleziona la direzione, inserisci il valore e premi "Converti". La conversione da metri a piedi mostra anche il formato piedi+pollici.</p>
</div>

<div class="related-tools">
<h3>Convertitori correlati</h3>
<div class="related-grid">
<a href="/smart-converter-tools/calcolatori/convertitore-chilometri-miglia/" class="related-card"><span class="related-icon">🚗</span><span class="related-title">Km ↔ Miglia</span></a>
<a href="/smart-converter-tools/calcolatori/convertitore-centimetri-pollici/" class="related-card"><span class="related-icon">📱</span><span class="related-title">Cm ↔ Pollici</span></a>
<a href="/smart-converter-tools/calcolatori/convertitore-chilogrammi-libbre/" class="related-card"><span class="related-icon">⚖️</span><span class="related-title">Kg ↔ Libbre</span></a>
</div>
</div>

<style>:root{--primary-purple:#667eea;--primary-purple-dark:#764ba2;--accent-green:#10b981;--gray-50:#f7fafc;--gray-100:#edf2f7;--gray-200:#e2e8f0;--gray-300:#cbd5e0;--gray-400:#a0aec0;--gray-600:#4a5568;--gray-700:#2d3748;--gray-800:#1a202c}.page-hero{background:linear-gradient(135deg,#667eea 0%,#764ba2 50%,#f093fb 100%);padding:1.25rem 1rem;text-align:center;margin:-1.5rem -1.5rem 1.5rem -1.5rem;box-shadow:0 4px 20px rgba(102,126,234,0.3)}.hero-icon{font-size:2.5rem;margin-bottom:0.5rem}.page-hero h1{color:white;font-size:1.5rem;font-weight:700;margin:0 0 0.4rem 0;line-height:1.2}.page-hero p{color:white;font-size:0.9rem;margin:0;opacity:0.95}.calculator-box{background:white;border:2px solid var(--gray-200);border-radius:12px;padding:1.25rem;box-shadow:0 4px 16px rgba(0,0,0,0.08);max-width:600px;margin:0 auto 1.5rem}.converter-tabs{display:grid;grid-template-columns:1fr 1fr;gap:0.4rem;margin-bottom:1.25rem}.tab-btn{background:var(--gray-50);border:2px solid var(--gray-200);border-radius:8px;padding:0.65rem 0.5rem;cursor:pointer;font-family:'Montserrat',sans-serif;font-size:0.85rem;font-weight:600;color:var(--gray-600);transition:all 0.3s;position:relative;overflow:hidden}.tab-btn::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,var(--primary-purple),var(--accent-green));transform:scaleX(0);transition:transform 0.3s}.tab-btn.active::before{transform:scaleX(1)}.tab-btn.active{background:white;border-color:var(--primary-purple);color:var(--primary-purple)}.tab-label{display:block;text-align:center}.converter-panel{display:none}.converter-panel.active{display:block}.input-wrapper{margin-bottom:0.9rem}.input-wrapper label{display:block;color:var(--gray-700);font-size:0.85rem;font-weight:600;margin-bottom:0.4rem;text-align:center}.input-wrapper input{width:100%;padding:0.9rem;font-size:1rem;font-family:'Montserrat',sans-serif;font-weight:500;text-align:center;border:2px solid var(--gray-200);border-radius:8px;background:var(--gray-50);color:var(--gray-800);transition:all 0.3s;min-height:48px}.input-wrapper input:focus{outline:none;border-color:var(--primary-purple);background:white;box-shadow:0 0 0 3px rgba(102,126,234,0.1)}.calc-button{width:100%;padding:1rem;font-size:1rem;font-weight:700;font-family:'Montserrat',sans-serif;color:white;background:linear-gradient(135deg,var(--primary-purple) 0%,var(--primary-purple-dark) 100%);border:none;border-radius:8px;cursor:pointer;transition:all 0.3s;box-shadow:0 4px 12px rgba(102,126,234,0.3);display:flex;align-items:center;justify-content:center;gap:0.5rem;margin-bottom:0.9rem;min-height:52px}.calc-button:hover{transform:translateY(-2px);box-shadow:0 6px 18px rgba(102,126,234,0.4)}.button-icon{font-size:1.1rem}.result-box{min-height:55px;display:flex;align-items:center;justify-content:center}.result-success{background:linear-gradient(135deg,#ecfdf5 0%,#d1fae5 100%);border:2px solid var(--accent-green);border-radius:8px;padding:0.9rem;text-align:center;animation:slideIn 0.3s ease}.result-main{color:var(--gray-800);font-size:1rem}.result-main strong{color:var(--accent-green);font-weight:700}.error-message{background:#fef2f2;border:2px solid #fca5a5;border-radius:8px;padding:0.9rem;color:#991b1b;text-align:center;font-weight:600}@keyframes slideIn{from{opacity:0;transform:translateY(-8px)}to{opacity:1;transform:translateY(0)}}.content-section{margin:1.5rem auto;line-height:1.6;max-width:800px}.content-section h2{color:var(--gray-800);font-size:1.3rem;font-weight:700;margin-bottom:0.8rem;padding-bottom:0.4rem;border-bottom:3px solid var(--primary-purple);display:inline-block}.content-section h3{color:var(--gray-700);font-size:1.1rem;font-weight:600;margin:1.2rem 0 0.6rem}.content-section p{color:var(--gray-600);margin-bottom:0.9rem;font-size:0.95rem}.related-tools{margin:2rem auto;max-width:800px}.related-tools h3{color:var(--gray-800);font-size:1.2rem;font-weight:700;margin-bottom:0.9rem}.related-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:0.8rem}.related-card{background:white;border:2px solid var(--gray-200);border-radius:10px;padding:0.9rem;text-decoration:none;display:flex;align-items:center;gap:0.65rem;transition:all 0.3s}.related-card:hover{border-color:var(--primary-purple);transform:translateY(-2px);box-shadow:0 6px 12px rgba(102,126,234,0.15)}.related-icon{font-size:1.6rem;flex-shrink:0}.related-title{color:var(--gray-700);font-weight:600;font-size:0.9rem}.ad-container{display:flex;flex-direction:column;align-items:center;margin:1.25rem auto;max-width:100%}.ad-primary{margin:1.25rem auto 1.5rem}.ad-label{font-size:0.65rem;color:var(--gray-400);text-transform:uppercase;letter-spacing:0.05em;margin-bottom:0.4rem;font-weight:600}.ad-placeholder{background:linear-gradient(135deg,var(--gray-50) 0%,var(--gray-100) 100%);border:2px dashed var(--gray-300);border-radius:8px;display:flex;align-items:center;justify-content:center}.ad-rectangle{width:336px;height:280px;max-width:100%}.ad-text{color:var(--gray-400);font-size:0.8rem;font-weight:500}@media (max-width:768px){.page-hero{padding:1rem 0.8rem;margin:-1rem -1rem 1.25rem -1rem}.hero-icon{font-size:2.2rem}.page-hero h1{font-size:1.35rem}.page-hero p{font-size:0.85rem}.calculator-box{padding:1rem}.related-grid{grid-template-columns:1fr}}</style>
