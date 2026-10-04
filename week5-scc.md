---
layout: default
title: "Discount-Rate Surgery on the Social Cost of Carbon"
permalink: /week5/scc/
---
<link href="https://fonts.googleapis.com/css2?family=Newsreader:opsz,wght@6..72,400;6..72,600;6..72,700&family=Public+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.min.js"></script>
<style> #ex{--paper:#F2F4F3;--ink:#13202A;--muted:#56636E;--rule:#C9D1D6;--now:#1D4E89;--later:#A3336B;--card:#FFFFFF;--serif:"Newsreader",Georgia,"Times New Roman",serif;--sans:"Public Sans",system-ui,-apple-system,"Segoe UI",sans-serif;color:var(--ink);font:400 17px/1.6 var(--sans);max-width:780px;margin:0 auto} #ex *{box-sizing:border-box} #ex h1{font:700 clamp(32px,6vw,52px)/1.05 var(--serif);letter-spacing:-.01em;margin:0 0 14px;color:var(--ink);border:0} #ex h2{font:600 28px/1.2 var(--serif);margin:56px 0 8px;color:var(--ink);border:0} #ex h3{font:600 19px/1.3 var(--serif);margin:28px 0 6px;color:var(--ink)} #ex p{margin:0 0 14px} #ex .lede{font:400 20px/1.5 var(--serif);max-width:62ch} #ex .small{font-size:14px;color:var(--muted)} #ex a{color:var(--now)} #ex a:focus-visible,#ex input:focus-visible,#ex button:focus-visible{outline:3px solid var(--later);outline-offset:2px} #ex .instrument{margin:30px 0 10px;padding:28px 26px 22px;background:var(--card);border:1px solid var(--rule);border-radius:4px} #ex .readout{display:flex;align-items:baseline;gap:14px;flex-wrap:wrap} #ex .price{font:700 clamp(64px,13vw,112px)/1 var(--serif);color:var(--now);font-variant-numeric:tabular-nums;letter-spacing:-.02em} #ex .per{font:500 16px/1.3 var(--sans);color:var(--muted)} #ex .sentence{margin:12px 0 18px;font:400 18px/1.5 var(--serif)} #ex .sentence b{color:var(--now)} #ex .rate-row{display:flex;align-items:center;gap:14px} #ex .rate-row label{font-weight:600;white-space:nowrap} #ex input[type=range]{width:100%;accent-color:var(--now);height:28px} #ex .rate-val{font:600 18px var(--sans);min-width:56px;text-align:right;font-variant-numeric:tabular-nums} #ex .track{position:relative;height:124px;margin:26px 4px 0} #ex .track .line{position:absolute;left:0;right:0;top:44px;height:2px;background:var(--rule)} #ex .tick{position:absolute;top:40px;width:1px;height:10px;background:var(--muted)} #ex .tick span{position:absolute;top:14px;left:-22px;width:44px;text-align:center;font-size:12px;color:var(--muted)} #ex .ref{position:absolute;transform:translateX(-50%);text-align:center;font-size:12px;line-height:1.25;color:var(--ink)} #ex .ref.up{top:0;width:110px} #ex .ref.up::after{content:"";display:block;width:2px;height:12px;background:var(--ink);margin:3px auto 0} #ex .ref.down{top:84px;width:190px} #ex .mk{position:absolute;top:46px;width:2px;height:34px;background:var(--ink);transform:translateX(-1px)} #ex .bracket{position:absolute;top:78px;height:2px;background:var(--ink)} #ex .dot{position:absolute;top:36px;width:18px;height:18px;border-radius:50%;background:var(--now);border:3px solid #fff;box-shadow:0 0 0 1px var(--now);transform:translateX(-50%);transition:left .15s ease} @media (prefers-reduced-motion:reduce){#ex .dot{transition:none}} #ex .panel{background:var(--card);border:1px solid var(--rule);border-radius:4px;padding:20px 20px 14px;margin:18px 0} #ex .chartbox{position:relative;height:340px} #ex .chartbox.tall{height:380px} #ex table.heat{width:100%;border-collapse:collapse;font-variant-numeric:tabular-nums;font-size:15px;display:table} #ex table.heat th,#ex table.heat td{padding:9px 6px;text-align:center;border:1px solid #fff} #ex table.heat th{font-weight:600;background:transparent;color:var(--muted);font-size:13px} #ex table.heat td.cur{outline:2px solid var(--ink);outline-offset:-2px;font-weight:600} #ex .controls{display:grid;grid-template-columns:1fr 1fr;gap:6px 26px} #ex .ctl label{display:flex;justify-content:space-between;font-size:14px;font-weight:600} #ex .ctl label output{font-weight:500;color:var(--now);font-variant-numeric:tabular-nums} #ex .ctl .hint{font-size:12.5px;color:var(--muted);margin-top:-4px} #ex .modes{display:flex;gap:8px;margin-bottom:12px;flex-wrap:wrap} #ex .modes button{font:500 14px var(--sans);padding:7px 12px;border:1px solid var(--rule);background:#fff;border-radius:3px;cursor:pointer;color:var(--ink)} #ex .modes button[aria-pressed=true]{background:var(--ink);color:#fff;border-color:var(--ink)} #ex .ramsey-only{display:none} #ex.ramsey .ramsey-only{display:block} #ex.ramsey .const-only{display:none} #ex .callout{border-left:4px solid var(--later);padding:4px 0 4px 16px;margin:18px 0;font:400 19px/1.5 var(--serif)} #ex pre{font-size:14px;line-height:1.7;overflow-x:auto} @media (max-width:640px){#ex .controls{grid-template-columns:1fr}#ex .chartbox,#ex .chartbox.tall{height:300px}#ex .ref{font-size:11px}#ex .ref.down{width:150px}#ex .rate-row{flex-wrap:wrap}#ex .rate-row label{width:100%}#ex table.heat{font-size:13px}} #ex .eq{font:400 15px/1.7 ui-monospace,Menlo,Consolas,monospace;background:#E8ECEB;padding:12px 14px;border-radius:3px;overflow-x:auto;white-space:pre;color:var(--ink)} #ex ol.src li,#ex ul.plain li{margin-bottom:8px} #ex .ptable{width:100%;border-collapse:collapse;font-size:14.5px;display:table} #ex .ptable td,#ex .ptable th{border:0;border-bottom:1px solid var(--rule);padding:7px 6px;text-align:left;vertical-align:top;background:transparent;color:var(--ink)} #ex footer{margin-top:60px;font-size:14px;color:var(--muted);border-top:1px solid var(--rule);padding-top:16px} #ex footer p{margin:0 0 4px} </style>
<div id="ex" class="w5">
<h1>Discount-rate surgery on the social cost of carbon</h1>
<p class="lede">Washington has priced the same tonne of CO<sub>2</sub> at single digits, at $51, and at $190. The climate science barely changed between those numbers. Mostly, the interest rate did. Below is a small, fully visible SCC model you can operate on yourself.</p>
<section class="instrument" aria-label="Interactive social cost of carbon">
<div class="readout">
<div class="price" id="heroPrice">$53</div>
<div class="per">per tonne of CO<sub>2</sub><br>emitted in 2025</div>
</div>
<p class="sentence" id="heroSentence">At a <b>3.0%</b> discount rate, one extra tonne emitted in 2025 does $53 of damage, valued in today's dollars.</p>
<div class="rate-row">
<label for="heroRate">Discount rate</label>
<input type="range" id="heroRate" min="0.5" max="7" step="0.1" value="3">
<span class="rate-val" id="heroRateVal">3.0%</span>
</div>
<div class="track" id="track" aria-hidden="true">
<div class="line"></div>
</div>
<p class="small" style="margin-top:6px">Log scale. Markers are official U.S. values for 2020 emissions; this model prices 2025 emissions with simpler damages, so compare shapes, not cents.</p>
</section>
<h2>One table, two choices</h2>
<p>Each cell is the SCC from the same physics and the same damage function. Only the discount rate (rows) and how far into the future we count damages (columns) change. The outlined cell matches your current settings.</p>
<div class="panel"><div style="overflow-x:auto"><table class="heat" id="heat"></table></div>
<p class="small" style="margin-top:10px">At 5% the horizon hardly matters: anything after 2100 is discounted to almost nothing. At 1.5%, the choice between stopping at 2100 and 2300 more than triples the price.</p></div>
<h2>When does the damage you're paying for happen?</h2>
<p>Cumulative present value of damages from the 2025 tonne, year by year. Where each line flattens is where the future stops mattering to that discount rate.</p>
<div class="panel"><div class="chartbox"><canvas id="cumChart" aria-label="Cumulative discounted damages by year for three discount rates" role="img"></canvas></div></div>
<p class="callout" id="shareCallout">At 1.5%, about 72% of the SCC comes from damages after 2100. At 5%, about 10% does.</p>
<p>That is the whole fight in one sentence. A low discount rate says the SCC is mostly about people living in the 2100s and 2200s. A high one says it is mostly about the next few decades. Neither is a scientific finding; it is an ethical and financial judgment about how to weigh the future.</p>
<h2>Which assumption moves the price most?</h2>
<p>Each bar swings one input across a defensible range while everything else stays at your current settings. Change the settings below and the ranking updates.</p>
<div class="panel"><div class="chartbox tall"><canvas id="tornado" aria-label="Sensitivity of the SCC to each assumption" role="img"></canvas></div></div>
<div class="panel" id="controlsPanel">
<h3 style="margin-top:0">Your settings</h3>
<div class="modes" role="group" aria-label="Discounting method">
<button type="button" id="mConst" aria-pressed="true">Constant discount rate</button>
<button type="button" id="mRamsey" aria-pressed="false">Ramsey rule: r = ρ + η·g</button>
</div>
<div class="controls">
<div class="ctl const-only"><label for="cR">Discount rate <output id="oR"></output></label><input type="range" id="cR" min="0.5" max="7" step="0.1" value="3"><div class="hint">Same rate every year.</div></div>
<div class="ctl ramsey-only"><label for="cRho">Pure time preference ρ <output id="oRho"></output></label><input type="range" id="cRho" min="0" max="3" step="0.1" value="0.2"><div class="hint">Impatience for its own sake.</div></div>
<div class="ctl ramsey-only"><label for="cEta">Inequality aversion η <output id="oEta"></output></label><input type="range" id="cEta" min="0.5" max="2" step="0.05" value="1.24"><div class="hint">Richer futures need less help.</div></div>
<div class="ctl"><label for="cG">Near-term GDP growth <output id="oG"></output></label><input type="range" id="cG" min="0.5" max="4" step="0.1" value="2.5"><div class="hint">Fades toward a third of this over ~100 yrs.</div></div>
<div class="ctl"><label for="cEcs">Climate sensitivity (ECS) <output id="oEcs"></output></label><input type="range" id="cEcs" min="1.5" max="5.5" step="0.1" value="3"><div class="hint">°C per CO<sub>2</sub> doubling. IPCC AR6 best estimate: 3.</div></div>
<div class="ctl"><label for="cD3">GDP lost at 3°C <output id="oD3"></output></label><input type="range" id="cD3" min="0.5" max="12" step="0.5" value="3"><div class="hint">Level of the damage function.</div></div>
<div class="ctl"><label for="cB">Damage curvature <output id="oB"></output></label><input type="range" id="cB" min="1" max="4" step="0.1" value="2"><div class="hint">2 = quadratic, as in DICE.</div></div>
<div class="ctl"><label for="cH">Count damages through <output id="oH"></output></label><input type="range" id="cH" min="2100" max="2300" step="10" value="2300"><div class="hint">Model horizon.</div></div>
</div>
<p class="small" style="margin-top:12px">Try the Ramsey rule at ρ = 0.2% and η = 1.24 (the calibration EPA used in 2023), then push growth up. Faster growth raises future damages in dollars, but it also raises the discount rate, and the second effect usually wins.</p>
</div>
<h2>What the model is doing</h2>
<p>A tonne of CO<sub>2</sub> is added to the air in 2025 on top of a middle-of-the-road emissions path (roughly 2.5°C by 2100 at ECS 3). The model tracks how much of that tonne stays airborne, how much extra warming it causes each year, what that warming costs as a share of world GDP, and then discounts each year's cost back to 2025.</p>
<div class="eq">Airborne fraction    A(s) = 0.217 + 0.224e^(-s/394.4) + 0.282e^(-s/36.5) + 0.276e^(-s/4.3)
Extra CO2 (ppm)      ΔC(t) = 1.285e-10 × A(t-2025)
Extra forcing        ΔF(t) = 5.35 × ΔC(t) / C(t)
Extra warming        ΔT(t) = Σ ΔF(s) × R(t-s),  R = two-box response scaled to ECS
Damages (share GDP)  D(T)  = d₃ × (T/3)^b
Marginal damage      MD(t) = D'(T_base(t)) × ΔT(t) × GDP(t)
SCC                  = Σ MD(t) / Π(1 + r_k),  t = 2025 … horizon</div>
<table class="ptable" style="margin-top:14px">
<tr><th>Piece</th><th>Value used</th><th>Where it comes from</th></tr>
<tr><td>Carbon cycle</td><td>Impulse response above</td><td>Joos et al. (2013), used in IPCC AR5 for GWP calculations</td></tr>
<tr><td>Temperature response</td><td>Two timescales, 8.4 and 409.5 years</td><td>Boucher &amp; Reddy (2008), IPCC AR5 WG1 Ch. 8; rescaled to your ECS</td></tr>
<tr><td>Forcing</td><td>5.35 ln(C/C₀) W/m²</td><td>Myhre et al. (1998)</td></tr>
<tr><td>Baseline CO<sub>2</sub>, warming</td><td>425 ppm rising toward 600 ppm; 1.3°C rising toward ~3.2°C</td><td>Stylized medium path, my assumption</td></tr>
<tr><td>World GDP 2025</td><td>$115 trillion</td><td>Rounded from IMF estimates</td></tr>
<tr><td>Damage function</td><td>3% of GDP at 3°C, quadratic</td><td>Close to DICE-2023's level; Barrage &amp; Nordhaus (2024)</td></tr>
</table>
<p class="small" style="margin-top:10px">Sanity check: the model's peak warming per tonne is about 0.48 thousandths of a degree per billion tonnes, in line with the IPCC's TCRE range (roughly 0.27 to 0.63°C per 1,000 GtCO<sub>2</sub>). At 3% it lands at about $53, close to the IWG's 2021 interim $51. At 2% it gives about $123, well below EPA's $190, because EPA's damage functions add mortality and other impacts and its discounting builds in uncertainty about future rates.</p>
<h3>What this model leaves out</h3>
<ul class="plain">
<li>Uncertainty. Official estimates average thousands of Monte Carlo draws; the average of a skewed distribution sits above the value at the central inputs.</li>
<li>Sector and regional detail. EPA's 2023 estimate combined three damage modules (GIVE, DSCIM, and a meta-analysis), including heat mortality and agriculture.</li>
<li>Tipping points, sea-level rise dynamics, and feedback from damages to growth.</li>
<li>Equity weighting. A dollar of damage counts the same whether it falls on a rich or poor country.</li>
</ul>
<h2>The policy backdrop</h2>
<p>In 2021 the Biden administration restored an interim $51 per tonne at a 3% rate. In late 2023 EPA finalized new estimates of $120, $190 and $340 at 2.5%, 2% and 1.5% (2020 emissions, 2020 dollars), with RFF's GIVE model at the core. Analysts at the time attributed most of the jump from about $50 to $190 to the lower discount rate, with updated damages accounting for roughly a third. On January 20, 2025, Executive Order 14154 disbanded the Interagency Working Group, withdrew its estimates, and directed agencies back to OMB's 2003 Circular A-4 guidance, which uses 3% and 7% rates. The first Trump administration's values, which used those rates and counted only domestic damages, were in the single digits.</p>
<p>Set the hero slider to 7% and you'll see why the choice of rate is where most of the policy argument actually lives.</p>
<h2>Ask the next question</h2>
<ul class="plain">
<li>Declining discount rates: what happens if the rate starts at 3% and steps down over time, the way the UK Green Book's long-term schedule does?</li>
<li>Domestic-only damages: the U.S. is roughly a quarter of world GDP at market exchange rates. Scale damages down and compare to the 2017 values.</li>
<li>Add a tipping-point term, like a higher curvature above 3°C, and see if it changes the tornado ranking.</li>
<li>Price methane the same way with a 12-year lifetime instead of CO<sub>2</sub>'s centuries, and watch the discount rate stop mattering.</li>
</ul>
<h2>Sources</h2>
<ol class="src small">
<li>U.S. EPA (2023). <em>Report on the Social Cost of Greenhouse Gases: Estimates Incorporating Recent Scientific Advances.</em></li>
<li>Interagency Working Group on Social Cost of Greenhouse Gases (2021). <em>Technical Support Document: Social Cost of Carbon, Methane, and Nitrous Oxide, Interim Estimates.</em></li>
<li>Rennert, K. et al. (2022). Comprehensive evidence implies a higher social cost of CO<sub>2</sub>. <em>Nature</em> 610, 687–692.</li>
<li>Barrage, L. &amp; Nordhaus, W. (2024). Policies, projections, and the social cost of carbon: Results from the DICE-2023 model. <em>PNAS</em> 121(13).</li>
<li>Joos, F. et al. (2013). Carbon dioxide and climate impulse response functions. <em>Atmos. Chem. Phys.</em> 13, 2793–2825.</li>
<li>IPCC AR5 WG1 Chapter 8 (2013), Appendix 8.A; IPCC AR6 WG1 (2021) for ECS and TCRE ranges.</li>
<li>Executive Order 14154, "Unleashing American Energy" (Jan. 20, 2025); Harvard EELP regulatory tracker on the social cost of carbon.</li>
<li>OMB Circular A-4 (2003).</li>
</ol>
<h2>How AI was used</h2>
<p class="small">Built with Claude (Anthropic). I asked it to (1) pull the official SCC values and the 2025 policy changes from primary and news sources, (2) write a reduced-form SCC model from published carbon-cycle and temperature impulse responses, (3) calibrate it so the 3% case could be checked against the IWG's $51, (4) build the discount-rate × horizon table, the cumulative-damage chart, and the sensitivity tornado, and (5) list what the toy model omits relative to EPA's. I checked the outputs against the published reference values above. The entire model runs in this page; view the source to see every line.</p>
<footer><p>Arjun Aujla, Econ 238, Fall 2026</p><p>SHOW ME Museum exhibit, class list topic: Discount-Rate Surgery on the SCC</p></footer>
</div>
<script>
(function(){
"use strict";
var Y0=115e12, N=276, START=2025;
var physCache={};
function physics(ecs){
  var key=ecs.toFixed(2); if(physCache[key]) return physCache[key];
  var C=new Float64Array(N),Tb=new Float64Array(N),dF=new Float64Array(N),R=new Float64Array(N),dT=new Float64Array(N);
  var pulse=1/(3.664*2.124e9), sc=ecs/(1.06*3.71);
  for(var s=0;s<N;s++){
    C[s]=425+175*(1-Math.exp(-s/60));
    Tb[s]=1.3+(ecs/3)*1.9*(1-Math.exp(-s/70));
    var A=0.2173+0.2240*Math.exp(-s/394.4)+0.2824*Math.exp(-s/36.54)+0.2763*Math.exp(-s/4.304);
    dF[s]=5.35*pulse*A/C[s];
    R[s]=(0.631/8.4*Math.exp(-s/8.4)+0.429/409.5*Math.exp(-s/409.5))*sc;
  }
  for(var t=0;t<N;t++){var acc=0;for(var k=0;k<=t;k++)acc+=dF[k]*R[t-k];dT[t]=acc;}
  return (physCache[key]={Tb:Tb,dT:dT});
}
function pvPath(p){
  var ph=physics(p.ecs), pv=new Float64Array(N), Y=Y0, DF=1;
  for(var s=0;s<N;s++){
    var g=p.g*(1/3+2/3*Math.exp(-s/100));
    var r=p.mode==="ramsey"? p.rho+p.eta*g : p.r;
    var T=ph.Tb[s];
    var md=p.d3*p.b*Math.pow(T,p.b-1)/Math.pow(3,p.b)*ph.dT[s]*Y;
    pv[s]=md*DF;
    Y*=1+g; DF/=1+r;
  }
  return pv;
}
function scc(p){var pv=pvPath(p),h=p.h-START,sum=0;for(var s=0;s<=h&&s<N;s++)sum+=pv[s];return sum;}
function fmt(v){return v>=100? "$"+Math.round(v).toLocaleString() : v>=10? "$"+Math.round(v) : "$"+v.toFixed(1);}
function clone(o){var c={};for(var k in o)c[k]=o[k];return c;}
var P={mode:"const",r:0.03,rho:0.002,eta:1.24,g:0.025,ecs:3,d3:0.03,b:2,h:2300};
var $=function(id){return document.getElementById(id);};
var reduce=window.matchMedia&&window.matchMedia("(prefers-reduced-motion: reduce)").matches;
if(window.Chart){Chart.defaults.font.family='"Public Sans", system-ui, sans-serif';Chart.defaults.color="#56636E";if(reduce)Chart.defaults.animation=false;}
/* log track */
var track=$("track"), LMIN=Math.log10(1), LMAX=Math.log10(1000);
function xpos(v){var l=Math.log10(Math.max(1,Math.min(1000,v)));return ((l-LMIN)/(LMAX-LMIN)*100)+"%";}
[1,10,100,1000].forEach(function(v){var d=document.createElement("div");d.className="tick";d.style.left=xpos(v);d.innerHTML="<span>$"+v.toLocaleString()+"</span>";track.appendChild(d);});
function addRef(v,html,cls){var d=document.createElement("div");d.className="ref "+cls;d.style.left=xpos(v);d.innerHTML=html;track.appendChild(d);}
function addMk(v){var d=document.createElement("div");d.className="mk";d.style.left=xpos(v);track.appendChild(d);}
addRef(51,"IWG 2021, 3%<br>$51","up");
addMk(5);addRef(5,"Trump 2017–20<br>single digits","down");
[120,190,340].forEach(addMk);
(function(){var b=document.createElement("div");b.className="bracket";b.style.left=xpos(120);b.style.width="calc("+xpos(340)+" - "+xpos(120)+")";track.appendChild(b);})();
addRef(200,"EPA 2023 at 2.5%, 2%, 1.5%<br>$120, $190, $340","down");
var dot=document.createElement("div");dot.className="dot";track.appendChild(dot);
/* heat table */
var RATES=[0.015,0.02,0.025,0.03,0.04,0.05,0.07], HOR=[2100,2150,2200,2300];
function drawHeat(){
  var base=clone(P);base.mode="const";
  var html="<tr><th>Rate</th>"+HOR.map(function(h){return "<th>"+h+"</th>";}).join("")+"</tr>";
  RATES.forEach(function(r){
    html+="<tr><th>"+(r*100).toFixed(1)+"%</th>";
    var pv=pvPath((base.r=r,base));
    HOR.forEach(function(h){
      var sum=0;for(var s=0;s<=h-START;s++)sum+=pv[s];
      var t=Math.min(1,Math.max(0,(Math.log10(Math.max(sum,1))-0.7)/2));
      var light=95-t*58, col="hsl(212,55%,"+light+"%)", txt=light<60?"#fff":"#13202A";
      var cur=(P.mode==="const"&&Math.abs(P.r-r)<1e-9&&P.h===h)?' class="cur"':"";
      html+="<td"+cur+' style="background:'+col+";color:"+txt+'">'+fmt(sum)+"</td>";
    });
    html+="</tr>";
  });
  $("heat").innerHTML=html;
}
/* cumulative chart */
var years=[];for(var s=0;s<N;s++)years.push(START+s);
var cumChart=new Chart($("cumChart"),{type:"line",data:{labels:years,datasets:[]},options:{
  maintainAspectRatio:false,interaction:{mode:"index",intersect:false},elements:{point:{radius:0}},
  scales:{x:{ticks:{callback:function(v,i){var y=years[i];return y%25===0?y:"";},autoSkip:false,maxRotation:0},grid:{display:false}},
          y:{title:{display:true,text:"Cumulative discounted damage ($ per tonne)"},beginAtZero:true,grid:{color:"#E3E8EA"}}},
  plugins:{legend:{position:"bottom"},tooltip:{callbacks:{label:function(c){return c.dataset.label+": "+fmt(c.parsed.y);}}}}}});
var line2100={id:"line2100",afterDraw:function(ch){if(ch.canvas.id!=="cumChart")return;var x=ch.scales.x.getPixelForValue(75),a=ch.chartArea,ctx=ch.ctx;ctx.save();ctx.strokeStyle="#13202A";ctx.setLineDash([4,4]);ctx.beginPath();ctx.moveTo(x,a.top);ctx.lineTo(x,a.bottom);ctx.stroke();ctx.setLineDash([]);ctx.fillStyle="#13202A";ctx.font="12px Public Sans, sans-serif";ctx.fillText("2100",x+5,a.top+12);ctx.restore();}};
Chart.register(line2100);
function drawCum(){
  var specs=[[0.015,"#A3336B"],[0.03,"#1D4E89"],[0.05,"#7A8B96"]], shares=[];
  cumChart.data.datasets=specs.map(function(sp){
    var p=clone(P);p.mode="const";p.r=sp[0];var pv=pvPath(p),c=0,arr=[];
    for(var s=0;s<N;s++){c+=pv[s];arr.push(c);}
    shares.push(Math.round((1-arr[75]/arr[N-1])*100));
    return {label:(sp[0]*100).toFixed(1)+"% rate",data:arr,borderColor:sp[1],backgroundColor:sp[1],borderWidth:2.5,tension:0};
  });
  cumChart.update();
  $("shareCallout").textContent="At 1.5%, about "+shares[0]+"% of the SCC comes from damages after 2100. At 3%, about "+shares[1]+"%. At 5%, about "+shares[2]+"%.";
}
/* tornado */
var tor=new Chart($("tornado"),{type:"bar",data:{labels:[],datasets:[{data:[],backgroundColor:[],borderWidth:0,barPercentage:.7}]},options:{
  indexAxis:"y",maintainAspectRatio:false,
  scales:{x:{type:"logarithmic",title:{display:true,text:"SCC ($ per tonne, log scale)"},ticks:{callback:function(v){var l=Math.log10(v);return Math.abs(l-Math.round(l))<1e-6||[2,5].indexOf(Math.round(v/Math.pow(10,Math.floor(l))))>=0?"$"+v:"";}},grid:{color:"#E3E8EA"}},y:{grid:{display:false}}},
  plugins:{legend:{display:false},tooltip:{callbacks:{label:function(c){var d=c.raw;return fmt(d[0])+" to "+fmt(d[1]);}}}}}});
var baseLine={id:"baseLine",afterDatasetsDraw:function(ch){if(ch.canvas.id!=="tornado")return;var v=ch.$base;if(!v)return;var x=ch.scales.x.getPixelForValue(v),a=ch.chartArea,ctx=ch.ctx;ctx.save();ctx.strokeStyle="#13202A";ctx.lineWidth=2;ctx.beginPath();ctx.moveTo(x,a.top);ctx.lineTo(x,a.bottom);ctx.stroke();ctx.fillStyle="#13202A";ctx.font="600 12px Public Sans, sans-serif";ctx.fillText("Your settings: "+fmt(v),Math.min(x+6,a.right-120),a.top-4);ctx.restore();}};
Chart.register(baseLine);
function drawTornado(){
  var base=scc(P), items=[];
  function sw(name,key,lo,hi,fl,fh){var a=clone(P),b=clone(P);a[key]=lo;b[key]=hi;var va=scc(a),vb=scc(b);items.push({name:name+" ("+fl+" to "+fh+")",lo:Math.min(va,vb),hi:Math.max(va,vb)});}
  if(P.mode==="const") sw("Discount rate","r",0.02,0.04,"2%","4%");
  else {sw("Time preference ρ","rho",0.0,0.02,"0%","2%");sw("Inequality aversion η","eta",1.0,1.5,"1.0","1.5");}
  sw("Horizon","h",2100,2300,"2100","2300");
  sw("Damage level at 3°C","d3",0.015,0.06,"1.5%","6%");
  sw("Damage curvature","b",2,3,"2","3");
  sw("Climate sensitivity","ecs",2.5,4,"2.5°C","4°C");
  sw("GDP growth","g",0.015,0.035,"1.5%","3.5%");
  items.sort(function(a,b){return (b.hi/b.lo)-(a.hi/a.lo);});
  tor.data.labels=items.map(function(i){return i.name;});
  tor.data.datasets[0].data=items.map(function(i){return [i.lo,i.hi];});
  tor.data.datasets[0].backgroundColor=items.map(function(i){return /Discount|ρ|η/.test(i.name)?"#A3336B":"#1D4E89";});
  tor.$base=base;tor.update();
}
/* hero + controls */
function hero(){
  var v=scc(P);$("heroPrice").textContent=fmt(v);dot.style.left=xpos(v);
  var rtxt=P.mode==="const"? "a <b>"+(P.r*100).toFixed(1)+"%</b> discount rate" : "the Ramsey rule (ρ = "+(P.rho*100).toFixed(1)+"%, η = "+P.eta.toFixed(2)+")";
  $("heroSentence").innerHTML="At "+rtxt+", one extra tonne emitted in 2025 does "+fmt(v)+" of damage through "+P.h+", valued in today's dollars.";
  $("heroRateVal").textContent=(P.r*100).toFixed(1)+"%";
}
function outputs(){
  $("oR").textContent=(P.r*100).toFixed(1)+"%";$("oRho").textContent=(P.rho*100).toFixed(1)+"%";$("oEta").textContent=P.eta.toFixed(2);
  $("oG").textContent=(P.g*100).toFixed(1)+"%";$("oEcs").textContent=P.ecs.toFixed(1)+"°C";$("oD3").textContent=(P.d3*100).toFixed(1)+"%";
  $("oB").textContent=P.b.toFixed(1);$("oH").textContent=P.h;
}
var pending=false;
function all(){if(pending)return;pending=true;requestAnimationFrame(function(){pending=false;outputs();hero();drawHeat();drawCum();drawTornado();});}
function setMode(m){P.mode=m;document.getElementById("ex").classList.toggle("ramsey",m==="ramsey");$("mConst").setAttribute("aria-pressed",m==="const");$("mRamsey").setAttribute("aria-pressed",m==="ramsey");all();}
$("mConst").onclick=function(){setMode("const");};$("mRamsey").onclick=function(){setMode("ramsey");};
$("heroRate").addEventListener("input",function(e){P.r=+e.target.value/100;$("cR").value=e.target.value;if(P.mode!=="const")setMode("const");else all();});
$("cR").addEventListener("input",function(e){P.r=+e.target.value/100;$("heroRate").value=e.target.value;all();});
[["cRho","rho",100],["cEta","eta",1],["cG","g",100],["cEcs","ecs",1],["cD3","d3",100],["cB","b",1],["cH","h",1]].forEach(function(c){
  $(c[0]).addEventListener("input",function(e){P[c[1]]=+e.target.value/c[2];all();});
});
all();
})();
</script>
