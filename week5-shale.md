---
layout: default
title: "Who Cut America's Power-Plant Emissions?"
permalink: /week5/shale/
---
<link href="https://fonts.googleapis.com/css2?family=Archivo:wdth,wght@100,500;100,700;125,800&family=Source+Serif+4:opsz,wght@8..60,400;8..60,600&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.min.js"></script>
<style> #ex{--ink:#22252A;--muted:#5E646C;--rule:#D9DDE1;--wash:#F3F5F6;--coal:#3B332E;--gas:#2563EB;--ws:#0E8F6C;--nuc:#9AA5AD;--ch4:#D9480F;--head:"Archivo","Helvetica Neue",Arial,sans-serif;--body:"Source Serif 4",Georgia,"Times New Roman",serif;color:var(--ink);font:400 18px/1.65 var(--body);max-width:800px;margin:0 auto} #ex *{box-sizing:border-box} #ex h1{font:800 clamp(32px,6.2vw,56px)/1.03 var(--head);font-stretch:125%;letter-spacing:-.01em;margin:0 0 18px;color:var(--ink);border:0} #ex h2{font:700 26px/1.2 var(--head);margin:56px 0 10px;color:var(--ink);border:0} #ex h3{font:700 18px/1.3 var(--head);margin:26px 0 6px;color:var(--ink)} #ex p{margin:0 0 14px} #ex .lede{font-size:21px;line-height:1.55} #ex .small{font:400 14.5px/1.55 var(--head);color:var(--muted)} #ex a{color:var(--gas)} #ex a:focus-visible,#ex input:focus-visible,#ex button:focus-visible{outline:3px solid var(--ch4);outline-offset:2px} #ex .big{display:grid;grid-template-columns:1fr 1fr;margin:30px 0 8px;border-top:3px solid var(--ink)} #ex .big>div{padding:14px 0 4px} #ex .big>div+div{padding-left:22px;border-left:1px solid var(--rule)} #ex .big .n{font:800 clamp(40px,8vw,64px)/1 var(--head);font-variant-numeric:tabular-nums} #ex .big .l{font:500 15px/1.4 var(--head);color:var(--muted);margin-top:6px} #ex .panel{border:1px solid var(--rule);border-radius:6px;padding:20px;margin:18px 0;background:#fff} #ex .chartbox{position:relative;height:380px} #ex .chartbox.short{height:200px} #ex .ctl{margin:16px 0 4px} #ex .ctl label{display:flex;justify-content:space-between;gap:12px;font:700 15px/1.4 var(--head)} #ex .ctl output{font-weight:500;color:var(--ws);font-variant-numeric:tabular-nums} #ex .ends{display:flex;justify-content:space-between;font:400 13px var(--head);color:var(--muted)} #ex input[type=range]{width:100%;accent-color:var(--ink);height:28px} #ex .toggles{display:flex;flex-wrap:wrap;gap:8px;margin-top:14px} #ex .toggles button{font:500 14px var(--head);padding:7px 12px;border:1px solid var(--rule);border-radius:999px;background:#fff;color:var(--ink);cursor:pointer} #ex .toggles button[aria-pressed=true]{background:var(--ch4);border-color:var(--ch4);color:#fff} #ex .methane{display:none;background:var(--wash);border-radius:6px;padding:4px 14px 10px;margin-top:12px} #ex.ch4 .methane{display:block} #ex .credit{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:16px} #ex .credit div{border-top:4px solid var(--c);padding-top:8px} #ex .credit b{display:block;font:800 26px/1.1 var(--head);font-variant-numeric:tabular-nums} #ex .credit span{font:500 13.5px/1.35 var(--head);color:var(--muted)} #ex .callout{font:600 20px/1.45 var(--body);border-left:5px solid var(--ch4);padding:2px 0 2px 16px;margin:18px 0} #ex pre{font-size:14px;line-height:1.7;overflow-x:auto} @media (max-width:640px){#ex .big{grid-template-columns:1fr}#ex .big>div+div{padding-left:0;border-left:0;border-top:1px solid var(--rule)}#ex .credit{grid-template-columns:1fr}#ex .chartbox{height:320px}} #ex .eq{font:400 14.5px/1.7 ui-monospace,Menlo,Consolas,monospace;background:var(--wash);padding:12px 14px;border-radius:6px;overflow-x:auto;white-space:pre;color:var(--ink)} #ex ol.src li,#ex ul.plain li{margin-bottom:8px} #ex table.d{width:100%;border-collapse:collapse;font:400 14.5px/1.4 var(--head);font-variant-numeric:tabular-nums;display:table} #ex table.d th,#ex table.d td{border:0;border-bottom:1px solid var(--rule);padding:7px 6px;text-align:right;background:transparent;color:var(--ink)} #ex table.d th:first-child,#ex table.d td:first-child{text-align:left} #ex table.d th{color:var(--muted);font-weight:500} #ex footer{margin-top:60px;border-top:1px solid var(--rule);padding-top:14px;font:400 14px var(--head);color:var(--muted)} #ex footer p{margin:0 0 4px} </style>
<div id="ex" class="w5">
<h1>Who cut America's power-plant emissions?</h1>
<p class="lede">U.S. electricity makes far less CO<sub>2</sub> than it did in 2005, even though the grid now produces more power. Shale gas gets the credit in one story, wind and solar in another. Here the drop is taken apart piece by piece, including the assumption that decides who "wins" and the methane leaks that both stories usually skip.</p>
<div class="big">
<div><div class="n" id="nCf">2.79 bn t</div><div class="l">CO<sub>2</sub> if 2024's electricity had been made with 2005's fuel mix</div></div>
<div><div class="n" id="nAct">1.52 bn t</div><div class="l">CO<sub>2</sub> actually emitted making 2024's electricity (estimated)</div></div>
</div>
<h2>From the 2005 mix to the 2024 grid</h2>
<p>Start from a counterfactual: the same 4,392 terawatt-hours generated in 2024, but with 2005's shares of coal, gas, oil and everything else. Each bar then shows how much one change removed or added.</p>
<div class="panel">
<div class="chartbox"><canvas id="waterfall" role="img" aria-label="Waterfall chart from counterfactual 2024 emissions with the 2005 mix to actual 2024 emissions"></canvas></div>
<div class="ctl">
<label for="theta">What did a new wind or solar megawatt-hour push off the grid? <output id="oTheta">50% coal and oil</output></label>
<input type="range" id="theta" min="0" max="100" step="5" value="50">
<div class="ends"><span>All gas</span><span>All coal and oil</span></div>
</div>
<div class="toggles" role="group" aria-label="Methane accounting">
<button type="button" id="tCO2" aria-pressed="true">Smokestack CO<sub>2</sub> only</button>
<button type="button" id="tCH4" aria-pressed="false">Add methane leakage</button>
</div>
<div class="methane">
<div class="ctl">
<label for="leak">Methane leaked, share of gas produced <output id="oLeak">2.3%</output></label>
<input type="range" id="leak" min="0" max="10" step="0.1" value="2.3">
<div class="ends"><span>0%</span><span>10%</span></div>
</div>
<div class="toggles" role="group" aria-label="Methane warming metric">
<button type="button" id="g100" aria-pressed="true">Count over 100 years (GWP100)</button>
<button type="button" id="g20" aria-pressed="false">Count over 20 years (GWP20)</button>
</div>
</div>
<div class="credit">
<div style="--c:var(--gas)"><b id="cGas">–</b><span>million t credited to gas replacing coal and oil</span></div>
<div style="--c:var(--ws)"><b id="cWs">–</b><span>million t credited to wind and solar</span></div>
<div style="--c:var(--nuc)"><b id="cOther">–</b><span>million t added as nuclear, hydro and other low-carbon lost share</span></div>
</div>
</div>
<p class="callout" id="swing">Slide the dial: gas's credit ranges from about 550 to 1,000 million tonnes, and wind and solar's from about 320 to 770. The ranking flips depending on one assumption.</p>
<p>That assumption is real, not a modeling trick. In most hours, wind and solar push out whichever plant is most expensive to run at the margin. When gas was cheap, that was often gas, not coal. So "renewables cut emissions" and "fracking cut emissions" can both be true, and how you split the credit depends on what you believe about dispatch. EIA's own 2005–2019 analysis credited about 65% of the decline to coal-to-gas switching and about 30% to renewables. Since 2019, wind and solar have grown fast enough that the split is much closer.</p>
<h2>The mix that changed</h2>
<div class="panel"><div class="chartbox short"><canvas id="mix" role="img" aria-label="Share of U.S. electricity generation by source, 2005 and 2024"></canvas></div></div>
<p>Coal fell from about half of U.S. generation to about 15%. Gas went from under a fifth to over 42%. Wind and solar went from almost nothing to about 17%. Nuclear's output stayed flat, so its share slipped as total demand grew.</p>
<h2>The methane fine print</h2>
<p>Burning gas makes roughly 40% as much CO<sub>2</sub> per megawatt-hour as burning coal. But methane, which is what natural gas mostly is, leaks between the well and the power plant, and methane traps far more heat than CO<sub>2</sub>, especially in its first two decades. The chart shows the full per-megawatt-hour footprint as leakage rises.</p>
<div class="panel">
<div class="chartbox"><canvas id="leakChart" role="img" aria-label="Greenhouse gas footprint per megawatt-hour for gas and coal power as methane leakage rises"></canvas></div>
<div class="toggles" role="group" aria-label="Metric for the leakage chart">
<button type="button" id="l100" aria-pressed="true">GWP100</button>
<button type="button" id="l20" aria-pressed="false">GWP20</button>
</div>
</div>
<p class="callout" id="breakeven">Counted over 100 years, gas power stays cleaner than coal until roughly 14% leakage. Counted over 20 years, the break-even falls to about 6%.</p>
<p>The best national measurement, Alvarez et al. (2018), put U.S. oil and gas supply-chain leakage at 2.3% of gross gas production, about 60% above EPA's inventory at the time. At that rate gas power still beats coal on either metric, but its advantage shrinks noticeably on the 20-year view. The national average also hides huge spread: aerial surveys have found basins under 1% and parts of the New Mexico Permian near 9%. Gas from a leaky basin can be close to coal on a 20-year basis. Note that this per-megawatt-hour comparison is gentler than the stricter test in Alvarez et al. (2012), which asked when gas beats coal at every time horizon, including the first few years, and found a threshold near 3.2%.</p>
<h2>Numbers used</h2>
<div class="panel" style="overflow-x:auto">
<table class="d">
<tr><th>Terawatt-hours</th><th>2005</th><th>2024</th></tr>
<tr><td>Coal</td><td>2,012.9</td><td>652.8</td></tr>
<tr><td>Natural gas</td><td>761.0</td><td>1,864.9</td></tr>
<tr><td>Petroleum and other gases</td><td>135.7</td><td>~25*</td></tr>
<tr><td>Nuclear</td><td>782.0</td><td>782.0</td></tr>
<tr><td>Hydro, biomass, geothermal</td><td>339.3</td><td>304.6</td></tr>
<tr><td>Wind and solar (incl. rooftop)</td><td>18.4</td><td>756.7</td></tr>
<tr><td>Other</td><td>6.2</td><td>6.5</td></tr>
<tr><td><b>Total</b></td><td><b>4,055.4</b></td><td><b>4,392.5</b></td></tr>
</table>
<p class="small" style="margin-top:10px">*Approximate. 2024 total is utility-scale (4,308.6 TWh) plus estimated small-scale solar (83.9 TWh). Hydro, biomass and geothermal for 2024 are total renewables (1,061.3 TWh) minus wind and solar.</p>
</div>
<div class="eq">CO2 per MWh (EIA 2023):   coal 1.050 t   gas 0.437 t   oil/other ~0.95 t
Counterfactual 2024:      Σ  G_2024 × share_2005(fuel) × factor(fuel)
Actual 2024:              Σ  G_2024(fuel) × factor(fuel)
Wind & solar credit:      ΔWS × [θ × coal/oil factor + (1−θ) × gas factor]
Gas credit:               (coal+oil decline − θ × ΔWS) × (coal/oil factor − gas factor)
Methane per gas MWh:      132 kg burned → leak = 132 × L / (1 − L) kg CH4
Methane per coal MWh:     ~1.5 kg CH4 from mines (rough)
GWP (IPCC AR6, fossil):   29.8 over 100 yr, 82.5 over 20 yr</div>
<p class="small">Check: the estimated 2024 total (about 1.52 billion t) is within about 1% of EIA's reported ~1.54 billion t of power-sector CO<sub>2</sub>. The 132 kg figure comes from EIA's ~7.36 cubic feet of gas per kWh at ~95% methane. Coal-mine methane is an order-of-magnitude estimate from EPA inventory scales and could be off by half; it barely moves the result.</p>
<h3>What this leaves out</h3>
<ul class="plain">
<li>Efficiency gains within each fuel. Today's gas fleet is mostly efficient combined-cycle plants; holding 2023 emission factors fixed hides some improvement since 2005.</li>
<li>Why the mix changed. Cheap shale gas, state renewable mandates, federal tax credits, and coal plant age all mattered, and they interacted.</li>
<li>Demand. Flat electricity demand from 2005 to about 2021 made all of this easier. That era is ending.</li>
</ul>
<h2>Ask the next question</h2>
<ul class="plain">
<li>Demand is back. Utility-scale generation hit about 4,429 TWh in 2025, a record. If data centers add hundreds of TWh, what fills it, and what does the waterfall look like in 2030?</li>
<li>Run the waterfall state by state. Texas and Pennsylvania tell very different stories.</li>
<li>Replace GWP with the social cost of methane versus carbon, and price the leaks in dollars.</li>
<li>Use hourly grid data to estimate θ directly instead of assuming it.</li>
</ul>
<h2>Sources</h2>
<ol class="src small">
<li>EIA, <em>Annual Energy Review</em>, Table 8.2a, Electricity Net Generation: Total (All Sectors), 2005 values.</li>
<li>EIA, <em>Electric Power Annual 2024</em> and Electricity Monthly data, 2024 generation and power-sector CO<sub>2</sub>; 2024 summaries via Wolf Street and Electrek, Feb. 2025.</li>
<li>EIA FAQ, "How much carbon dioxide is produced per kilowatthour of U.S. electricity generation?" (2023 factors: coal 2.31 lb/kWh, gas 0.96 lb/kWh).</li>
<li>EIA, <em>Today in Energy</em> (2021), "Electric power sector CO<sub>2</sub> emissions drop as generation mix shifts from coal to natural gas."</li>
<li>Alvarez, R. A. et al. (2018). Assessment of methane emissions from the U.S. oil and gas supply chain. <em>Science</em> 361, 186–188.</li>
<li>Alvarez, R. A. et al. (2012). Greater focus needed on methane leakage from natural gas infrastructure. <em>PNAS</em> 109(17).</li>
<li>Chen, Y. et al. (2022). Quantifying regional methane emissions in the New Mexico Permian Basin with a comprehensive aerial survey. <em>Environ. Sci. Technol.</em></li>
<li>IPCC AR6 WG1 (2021), Chapter 7, Table 7.15 (methane GWPs).</li>
<li>EIA, <em>Electricity Explained</em>, 2025 U.S. generation.</li>
</ol>
<h2>How AI was used</h2>
<p class="small">Built with Claude (Anthropic). I asked it to (1) pull 2005 and 2024 generation by fuel and EIA's emission factors, (2) build a counterfactual "2005 mix on the 2024 grid" and decompose the gap, (3) identify which assumption controls how credit is split, which turned out to be what renewables displace at the margin, and make that a dial instead of hiding it, (4) add methane leakage with both 20- and 100-year metrics and compute the break-even rates, and (5) check the estimated 2024 total against EIA's reported emissions. All calculations run in this page; view the source to see them.</p>
<footer><p>Arjun Aujla, Econ 238, Fall 2026</p><p>SHOW ME Museum exhibit, my own topic</p></footer>
</div>
<script>
(function(){
"use strict";
var G=4392.5;
var S05={coal:2012.9/4055.4,gas:761.0/4055.4,oil:135.7/4055.4,ws:18.4/4055.4};
var A24={coal:652.8,gas:1864.9,oil:25,ws:756.7};
var EF={coal:1.050,gas:0.437,oil:0.95};
var CH4_GAS=132, CH4_COAL=1.5;
var st={theta:0.5,ch4:false,leak:0.023,gwp:29.8,lgwp:29.8};
var $=function(id){return document.getElementById(id);};
var reduce=window.matchMedia&&window.matchMedia("(prefers-reduced-motion: reduce)").matches;
Chart.defaults.font.family='"Archivo", "Helvetica Neue", Arial, sans-serif';Chart.defaults.color="#5E646C";if(reduce)Chart.defaults.animation=false;
function factors(ch4,leak,gwp){
  var gasEF=EF.gas, coalEF=EF.coal, oilEF=EF.oil;
  if(ch4){gasEF+=CH4_GAS*leak/(1-leak)*gwp/1000;coalEF+=CH4_COAL*gwp/1000;}
  return {coal:coalEF,gas:gasEF,oil:oilEF};
}
function decomp(){
  var f=factors(st.ch4,st.leak,st.gwp);
  var cf={coal:G*S05.coal,gas:G*S05.gas,oil:G*S05.oil,ws:G*S05.ws};
  var Ecf=cf.coal*f.coal+cf.gas*f.gas+cf.oil*f.oil;
  var Eact=A24.coal*f.coal+A24.gas*f.gas+A24.oil*f.oil;
  var drop=(cf.coal-A24.coal)+(cf.oil-A24.oil);
  var fossEF=((cf.coal-A24.coal)*f.coal+(cf.oil-A24.oil)*f.oil)/drop;
  var dWS=A24.ws-cf.ws, dGas=A24.gas-cf.gas, otherLoss=dWS+dGas-drop;
  var ws=dWS*(st.theta*fossEF+(1-st.theta)*f.gas);
  var gas=(drop-st.theta*dWS)*(fossEF-f.gas);
  var other=-otherLoss*f.gas;
  return {Ecf:Ecf,Eact:Eact,ws:ws,gas:gas,other:other};
}
function fm(v){return Math.round(v).toLocaleString();}
var wf=new Chart($("waterfall"),{type:"bar",data:{labels:["2024 grid,\n2005 mix","Gas replaced\ncoal and oil","Wind and\nsolar","Nuclear, hydro\nlost share","Actual\n2024"],
  datasets:[{data:[],backgroundColor:["#3B332E","#2563EB","#0E8F6C","#9AA5AD","#22252A"],borderWidth:0,barPercentage:.72}]},
  options:{maintainAspectRatio:false,plugins:{legend:{display:false},tooltip:{callbacks:{label:function(c){var d=c.raw;return fm(Math.abs(d[1]-d[0]))+" million t";}}}},
  scales:{y:{beginAtZero:true,title:{display:true,text:"Million tonnes per year"},grid:{color:"#ECEFF1"}},x:{grid:{display:false},ticks:{callback:function(v){return this.getLabelForValue(v).split("\n");}}}}}});
var wfLabels={id:"wfLabels",afterDatasetsDraw:function(ch){if(ch.canvas.id!=="waterfall")return;var ctx=ch.ctx,meta=ch.getDatasetMeta(0);ctx.save();ctx.font="700 13px Archivo, sans-serif";ctx.fillStyle="#22252A";ctx.textAlign="center";
  meta.data.forEach(function(b,i){var d=ch.data.datasets[0].data[i];var v=d[1]-d[0];var txt=(i===0||i===4)?fm(d[1]):(v>0?"+":"−")+fm(Math.abs(v));ctx.fillText(txt,b.x,Math.min(b.y,b.base)-6);});ctx.restore();}};
Chart.register(wfLabels);
function drawWF(){
  var d=decomp(), a=d.Ecf, b=a-d.gas, c=b-d.ws, e=c-d.other;
  wf.data.datasets[0].data=[[0,a],[b,a],[c,b],[c,e],[0,d.Eact]];
  wf.update();
  $("nCf").textContent=(d.Ecf/1000).toFixed(2)+" bn t";$("nAct").textContent=(d.Eact/1000).toFixed(2)+" bn t";
  $("cGas").textContent=fm(d.gas);$("cWs").textContent=fm(d.ws);$("cOther").textContent="+"+fm(-d.other);
  var t=Math.round(st.theta*100);
  $("oTheta").textContent= t===0?"all gas": t===100?"all coal and oil": t+"% coal and oil, "+(100-t)+"% gas";
  var s0=st.theta;st.theta=0;var lo=decomp();st.theta=1;var hi=decomp();st.theta=s0;
  $("swing").textContent="Slide the dial: gas's credit ranges from about "+r50(hi.gas)+" to "+r50(lo.gas)+" million tonnes, and wind and solar's from about "+r50(lo.ws)+" to "+r50(hi.ws)+". "+(hi.ws>hi.gas&&lo.gas>lo.ws?"The ranking flips depending on one assumption.":"");
}
function r50(v){return (Math.round(v/10)*10).toLocaleString();}
var mix=new Chart($("mix"),{type:"bar",data:{labels:["2005","2024"],datasets:[
  {label:"Coal",data:[2012.9/4055.4,652.8/4392.5],backgroundColor:"#3B332E"},
  {label:"Oil & other gases",data:[135.7/4055.4,25/4392.5],backgroundColor:"#8C6E54"},
  {label:"Natural gas",data:[761.0/4055.4,1864.9/4392.5],backgroundColor:"#2563EB"},
  {label:"Nuclear",data:[782.0/4055.4,782.0/4392.5],backgroundColor:"#9AA5AD"},
  {label:"Hydro, biomass, geothermal",data:[339.3/4055.4,304.6/4392.5],backgroundColor:"#6BA6C9"},
  {label:"Wind & solar",data:[18.4/4055.4,756.7/4392.5],backgroundColor:"#0E8F6C"},
  {label:"Other",data:[6.2/4055.4,6.5/4392.5],backgroundColor:"#D9DDE1"}]},
  options:{indexAxis:"y",maintainAspectRatio:false,scales:{x:{stacked:true,max:1,ticks:{callback:function(v){return Math.round(v*100)+"%";}},grid:{color:"#ECEFF1"}},y:{stacked:true,grid:{display:false}}},
  plugins:{legend:{position:"bottom",labels:{boxWidth:12}},tooltip:{callbacks:{label:function(c){return c.dataset.label+": "+(c.parsed.x*100).toFixed(1)+"%";}}}}}});
var Ls=[];for(var i=0;i<=100;i++)Ls.push(i/10);
var lc=new Chart($("leakChart"),{type:"line",data:{labels:Ls,datasets:[]},options:{maintainAspectRatio:false,elements:{point:{radius:0}},interaction:{mode:"index",intersect:false},
  scales:{x:{title:{display:true,text:"Methane leaked (% of gas produced)"},ticks:{callback:function(v,i){return Ls[i]%1===0?Ls[i]+"%":"";},autoSkip:false,maxRotation:0},grid:{display:false}},
          y:{beginAtZero:true,title:{display:true,text:"Tonnes CO₂-equivalent per MWh"},grid:{color:"#ECEFF1"}}},
  plugins:{legend:{position:"bottom"},tooltip:{callbacks:{title:function(c){return Ls[c[0].dataIndex]+"% leakage";},label:function(c){return c.dataset.label+": "+c.parsed.y.toFixed(2)+" t";}}}}}});
var marks={id:"marks",afterDraw:function(ch){if(ch.canvas.id!=="leakChart")return;var ctx=ch.ctx,a=ch.chartArea,x=ch.scales.x;ctx.save();ctx.font="600 12px Archivo, sans-serif";
  [[2.3,"Alvarez 2018: 2.3%"],[9.4,"NM Permian: 9.4%"]].forEach(function(m){var px=x.getPixelForValue(Math.round(m[0]*10));ctx.strokeStyle="#D9480F";ctx.setLineDash([3,3]);ctx.beginPath();ctx.moveTo(px,a.top);ctx.lineTo(px,a.bottom);ctx.stroke();ctx.setLineDash([]);ctx.fillStyle="#D9480F";ctx.textAlign=m[0]>8?"right":"left";ctx.fillText(m[1],px+(m[0]>8?-5:5),a.top+12);});
  ctx.restore();}};
Chart.register(marks);
function breakeven(gwp){var c=EF.coal+CH4_COAL*gwp/1000, k=CH4_GAS*gwp/1000, q=(c-EF.gas)/k;return q/(1+q);}
function drawLeak(){
  var g=st.lgwp;
  lc.data.datasets=[
    {label:"Gas power",data:Ls.map(function(L){var l=L/100;return EF.gas+CH4_GAS*l/(1-l)*g/1000;}),borderColor:"#2563EB",backgroundColor:"#2563EB",borderWidth:3},
    {label:"Coal power",data:Ls.map(function(){return EF.coal+CH4_COAL*g/1000;}),borderColor:"#3B332E",backgroundColor:"#3B332E",borderWidth:3}];
  lc.update();
  var b100=breakeven(29.8)*100,b20=breakeven(82.5)*100;
  $("breakeven").textContent="Counted over 100 years, gas power stays cleaner than coal until roughly "+b100.toFixed(0)+"% leakage. Counted over 20 years, the break-even falls to about "+b20.toFixed(1)+"%.";
}
function press(on,off){$(on).setAttribute("aria-pressed","true");$(off).setAttribute("aria-pressed","false");}
$("theta").addEventListener("input",function(e){st.theta=+e.target.value/100;drawWF();});
$("tCO2").onclick=function(){st.ch4=false;press("tCO2","tCH4");document.getElementById("ex").classList.remove("ch4");drawWF();};
$("tCH4").onclick=function(){st.ch4=true;press("tCH4","tCO2");document.getElementById("ex").classList.add("ch4");drawWF();};
$("leak").addEventListener("input",function(e){st.leak=+e.target.value/100;$("oLeak").textContent=(+e.target.value).toFixed(1)+"%";drawWF();});
$("g100").onclick=function(){st.gwp=29.8;press("g100","g20");drawWF();};
$("g20").onclick=function(){st.gwp=82.5;press("g20","g100");drawWF();};
$("l100").onclick=function(){st.lgwp=29.8;press("l100","l20");drawLeak();};
$("l20").onclick=function(){st.lgwp=82.5;press("l20","l100");drawLeak();};
drawWF();drawLeak();
})();
</script>
