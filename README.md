<!doctype html><html><head><meta charset=utf8><meta name=viewport content="width=device-width,initial-scale=1,viewport-fit=cover"><style>:root{color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}html{scroll-padding-top:env(safe-area-inset-top,0px)}body{margin:0;padding:0;font:14px -apple-system,BlinkMacSystemFont,sans-serif;background:#fff;color:#000}img{max-width:100%}[hidden]:not([hidden=until-found i]){display:none!important}</style></head><body>
<title>Multimodal Freight (MMF) (Copy)</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@600;700;800&family=Barlow:wght@400;500;600&family=IBM+Plex+Mono:wght@500&display=swap">
<style>
/* Layout: one mobile column read like a rail line — stations (sections) hang off a yellow track, fleet & depot numbers set like container markings */
:root{
  --bg:#F3F5FA; --surface:#FFFFFF; --ink:#0F1A3D; --muted:#4D587A; --line:#D9DEEB;
  --navy:#16235C; --navy-ink:#FFFFFF; --yellow:#F6C514; --yellow-ink:#16235C; --red:#D3262F;
  --display:"Barlow Condensed","Arial Narrow",Arial,sans-serif;
  --body:"Barlow",system-ui,-apple-system,"Segoe UI",sans-serif;
  --mono:"IBM Plex Mono",ui-monospace,Menlo,Consolas,monospace;
}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){
  --bg:#0B1230; --surface:#131C44; --ink:#EEF1FA; --muted:#A9B2D2; --line:#26316A;
  --navy:#1D2C72; --navy-ink:#FFFFFF; --yellow:#F6C514; --yellow-ink:#0B1230; --red:#F0525A; color-scheme:dark}}
:root[data-theme="dark"]{
  --bg:#0B1230; --surface:#131C44; --ink:#EEF1FA; --muted:#A9B2D2; --line:#26316A;
  --navy:#1D2C72; --navy-ink:#FFFFFF; --yellow:#F6C514; --yellow-ink:#0B1230; --red:#F0525A; color-scheme:dark}

*{box-sizing:border-box}
body{background:var(--bg);color:var(--ink);font:400 16px/1.55 var(--body);-webkit-font-smoothing:antialiased}
a{color:inherit}
:focus-visible{outline:3px solid var(--yellow);outline-offset:2px}
.wrap{max-width:760px;margin:0 auto;padding-inline:18px}
h1,h2,h3{font-family:var(--display);text-wrap:balance;margin:0;line-height:1.02;letter-spacing:.005em}
h2{font-size:clamp(30px,8vw,42px);font-weight:800;text-transform:uppercase}
h3{font-size:22px;font-weight:700;text-transform:uppercase}
p{margin:0}
.tag{font-family:var(--mono);font-size:12px;letter-spacing:.08em;text-transform:uppercase;color:var(--muted)}

/* Hero */
.hero{background:var(--navy);color:var(--navy-ink);position:relative;overflow:hidden}
.hero-top{display:flex;align-items:center;justify-content:space-between;gap:12px;padding-block:14px}
.logo{height:44px;width:auto;border-radius:6px;display:block}
.parent{font-family:var(--mono);font-size:11px;letter-spacing:.08em;text-transform:uppercase;opacity:.85;text-align:right;line-height:1.35}
.hero-photo{position:relative;aspect-ratio:16/10;max-width:100%;background:#0B1230}
.hero-photo img{width:100%;height:100%;object-fit:cover;display:block}
.hero-photo::after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,rgba(22,35,92,0) 45%,rgba(22,35,92,.95) 100%)}
.hero-text{position:relative;margin-top:-86px;z-index:1;padding-block:0 26px;display:grid;gap:12px}
.hero h1{font-size:clamp(44px,13vw,76px);font-weight:800;text-transform:uppercase;line-height:.92}
.hero h1 span{color:var(--yellow)}
.motto{font-family:var(--display);font-weight:600;font-size:20px;letter-spacing:.14em;text-transform:uppercase;color:var(--yellow)}
.lede{font-size:17px;max-width:58ch;opacity:.92}
.actions{display:flex;flex-wrap:wrap;gap:10px;margin-top:6px}
.btn{display:inline-flex;align-items:center;gap:8px;font:700 16px/1 var(--display);letter-spacing:.06em;text-transform:uppercase;text-decoration:none;padding:13px 16px;border-radius:4px;border:2px solid var(--yellow)}
.btn.primary{background:var(--yellow);color:var(--yellow-ink)}
.btn.ghost{color:var(--navy-ink)}
.btn svg{width:18px;height:18px;flex:none}
.hazard{height:10px;background:repeating-linear-gradient(-45deg,var(--yellow) 0 14px,var(--navy) 14px 28px)}

/* Numbers */
.numbers{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:1px;background:var(--line);border:1px solid var(--line);margin-top:28px}
.num{background:var(--surface);padding:16px 14px;display:grid;gap:2px}
.num b{font:800 40px/1 var(--display);color:var(--ink);font-variant-numeric:tabular-nums}
.num b small{font-size:20px;font-weight:700;color:var(--muted);margin-left:2px}
.num span{font-size:14px;color:var(--muted);line-height:1.3}
@media (min-width:620px){.numbers{grid-template-columns:repeat(4,minmax(0,1fr))}}

/* Sections */
section{padding-block:44px 8px}
.head{display:grid;gap:8px;margin-bottom:20px}
.head p{color:var(--muted);max-width:60ch}

.about{display:grid;gap:18px}
.about-card{display:grid;grid-template-columns:110px minmax(0,1fr);gap:14px;align-items:start}
.about-card img{width:110px;aspect-ratio:3/4;object-fit:cover;border-radius:4px;max-width:100%}
.timeline{display:grid;gap:0;border-left:3px solid var(--yellow);margin-left:6px}
.timeline div{position:relative;padding:0 0 16px 18px}
.timeline div::before{content:"";position:absolute;left:-9px;top:5px;width:15px;height:15px;border-radius:50%;background:var(--bg);border:3px solid var(--navy)}
.timeline b{font:800 22px/1 var(--display);display:block;margin-bottom:3px}
.vision{background:var(--yellow);color:var(--yellow-ink);padding:18px;border-radius:4px;font:700 22px/1.15 var(--display);text-transform:uppercase;letter-spacing:.02em}
.vision small{display:block;font:500 12px/1.4 var(--mono);letter-spacing:.08em;margin-bottom:6px}

/* Services */
.services{display:grid;gap:14px}
.svc{background:var(--surface);border:1px solid var(--line);border-radius:6px;overflow:hidden;display:grid}
.svc img{width:100%;aspect-ratio:16/8;object-fit:cover;display:block;max-width:100%}
.svc-body{padding:16px;display:grid;gap:10px;min-width:0}
.svc-top{display:flex;justify-content:space-between;align-items:baseline;gap:10px}
.code{font-family:var(--mono);font-size:12px;color:var(--muted);white-space:nowrap}
.svc ul{margin:0;padding:0;list-style:none;display:flex;flex-wrap:wrap;gap:6px}
.svc li{font-size:13.5px;font-weight:600;background:var(--bg);border:1px solid var(--line);padding:4px 9px;border-radius:999px}
.svc p{color:var(--muted)}
@media (min-width:620px){.svc{grid-template-columns:42% minmax(0,1fr)}.svc img{height:100%;aspect-ratio:auto}}

/* Tables */
.tbl{overflow-x:auto;border:1px solid var(--line);border-radius:6px;background:var(--surface)}
table{width:100%;border-collapse:collapse;font-variant-numeric:tabular-nums;min-width:320px}
th,td{padding:10px 8px;text-align:right;border-bottom:1px solid var(--line);white-space:nowrap}
th:first-child,td:first-child{text-align:left}
thead th{font:600 12px/1.2 var(--mono);letter-spacing:.06em;text-transform:uppercase;color:var(--muted)}
tbody tr:last-child td{border-bottom:0}
tfoot td{font-weight:700;border-top:2px solid var(--ink);border-bottom:0}
.note{font-size:14px;color:var(--muted);margin-top:10px}

/* Rail line network */
.line{position:relative;display:grid;gap:0;margin-left:4px}
.line::before{content:"";position:absolute;left:13px;top:10px;bottom:10px;width:6px;background:var(--yellow);border-radius:3px}
.stn{position:relative;padding:0 0 22px 46px;display:grid;gap:4px}
.stn::before{content:"";position:absolute;left:4px;top:2px;width:24px;height:24px;border-radius:50%;background:var(--surface);border:5px solid var(--navy)}
.stn.hq::before{background:var(--red);border-color:var(--navy)}
.stn h3{font-size:24px}
.stn .tag{color:var(--muted)}
.facts{display:flex;flex-wrap:wrap;gap:6px 14px;font-size:14.5px;color:var(--muted)}
.facts b{color:var(--ink);font-weight:600}
.tel{font-family:var(--mono);font-size:14.5px;text-decoration:none;border-bottom:1px dashed var(--muted);width:max-content}

/* Gallery */
.strip{display:grid;grid-auto-flow:column;grid-auto-columns:78%;gap:10px;overflow-x:auto;scroll-snap-type:x mandatory;padding-bottom:8px}
.strip figure{margin:0;scroll-snap-align:start;background:var(--surface);border:1px solid var(--line);border-radius:6px;overflow:hidden}
.strip img{width:100%;aspect-ratio:4/3;object-fit:cover;display:block}
.strip figcaption{padding:10px 12px;font-size:14px;color:var(--muted)}
@media (min-width:620px){.strip{grid-auto-columns:46%}}

/* Projects */
.projects{display:grid;gap:0;border-top:1px solid var(--line)}
.prj{display:grid;grid-template-columns:76px minmax(0,1fr);gap:12px;padding:12px 0;border-bottom:1px solid var(--line)}
.prj .yr{font:500 13px/1.5 var(--mono);color:var(--muted)}
.prj b{display:block;font-weight:600}
.prj span{color:var(--muted);font-size:15px}
.more{margin-top:14px}
.more summary{cursor:pointer;font:700 16px var(--display);letter-spacing:.06em;text-transform:uppercase;color:var(--ink);list-style:none;display:inline-flex;gap:8px;align-items:center;padding:10px 14px;border:2px solid var(--ink);border-radius:4px}
.more summary::-webkit-details-marker{display:none}
.more[open] summary{margin-bottom:6px}

/* Recognition */
.awards{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:10px}
.award{background:var(--surface);border:1px solid var(--line);border-radius:6px;padding:14px;display:grid;gap:6px;align-content:start}
.award .seal{width:38px;height:38px;border-radius:50%;background:var(--yellow);color:var(--yellow-ink);display:grid;place-items:center;font:800 13px var(--display)}
.award b{font:700 18px/1.1 var(--display);text-transform:uppercase}
.award span{font-size:13.5px;color:var(--muted);line-height:1.35}

/* Contact */
.contact{background:var(--navy);color:var(--navy-ink);margin-top:48px;padding-block:36px 40px}
.contact h2{color:var(--yellow)}
.contact-grid{display:grid;gap:16px;margin-top:18px}
.contact .row{display:grid;gap:2px;padding-bottom:14px;border-bottom:1px solid rgba(255,255,255,.18)}
.contact .row:last-child{border-bottom:0}
.contact .k{font:500 12px var(--mono);letter-spacing:.08em;text-transform:uppercase;opacity:.75}
.contact .v{font:700 24px/1.15 var(--display);letter-spacing:.02em;text-decoration:none}
.contact .actions{margin-top:20px}
footer{background:var(--navy);color:var(--navy-ink);opacity:1}
footer .wrap{padding-block:14px 26px;font-size:13px;opacity:.75;border-top:1px solid rgba(255,255,255,.14)}
@media (prefers-reduced-motion:no-preference){.strip{scroll-behavior:smooth}}
</style>

<header class="hero">
  <div class="wrap hero-top">
    <img class="logo" src="img/logo.png" alt="Multimodal Freight logo">
    <div class="parent">A subsidiary of<br>KTMB · Est. 1989</div>
  </div>
  <div class="hero-photo"><img src="img/hero.jpg" alt="Row of MMF prime movers hauling containers"></div>
  <div class="wrap hero-text">
    <h1>Multimodal <span>Freight</span> Sdn Bhd</h1>
    <p class="motto">We deliver your trust</p>
    <p class="lede">Total logistics provider for Malaysia: container haulage, rail-served container depots, warehousing, freight forwarding and licensed Multimodal Transport Operator (MTO) services.</p>
    <div class="actions">
      <a class="btn primary" href="#contact"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.4"><path d="M22 16.9v3a2 2 0 0 1-2.2 2 19.8 19.8 0 0 1-8.6-3.1 19.5 19.5 0 0 1-6-6A19.8 19.8 0 0 1 2.1 4.2 2 2 0 0 1 4.1 2h3a2 2 0 0 1 2 1.7c.1 1 .4 1.9.7 2.8a2 2 0 0 1-.5 2.1L8 9.9a16 16 0 0 0 6 6l1.3-1.3a2 2 0 0 1 2.1-.4c.9.3 1.8.6 2.8.7a2 2 0 0 1 1.7 2z"/></svg>Contact us</a>
      <a class="btn ghost" href="https://drive.google.com/file/d/1n2fFTOTeseU4VcR2TvPiuJ7z3vIsWumR/view?usp=drive_link" target="_blank" rel="noopener"><svg viewBox="0 0 24 24" fill="currentColor"><path d="M8 5v14l11-7z"/></svg>Watch video</a>
    </div>
  </div>
  <div class="hazard"></div>
</header>

<main class="wrap">
  <div class="numbers" aria-label="MMF at a glance">
    <div class="num"><b>36<small>yrs</small></b><span>in Malaysian logistics</span></div>
    <div class="num"><b>6</b><span>branches near major ports</span></div>
    <div class="num"><b>97</b><span>prime movers on the road</span></div>
    <div class="num"><b>621</b><span>20’ &amp; 40’ trailers</span></div>
  </div>

  <section id="about">
    <div class="head">
      <span class="tag">About us</span>
      <h2>Rail-backed logistics since 1989</h2>
    </div>
    <div class="about">
      <div class="about-card">
        <img src="img/hq.jpg" alt="MMF corporate head office building">
        <p>Multimodal Freight Sdn Bhd (MMF) is a wholly-owned subsidiary of <b>Keretapi Tanah Melayu Berhad (KTMB)</b>. We started out serving KTMB’s logistics needs and have grown into a total logistics provider for local and international customers, supported by agents and representatives worldwide.</p>
      </div>
      <div class="timeline">
        <div><b>1989</b>MMF established to serve KTMB’s logistics needs.</div>
        <div><b>2001</b>Accorded Malaysia Multimodal Transport Operator (MTO) status to handle inbound and outbound Government cargo.</div>
        <div><b>2021</b>Two wins at the Kuala Lumpur International Logistics &amp; Transport Awards.</div>
        <div><b>Today</b>Six branches, five rail-served container yards and 142,000 sq ft of warehousing.</div>
      </div>
      <div class="vision"><small>Our vision</small>To be one of the leading integrated logistics solution providers in the logistics industry</div>
      <p class="note" style="margin-top:0">Why MMF: competitive and innovative solutions, without compromising quality and safety.</p>
    </div>
  </section>

  <section id="services">
    <div class="head">
      <span class="tag">What we do</span>
      <h2>Five services, one partner</h2>
      <p>Road, rail, sea and air, handled end to end.</p>
    </div>
    <div class="services">
      <article class="svc">
        <img src="img/fleet.jpg" alt="MMF prime movers lined up">
        <div class="svc-body">
          <div class="svc-top"><h3>Container Haulage</h3><span class="code">MMF-01</span></div>
          <p>One of the pioneers of container haulage in Malaysia, with a fleet deployed by market demand. Drivers are trained under our Road Safety &amp; Driving Program.</p>
          <ul><li>Port Klang</li><li>Pasir Gudang</li><li>20’ &amp; 40’</li><li>Side loaders</li><li>Tippers</li></ul>
        </div>
      </article>
      <article class="svc">
        <img src="img/handler.jpg" alt="Container handler stacking containers at an MMF yard">
        <div class="svc-body">
          <div class="svc-top"><h3>Container Depot</h3><span class="code">MMF-02</span></div>
          <p>Rail-served container yards for empty storage and maintenance &amp; repair, with KTMB Block Train movements between our yards.</p>
          <ul><li>Lift on / lift off</li><li>Maintenance &amp; repair</li><li>Road &amp; rail repositioning</li><li>Transit yard</li></ul>
        </div>
      </article>
      <article class="svc">
        <img src="img/warehouse.jpg" alt="Inside an MMF warehouse with palletised cargo">
        <div class="svc-body">
          <div class="svc-top"><h3>Warehouse &amp; Distribution</h3><span class="code">MMF-03</span></div>
          <p>Non-bonded warehouses at Port Klang and Shah Alam, fully fenced with 24-hour security and access control, close to highways and ports.</p>
          <ul><li>Palletised &amp; loose cargo</li><li>Stuffing / unstuffing</li><li>Under roof &amp; open yard</li><li>Transportation</li></ul>
        </div>
      </article>
      <article class="svc">
        <img src="img/ship.jpg" alt="Container vessel at sea">
        <div class="svc-body">
          <div class="svc-top"><h3>Freight Forwarding</h3><span class="code">MMF-04</span></div>
          <p>Offices close to seaports and airports for fast port and customs clearance, backed by a worldwide agent network for import and export.</p>
          <ul><li>Sea &amp; air freight</li><li>Customs documentation</li><li>Port clearance</li><li>Inland transport</li></ul>
        </div>
      </article>
      <article class="svc">
        <img src="img/loco.jpg" alt="KTMB locomotive being lifted during an MTO project">
        <div class="svc-body">
          <div class="svc-top"><h3>Multimodal Transport Operator</h3><span class="code">MMF-05</span></div>
          <p>Licensed MTO serving corporates and Government agencies, run by our Global Logistics Division (GLD) for complex and heavy project cargo.</p>
          <ul><li>Oil &amp; gas equipment</li><li>Military assets</li><li>Heavy cargo</li><li>Rail &amp; LRT / ETS</li></ul>
        </div>
      </article>
    </div>
  </section>

  <section id="capacity">
    <div class="head">
      <span class="tag">Capacity</span>
      <h2>Fleet &amp; facilities</h2>
    </div>
    <h3 style="font-size:20px;margin-bottom:10px">Haulage fleet</h3>
    <div class="tbl"><table>
      <thead><tr><th>Location</th><th>Prime mover</th><th>Trailer</th><th>Side loader</th><th>Tipper</th></tr></thead>
      <tbody>
        <tr><td>Port Klang</td><td>57</td><td>382</td><td>14</td><td>2</td></tr>
        <tr><td>Pasir Gudang</td><td>40</td><td>239</td><td>5</td><td>5</td></tr>
      </tbody>
      <tfoot><tr><td>Total</td><td>97</td><td>621</td><td>19</td><td>7</td></tr></tfoot>
    </table></div>

    <h3 style="font-size:20px;margin:24px 0 10px">Container depots</h3>
    <div class="tbl"><table>
      <thead><tr><th>Yard</th><th>Size</th><th>Capacity</th></tr></thead>
      <tbody>
        <tr><td>Padang Besar</td><td>12 acres</td><td>2,500 TEUs</td></tr>
        <tr><td>Butterworth (PCT1)</td><td>5 acres</td><td>1,500 TEUs</td></tr>
        <tr><td>Butterworth (PCT2)</td><td>7 acres</td><td>1,800 TEUs</td></tr>
        <tr><td>Port Klang</td><td>4.5 acres</td><td>1,000 TEUs</td></tr>
        <tr><td>Pasir Gudang</td><td>7 acres</td><td>1,500 TEUs</td></tr>
      </tbody>
      <tfoot><tr><td>Total</td><td>35.5 acres</td><td>8,300 TEUs</td></tr></tfoot>
    </table></div>

    <h3 style="font-size:20px;margin:24px 0 10px">Warehouses</h3>
    <div class="tbl"><table>
      <thead><tr><th>Location</th><th>Type</th><th>Size</th></tr></thead>
      <tbody>
        <tr><td>Port Klang</td><td>Non-bonded</td><td>42,000 sq ft</td></tr>
        <tr><td>Shah Alam</td><td>Non-bonded</td><td>100,000 sq ft</td></tr>
      </tbody>
    </table></div>
    <p class="note">All container yards are rail served, so customers can choose road or rail.</p>
  </section>

  <section id="network">
    <div class="head">
      <span class="tag">Our network · north to south</span>
      <h2>Along the KTMB line</h2>
      <p>Branches sit at Malaysia’s major ports and rail terminals, from the Thai border to Johor.</p>
    </div>
    <div class="line">
      <div class="stn">
        <span class="tag">Perlis</span><h3>Padang Besar</h3>
        <div class="facts"><span><b>Depot</b> 12 acres · 2,500 TEUs</span><span>Container Freight Station</span></div>
        <a class="tel" href="tel:+6049490749">04-949 0749</a>
      </div>
      <div class="stn">
        <span class="tag">Pulau Pinang</span><h3>Butterworth</h3>
        <div class="facts"><span><b>Depots</b> PCT1 &amp; PCT2 · 3,300 TEUs</span><span>Freight forwarding</span></div>
        <a class="tel" href="tel:+6043325533">04-332 5533</a>
      </div>
      <div class="stn hq">
        <span class="tag">Selangor · Corporate head office</span><h3>Glenmarie, Shah Alam</h3>
        <div class="facts"><span><b>Warehouse</b> 100,000 sq ft</span><span>Global Logistics Division (GLD): 03-5510 0424</span></div>
        <a class="tel" href="tel:+60355618100">03-5561 8100</a>
      </div>
      <div class="stn">
        <span class="tag">Selangor</span><h3>Port Klang</h3>
        <div class="facts"><span><b>Haulage</b> 57 prime movers</span><span><b>Warehouse</b> 42,000 sq ft</span><span><b>Depot</b> 1,000 TEUs</span></div>
        <a class="tel" href="tel:+60331654920">03-3165 4920</a>
      </div>
      <div class="stn" style="padding-bottom:0">
        <span class="tag">Johor</span><h3>Pasir Gudang</h3>
        <div class="facts"><span><b>Haulage</b> 40 prime movers</span><span><b>Depot</b> 7 acres · 1,500 TEUs</span></div>
        <a class="tel" href="tel:+6072529200">07-252 9200</a>
      </div>
    </div>
  </section>

  <section id="gallery">
    <div class="head">
      <span class="tag">On the ground</span>
      <h2>See us at work</h2>
    </div>
    <div class="strip" tabindex="0" aria-label="Photo gallery, scroll sideways">
      <figure><img src="img/railyard.jpg" alt="Container train at a rail yard" loading="lazy"><figcaption>Rail-served container yards</figcaption></figure>
      <figure><img src="img/ets.jpg" alt="ETS train set being lifted at port" loading="lazy"><figcaption>Shipment of the first new ETS for KTMB</figcaption></figure>
      <figure><img src="img/air.jpg" alt="Heavy turbine parts loaded into a cargo aircraft" loading="lazy"><figcaption>TNB turbine parts flown to Berlin</figcaption></figure>
      <figure><img src="img/depot.jpg" alt="Stacked containers at depot" loading="lazy"><figcaption>Container storage &amp; repair</figcaption></figure>
      <figure><img src="img/racks.jpg" alt="Warehouse racking" loading="lazy"><figcaption>Shah Alam warehouse</figcaption></figure>
      <figure><img src="img/team.jpg" alt="MMF drivers and crew in front of trucks" loading="lazy"><figcaption>Our trained haulage crew</figcaption></figure>
    </div>
  </section>

  <section id="projects">
    <div class="head">
      <span class="tag">Track record</span>
      <h2>Trusted with the hard moves</h2>
      <p>Main customers include MINDEF and KTMB. Selected MTO and project cargo work:</p>
    </div>
    <div class="projects">
      <div class="prj"><span class="yr">2025</span><div><b>CRRC Corporation</b><span>Light Rail Vehicles (LRV) for the RTS project</span></div></div>
      <div class="prj"><span class="yr">2024</span><div><b>Tenaga Nasional Berhad</b><span>1000MW steam turbine IP rotor and inner casings, Janamanjung to GE Power, Berlin</span></div></div>
      <div class="prj"><span class="yr">2024</span><div><b>RTM</b><span>Radio broadcasting automation equipment and systems</span></div></div>
      <div class="prj"><span class="yr">Ongoing</span><div><b>MINDEF</b><span>Military items, equipment and army household moves, Peninsular to Sabah &amp; Sarawak</span></div></div>
      <div class="prj"><span class="yr">2017</span><div><b>Marubeni Corporation</b><span>5 sets of ETS component equipment from Japan</span></div></div>
      <div class="prj"><span class="yr">2011–12</span><div><b>Ministry of Transport</b><span>38 Electric Multiple Units, Port Klang to KTMB Batu Gajah</span></div></div>
    </div>
    <details class="more">
      <summary>+ More projects</summary>
      <div class="projects">
        <div class="prj"><span class="yr">2016–18</span><div><b>TWA (Malaysia)</b><span>33 KTMB maintenance machines from Plasser &amp; Theurer, Germany</span></div></div>
        <div class="prj"><span class="yr">2017–18</span><div><b>System Enhancement &amp; Resources Technology</b><span>35 motor trolleys from Korea to Shah Alam</span></div></div>
        <div class="prj"><span class="yr">2016–17</span><div><b>DMIA</b><span>25 m rail track for the Klang Valley Double Tracking Project, China to KTMB Serendah</span></div></div>
        <div class="prj"><span class="yr">—</span><div><b>Scania (M)</b><span>162 RapidKL buses</span></div></div>
        <div class="prj"><span class="yr">—</span><div><b>KTMB</b><span>Relocation of Tanjung Pagar (Singapore) rail tracks; Blue Coach rail set from Japan</span></div></div>
        <div class="prj"><span class="yr">—</span><div><b>MMC-Gamuda KVMRT</b><span>MRT underground works package; EDTP rail equipment Ipoh to Padang Besar</span></div></div>
        <div class="prj"><span class="yr">—</span><div><b>Meiden-Meidensha JV · Otis Elevator</b><span>MRT power supply, signalling and communications equipment</span></div></div>
        <div class="prj"><span class="yr">—</span><div><b>Ircon International</b><span>EDTP rail equipment, Seremban to Gemas</span></div></div>
        <div class="prj"><span class="yr">—</span><div><b>NSTP</b><span>Newsprint and printed material</span></div></div>
      </div>
    </details>
  </section>

  <section id="recognition">
    <div class="head">
      <span class="tag">Recognition</span>
      <h2>Awards &amp; certification</h2>
    </div>
    <div class="awards">
      <div class="award"><div class="seal">2021</div><b>Multimodal Transport Operator Award</b><span>KL International Logistics &amp; Transport Awards</span></div>
      <div class="award"><div class="seal">2021</div><b>Best Cross-Border Logistics Provider</b><span>KL International Logistics &amp; Transport Awards</span></div>
      <div class="award"><div class="seal">MOF</div><b>Bumiputera Company</b><span>Registered with the Ministry of Finance Malaysia</span></div>
      <div class="award"><div class="seal">✓</div><b>Halal Certified</b><span>Sijil Pengesahan Halal Malaysia</span></div>
    </div>
  </section>
</main>

<section class="contact" id="contact">
  <div class="wrap">
    <span class="tag" style="color:var(--yellow)">Talk to us</span>
    <h2>Get a quote</h2>
    <div class="contact-grid">
      <div class="row"><span class="k">Corporate head office · Glenmarie, Shah Alam</span><a class="v" href="tel:+60355618100">03-5561 8100</a></div>
      <div class="row"><span class="k">Global Logistics Division (MTO projects)</span><a class="v" href="tel:+60355100424">03-5510 0424</a></div>
      <div class="row"><span class="k">Website</span><a class="v" href="http://www.multimodal.com.my" target="_blank" rel="noopener">multimodal.com.my</a></div>
      <div class="row"><span class="k">Instagram · Facebook</span><span class="v">@mmf.official · Multimodal Freight Sdn Bhd</span></div>
    </div>
    <div class="actions">
      <a class="btn primary" href="http://www.multimodal.com.my" target="_blank" rel="noopener">Visit website</a>
      <a class="btn ghost" href="https://www.instagram.com/mmf.official/" target="_blank" rel="noopener">Instagram</a>
    </div>
  </div>
</section>
<footer><div class="wrap">Multimodal Freight Sdn Bhd (174274-D) · A member of the KTMB Group</div></footer>

</body></html>
