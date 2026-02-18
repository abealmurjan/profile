<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Ibrahim Al-Murjan — Global VP of Product. 18 years building products, teams, and platforms that scale across 2,500+ locations.">
<title>Ibrahim Al-Murjan — Global VP of Product</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;1,9..40,300;1,9..40,400&display=swap" rel="stylesheet">
<style>
/* ============================================
   MOBILE-FIRST · WCAG CONTRAST-SAFE
   ============================================ */
*, *::before, *::after { margin:0; padding:0; box-sizing:border-box; }
html { scroll-behavior:smooth; -webkit-text-size-adjust:100%; }
body { font-family:'DM Sans',-apple-system,BlinkMacSystemFont,sans-serif; background:#0C0C0E; color:#E8E4DC; line-height:1.6; overflow-x:hidden; -webkit-font-smoothing:antialiased; }
img { max-width:100%; height:auto; display:block; }
a { color:inherit; }
::selection { background:#D4A853; color:#0C0C0E; }
:root {
  --bg:#0C0C0E; --bg2:#141418; --bg3:#1A1A20;
  --c1:#E8E4DC; --c2:#B5AFA5; --c3:#8A847A;
  --gold:#E0B45C; --gold-dim:rgba(224,180,92,0.12); --gold-glow:rgba(224,180,92,0.25);
  --line:rgba(232,228,220,0.08);
  --serif:'Instrument Serif',Georgia,serif; --sans:'DM Sans',sans-serif;
}
.wrap { width:100%; max-width:1200px; margin:0 auto; padding:0 20px; }
.sec { padding:48px 0; }

/* --- Nav --- */
.nav { position:fixed; top:0; left:0; right:0; z-index:100; padding:14px 0;
  background:rgba(12,12,14,0.85); backdrop-filter:blur(20px); -webkit-backdrop-filter:blur(20px);
  border-bottom:1px solid var(--line); }
.nav .wrap { display:flex; justify-content:space-between; align-items:center; }
.nav-logo { font-family:var(--serif); font-size:1.25rem; text-decoration:none; color:var(--c1); z-index:102; position:relative; }
.nav-logo span { color:var(--gold); }
.nav-menu { display:none; }
.nav-btn { background:none; border:none; cursor:pointer; width:24px; height:18px; position:relative; z-index:102; }
.nav-btn span { display:block; width:100%; height:2px; background:var(--c1); position:absolute; left:0; transition:all 0.3s; }
.nav-btn span:nth-child(1){top:0} .nav-btn span:nth-child(2){top:8px} .nav-btn span:nth-child(3){top:16px}
.nav-btn.on span:nth-child(1){top:8px;transform:rotate(45deg)} .nav-btn.on span:nth-child(2){opacity:0} .nav-btn.on span:nth-child(3){top:8px;transform:rotate(-45deg)}
.nav-ov { display:none; position:fixed; inset:0; z-index:101; background:rgba(12,12,14,0.98);
  flex-direction:column; justify-content:center; align-items:center; gap:28px; }
.nav-ov.on { display:flex; }
.nav-ov a { color:var(--c2); text-decoration:none; font-size:1.15rem; letter-spacing:0.04em; text-transform:uppercase; transition:color 0.3s; }
.nav-ov a:hover { color:var(--gold); }
.pill { background:var(--gold)!important; color:var(--bg)!important; padding:12px 28px; border-radius:100px; font-weight:500; text-transform:none!important; font-size:1rem!important; }

/* --- Buttons --- */
.btn-g { display:inline-flex; align-items:center; justify-content:center; gap:8px;
  background:var(--gold); color:var(--bg); padding:14px 28px; border-radius:100px;
  text-decoration:none; font-weight:500; font-size:0.95rem; transition:transform 0.3s,box-shadow 0.3s; border:none; cursor:pointer; }
.btn-g:hover { transform:translateY(-2px); box-shadow:0 8px 24px var(--gold-glow); }
.btn-o { display:inline-flex; align-items:center; justify-content:center; gap:8px;
  background:transparent; color:var(--c1); padding:14px 28px; border-radius:100px;
  text-decoration:none; font-size:0.95rem; border:1px solid rgba(232,228,220,0.2); transition:all 0.3s; }
.btn-o:hover { border-color:var(--gold); color:var(--gold); }

/* --- Hero --- */
.hero { padding-top:80px; padding-bottom:32px; }
.hero-ey { display:inline-flex; align-items:center; gap:8px; font-size:0.75rem;
  text-transform:uppercase; letter-spacing:0.15em; color:var(--gold); font-weight:500; margin-bottom:16px; }
.hero-ey::before { content:''; width:20px; height:1px; background:var(--gold); }
.hero h1 { font-family:var(--serif); font-size:2.2rem; line-height:1.08; letter-spacing:-0.03em; margin-bottom:20px; }
.hero h1 em { font-style:italic; color:var(--gold); }
.hero-desc { font-size:0.95rem; color:var(--c2); line-height:1.7; margin-bottom:28px; }
.hero-btns { display:flex; flex-direction:column; gap:12px; }
.hero-photo { margin-top:32px; position:relative; width:100%; max-width:260px; }
.hero-photo img { width:100%; aspect-ratio:4/5; object-fit:cover; border-radius:16px; border:1px solid var(--line); }
.hero-photo::after { content:''; position:absolute; inset:0; border-radius:16px;
  background:linear-gradient(180deg,transparent 50%,rgba(12,12,14,0.5)); pointer-events:none; }
.bdg { position:absolute; background:var(--bg3); border:1px solid var(--line); border-radius:12px; padding:10px 16px; z-index:2; }
.bdg-l { font-size:0.6rem; text-transform:uppercase; letter-spacing:0.1em; color:var(--c3); }
.bdg-v { font-family:var(--serif); font-size:1.1rem; color:var(--gold); }
.bdg-a { bottom:-12px; left:-8px; }
.bdg-y { position:absolute; top:-10px; right:-8px; background:var(--gold); color:var(--bg); border-radius:10px; padding:10px 14px; text-align:center; z-index:2; }
.bdg-y .n { font-family:var(--serif); font-size:1.3rem; display:block; line-height:1; }
.bdg-y .l { font-size:0.55rem; text-transform:uppercase; letter-spacing:0.06em; opacity:0.8; }

/* --- Stats --- */
.stats { border-top:1px solid var(--line); border-bottom:1px solid var(--line); padding:36px 0; }
.stats-r { display:grid; grid-template-columns:1fr 1fr; gap:24px; text-align:center; }
.sn { font-family:var(--serif); font-size:1.8rem; color:var(--gold); display:block; line-height:1; margin-bottom:4px; }
.sl { font-size:0.7rem; color:var(--c2); text-transform:uppercase; letter-spacing:0.08em; }

/* --- Section headers --- */
.se { display:inline-flex; align-items:center; gap:8px; font-size:0.7rem; text-transform:uppercase;
  letter-spacing:0.15em; color:var(--gold); font-weight:500; margin-bottom:12px; }
.se::before { content:''; width:20px; height:1px; background:var(--gold); }
.st { font-family:var(--serif); font-size:1.8rem; letter-spacing:-0.02em; line-height:1.1; margin-bottom:36px; }
.st em { font-style:italic; color:var(--gold); }

/* --- About --- */
.ab p { font-size:0.95rem; color:var(--c2); line-height:1.8; margin-bottom:16px; }
.ab p:first-of-type::first-letter { font-family:var(--serif); font-size:3rem; float:left; color:var(--gold); line-height:1; margin-right:10px; margin-top:4px; }
.sk { display:grid; grid-template-columns:1fr; gap:12px; margin-top:32px; }
.skc { background:var(--bg2); border:1px solid var(--line); border-radius:12px; padding:18px; }
.ski { width:32px; height:32px; background:var(--gold-dim); border-radius:8px;
  display:flex; align-items:center; justify-content:center; margin-bottom:10px; color:var(--gold); }
.skc h4 { font-family:var(--serif); font-size:1rem; margin-bottom:4px; }
.skc p { font-size:0.8rem; color:var(--c3); line-height:1.5; }

/* --- Portfolio --- */
.pf-sec { background:var(--bg2); }
.pc { background:var(--bg3); border:1px solid var(--line); border-radius:16px; overflow:hidden; margin-bottom:24px; transition:transform 0.4s,box-shadow 0.4s; }
.pc:hover { transform:translateY(-3px); box-shadow:0 16px 48px rgba(0,0,0,0.3); }
.pt { padding:24px; }
.ptag { font-size:0.65rem; text-transform:uppercase; letter-spacing:0.12em; color:var(--gold); font-weight:500; margin-bottom:10px; }
.pc h3 { font-family:var(--serif); font-size:1.3rem; letter-spacing:-0.02em; margin-bottom:12px; line-height:1.15; }
.pc p { color:var(--c2); font-size:0.88rem; line-height:1.7; margin-bottom:20px; }
.pn { display:flex; flex-wrap:wrap; gap:16px; padding-top:16px; border-top:1px solid var(--line); }
.pn .v { font-family:var(--serif); font-size:1.2rem; color:var(--gold); display:block; line-height:1.1; }
.pn .l { font-size:0.65rem; color:var(--c3); text-transform:uppercase; letter-spacing:0.06em; }
.pg { background:var(--bg); padding:16px; overflow-x:auto; -webkit-overflow-scrolling:touch; scrollbar-width:none; position:relative; }
.pg::-webkit-scrollbar { display:none; }
.pg::before { content:''; position:absolute; inset:0; background:radial-gradient(ellipse at 50% 50%,var(--gold-dim),transparent 70%); opacity:0.3; pointer-events:none; }
.gr { display:flex; gap:12px; }
.gr img { flex:0 0 auto; width:55vw; max-width:280px; border-radius:12px;
  border:1px solid rgba(255,255,255,0.06); box-shadow:0 8px 32px rgba(0,0,0,0.4);
  transition:transform 0.3s; position:relative; z-index:1; }
.gr img:hover { transform:translateY(-4px); }
.sh { text-align:center; padding:8px 0 4px; font-size:0.65rem; color:var(--c3);
  text-transform:uppercase; letter-spacing:0.08em; position:relative; z-index:1; }

/* --- Timeline --- */
.tl { position:relative; padding-left:24px; }
.tl::before { content:''; position:absolute; left:0; top:0; bottom:0; width:1px;
  background:linear-gradient(180deg,var(--gold),var(--line),transparent); }
.ti { position:relative; padding-bottom:40px; }
.ti::before { content:''; position:absolute; left:-28px; top:6px; width:8px; height:8px;
  border-radius:50%; background:var(--gold); box-shadow:0 0 0 3px var(--bg),0 0 0 4px var(--gold); }
.td { font-size:0.7rem; text-transform:uppercase; letter-spacing:0.1em; color:var(--gold); font-weight:500; margin-bottom:6px; }
.ti h3 { font-family:var(--serif); font-size:1.15rem; margin-bottom:3px; }
.ti h4 { font-size:0.85rem; color:var(--c2); font-weight:400; margin-bottom:10px; }
.ti p { font-size:0.85rem; color:var(--c3); line-height:1.7; }

/* --- Education --- */
.edu-grid { display:grid; grid-template-columns:1fr; gap:16px; margin-top:32px; }
.edu-card { background:var(--bg2); border:1px solid var(--line); border-radius:12px; padding:20px; }
.edu-deg { font-family:var(--serif); font-size:1.05rem; color:var(--c1); margin-bottom:4px; }
.edu-school { font-size:0.82rem; color:var(--gold); margin-bottom:4px; }
.edu-detail { font-size:0.78rem; color:var(--c3); line-height:1.5; }

/* --- Extras bar --- */
.extras { display:flex; flex-wrap:wrap; gap:8px; margin-top:20px; }
.ext-tag { background:var(--gold-dim); color:var(--gold); font-size:0.7rem; padding:6px 14px;
  border-radius:100px; font-weight:500; letter-spacing:0.02em; }

/* --- Testimonials --- */
.tg { display:grid; grid-template-columns:1fr; gap:16px; }
.tc { background:var(--bg2); border:1px solid var(--line); border-radius:16px; padding:24px; position:relative; }
.tc::before { content:'\201C'; font-family:var(--serif); font-size:3.5rem; color:var(--gold-dim); position:absolute; top:8px; left:18px; line-height:1; }
.tc blockquote { font-size:0.88rem; color:var(--c2); line-height:1.75; margin-bottom:20px; font-style:italic; position:relative; z-index:1; }
.tw { display:flex; align-items:center; gap:10px; }
.tav { width:36px; height:36px; border-radius:50%; background:var(--gold-dim);
  display:flex; align-items:center; justify-content:center; color:var(--gold); font-family:var(--serif); font-size:0.9rem; flex-shrink:0; }
.tn { font-weight:500; font-size:0.85rem; }
.tr { font-size:0.72rem; color:var(--c3); }

/* --- CTA --- */
.cta { text-align:center; }
.cta .st { max-width:600px; margin:0 auto 16px; }
.cta-sub { color:var(--c2); margin-bottom:32px; font-size:0.95rem; }
.cta-b { display:flex; flex-direction:column; align-items:center; gap:12px; }

/* --- Footer --- */
.ft { border-top:1px solid var(--line); padding:32px 0; text-align:center; }
.ft p { color:var(--c3); font-size:0.75rem; }

/* --- Animations --- */
.an { opacity:0; transform:translateY(24px); transition:opacity 0.6s ease,transform 0.6s ease; }
.an.vi { opacity:1; transform:translateY(0); }
.d1{transition-delay:.1s} .d2{transition-delay:.2s} .d3{transition-delay:.3s}

/* ============================================ TABLET ============================================ */
@media(min-width:600px){
  .wrap{padding:0 32px} .sec{padding:64px 0}
  .hero h1{font-size:2.8rem} .hero-btns{flex-direction:row} .hero-photo{max-width:300px}
  .stats-r{grid-template-columns:repeat(4,1fr)} .sn{font-size:2.2rem} .sl{font-size:0.75rem}
  .sk{grid-template-columns:1fr 1fr} .st{font-size:2.2rem}
  .pt{padding:32px} .pc h3{font-size:1.5rem}
  .gr img{width:40vw;max-width:300px} .sh{display:none}
  .tg{grid-template-columns:1fr 1fr} .cta-b{flex-direction:row;justify-content:center}
  .edu-grid{grid-template-columns:1fr 1fr}
}
/* ============================================ DESKTOP ============================================ */
@media(min-width:960px){
  .wrap{padding:0 48px} .sec{padding:96px 0}
  .nav-btn{display:none}
  .nav-menu{display:flex;gap:28px;align-items:center}
  .nav-menu a{color:var(--c2);text-decoration:none;font-size:0.8rem;letter-spacing:0.04em;text-transform:uppercase;transition:color 0.3s}
  .nav-menu a:hover{color:var(--gold)}
  .nav-menu .pill{background:var(--gold);color:var(--bg);padding:10px 22px;border-radius:100px;font-weight:500;text-transform:none;font-size:0.85rem;transition:transform 0.3s,box-shadow 0.3s}
  .nav-menu .pill:hover{transform:translateY(-1px);box-shadow:0 4px 16px var(--gold-glow)}
  .hero-inner{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
  .hero{padding-top:100px;padding-bottom:48px}
  .hero h1{font-size:clamp(2.8rem,4.5vw,4.2rem)} .hero-desc{font-size:1.05rem}
  .hero-photo{margin-top:0;max-width:360px}
  .bdg-a{bottom:-16px;left:-24px;padding:14px 20px} .bdg-v{font-size:1.3rem}
  .bdg-y{top:-14px;right:-16px;padding:12px 18px} .bdg-y .n{font-size:1.5rem}
  .about-inner{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:start}
  .ab p{font-size:1.02rem}
  .pt{padding:40px} .pc h3{font-size:1.7rem} .pc p{font-size:0.92rem}
  .gr img{width:auto;max-width:none;height:380px} .pg{padding:28px}
  .sn{font-size:2.8rem} .sl{font-size:0.8rem}
  .st{font-size:2.8rem;margin-bottom:48px}
  .tc{padding:36px} .tc blockquote{font-size:0.95rem}
  .tl{padding-left:32px} .ti h3{font-size:1.35rem}
}
@media(min-width:1200px){
  .hero h1{font-size:4.2rem} .gr img{height:420px} .pg{padding:36px}
}
</style>
</head>
<body>

<nav class="nav"><div class="wrap">
  <a href="#" class="nav-logo">abe<span>.</span></a>
  <div class="nav-menu">
    <a href="#about">About</a><a href="#portfolio">Portfolio</a><a href="#experience">Experience</a><a href="#refs">References</a>
    <a href="mailto:abealmurjan@gmail.com" class="pill">Let's Connect</a>
  </div>
  <button class="nav-btn" id="nb" aria-label="Menu"><span></span><span></span><span></span></button>
</div></nav>
<div class="nav-ov" id="no">
  <a href="#about">About</a><a href="#portfolio">Portfolio</a><a href="#experience">Experience</a><a href="#refs">References</a>
  <a href="mailto:abealmurjan@gmail.com" class="pill">Let's Connect</a>
</div>

<!-- ========== HERO ========== -->
<section class="hero sec"><div class="wrap"><div class="hero-inner">
  <div>
    <div class="hero-ey">Global VP of Product</div>
    <h1>18 years building<br><em>products & teams</em><br>that scale</h1>
    <p class="hero-desc">I'm Ibrahim Al-Murjan. I build and scale digital platforms and the teams behind them — across 2,500+ locations in North America, Europe, and Asia. Consumer apps, AI-powered clinical tools, enterprise systems. From zero to millions of users, from first hire to 62-person global org.</p>
    <div class="hero-btns">
      <a href="mailto:abealmurjan@gmail.com" class="btn-g">✉ Get in Touch</a>
      <a href="https://www.linkedin.com/in/abealmurjan/" target="_blank" class="btn-o">LinkedIn</a>
    </div>
  </div>
  <div class="hero-photo">
    <img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/7bc9c342-47bf-48e0-bd09-e07d94b646dc/5+-+Abe.jpeg" alt="Ibrahim Al-Murjan" width="360" height="450">
    <div class="bdg bdg-a"><div class="bdg-l">Award</div><div class="bdg-v">Mars Global<br>Innovation Winner</div></div>
    <div class="bdg-y"><span class="n">18+</span><span class="l">Years in Product</span></div>
  </div>
</div></div></section>

<!-- ========== STATS ========== -->
<div class="stats"><div class="wrap"><div class="stats-r">
  <div class="an"><span class="sn">2M+</span><span class="sl">App Users</span></div>
  <div class="an d1"><span class="sn">1.5M+</span><span class="sl">AI Dictations Processed</span></div>
  <div class="an d2"><span class="sn">$110M</span><span class="sl">Portfolio Managed</span></div>
  <div class="an d3"><span class="sn">4.8★</span><span class="sl">User Satisfaction</span></div>
</div></div></div>

<!-- ========== ABOUT ========== -->
<section id="about" class="sec"><div class="wrap"><div class="about-inner">
  <div class="ab an">
    <div class="se">Background</div>
    <h2 class="st">How I <em>work</em></h2>
    <p>I started on the ground floor — training hospital teams on software across 18 states, learning every operational pain point firsthand. That shaped how I approach product: start with the real problem, build for the people using it, measure what matters.</p>
    <p>Since then I've gone from program leader to Global VP of Product, building a 62-person team across product, design, engineering, and operations. I manage a $110M annual portfolio spanning consumer apps, AI clinical tools, telehealth, and enterprise workflow systems across 2,500+ locations globally. I've shipped products in as little as 6 weeks and scaled them to millions of users.</p>
    <p>Graduate of the University of Denver — M.A. in Global Finance & Trade from the Korbel School of International Studies, B.S. in Business Information Technology from Daniels College of Business. Fluent in English and Arabic.</p>
  </div>
  <div class="an d2"><div class="sk">
    <div class="skc"><div class="ski">⚡</div><h4>0 → 1 Launches</h4><p>Multiple products from concept to production — including an AI dictation tool shipped in 6 weeks.</p></div>
    <div class="skc"><div class="ski">📐</div><h4>Team Builder</h4><p>Built product and engineering departments from scratch. Grew a 62-person global org with clear KPIs.</p></div>
    <div class="skc"><div class="ski">↗</div><h4>Global Scale</h4><p>Products deployed across 2,500+ locations in North America, Europe, and Asia serving millions of users.</p></div>
    <div class="skc"><div class="ski">◉</div><h4>AI in Production</h4><p>Shipped AI dictation, triage, and decision-support tools in regulated healthcare — with human-in-the-loop safeguards.</p></div>
  </div></div>
</div></div></section>

<!-- ========== PORTFOLIO ========== -->
<section id="portfolio" class="sec pf-sec"><div class="wrap">
  <div class="se">Product Portfolio</div>
  <h2 class="st">What I've <em>shipped</em></h2>

  <!-- myVCA -->
  <div class="pc an"><div class="pt"><div class="ptag">Consumer Mobile App</div><h3>Consumer Healthcare App</h3><p>Consumer mobile app for a 1,000+ location veterinary network. Handles check-in, document signing, Text to Pay digital checkout (powering $1B+ in payment collection), and 24/7 care access. Grew to over 2M active users with a 4.8-star rating.</p><div class="pn"><div><span class="v">2M+</span><span class="l">Active Users</span></div><div><span class="v">$1B+</span><span class="l">Payments Processed</span></div><div><span class="v">4.8★</span><span class="l">App Store Rating</span></div></div></div>
  <div class="pg"><div class="gr"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/29c98f01-9696-4ad4-a6d2-28f03ebef127/myvca-1.jpg" alt="myVCA Home" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/d553794d-a360-45c9-b5b5-35a8f90de84a/myvca-2.jpg" alt="myVCA Profile" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/b1a24247-615c-465a-a4af-dbc7aea42ccd/myvca-4.jpg" alt="myVCA Features" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/faaae44c-9df9-4627-9524-913c66503bba/myvca-4+%281%29.jpg" alt="myVCA Checkout" loading="lazy"></div><div class="sh">← Swipe to see more →</div></div></div>

  <!-- Scribe AI -->
  <div class="pc an"><div class="pt"><div class="ptag">AI-Powered Clinical Tool</div><h3>AI Medical Dictation</h3><p>AI-powered dictation tool that replaced manual medical record writing. Veterinarians dictate, the system transcribes and pushes structured SOAP notes directly into the practice management system. Cut documentation time by 90%, drove a 30% increase in clinical efficiency, and went from concept to production in 6 weeks. Over 1.5M dictations processed in the field — one of the first production AI tools in veterinary medicine.</p><div class="pn"><div><span class="v">1.5M+</span><span class="l">Dictations Processed</span></div><div><span class="v">30%</span><span class="l">Efficiency Gain</span></div><div><span class="v">6 wks</span><span class="l">Concept to Launch</span></div></div></div>
  <div class="pg"><div class="gr"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/52c4c0f5-494d-4a0a-b471-40533a7a1678/scribe+-+1.jpg" alt="Scribe Dictation" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/cb27256c-121c-4db8-ab77-2e00219b07e9/scribe+-+2.jpg" alt="Scribe Transcription" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/be26933b-e195-44c9-8c71-673f638a1f54/scribe+-+3.jpg" alt="Scribe Records" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/63ee0a82-1c52-4c4d-9b60-a5919a0a4350/scribe+-+4.jpg" alt="Scribe Dashboard" loading="lazy"></div><div class="sh">← Swipe to see more →</div></div></div>

  <!-- Telehealth -->
  <div class="pc an"><div class="pt"><div class="ptag">Virtual Care Platform</div><h3>Telehealth & Live Chat</h3><p>In-app teletriage chat launched in 2018, expanded to full video and 24/7 access in 2020 as a critical part of the pandemic response. Available to over 1M+ clients across the network. Omnichannel — web and mobile, integrated with medical records and real-time clinical data.</p><div class="pn"><div><span class="v">1M+</span><span class="l">Clients with Access</span></div><div><span class="v">24/7</span><span class="l">Around-the-Clock</span></div><div><span class="v">4.8★</span><span class="l">Client Satisfaction</span></div></div></div>
  <div class="pg"><div class="gr"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/01657c15-227d-4558-a55d-fd1d7c59a0f1/telehealth-1.jpg" alt="Telehealth" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/710bce2c-bdc2-451e-9846-2974f70ce605/telehealth-2.jpg" alt="Live Chat" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/2246e5d4-91f3-4d9a-9ef6-d92face85ead/telehealth-3.jpg" alt="Chat View" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/9fa280a2-e1c6-49ae-a83e-1bbbef890caa/telehealth-4.jpg" alt="Video Call" loading="lazy"></div><div class="sh">← Swipe to see more →</div></div></div>

  <!-- Staff Enablement -->
  <div class="pc an"><div class="pt"><div class="ptag">Operational Efficiency & Privacy</div><h3>Staff Enablement & Direct Messaging</h3><p>Mobile staff platform paired with a 2-way SMS system for client communication — launched in 2014, before most healthcare orgs had a direct messaging strategy. Gave clients the instant access they expect while protecting employee personal phone numbers and work-life boundaries. Digitized front-desk workflows, eliminated paper processes, and became the primary engagement channel across the network.</p><div class="pn"><div><span class="v">5M+</span><span class="l">Client Engagements</span></div><div><span class="v">75M+</span><span class="l">Messages Exchanged</span></div><div><span class="v">10M+</span><span class="l">Paper Forms Eliminated</span></div></div></div>
  <div class="pg"><div class="gr"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/7a638a63-9496-4127-8825-15e18438d58d/companion-1.jpg" alt="Retriever+" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/6df8c33d-a24c-4ebb-9c3e-c6078fe5f6b6/companion-2.jpg" alt="Retriever+ Docs" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/d6f14579-5759-409c-bb5e-4037aa4563b1/companion-4.jpg" alt="Dashboard" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/71581fce-b299-4e2f-8cc6-d25b03e322b5/sms-1.jpg" alt="SMS" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/f92b351c-a683-44e1-b590-76fa7eec72fa/sms-2.jpg" alt="SMS Thread" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/bd249175-3787-4866-86fe-2ddf991a2b37/sms-3.jpg" alt="SMS Photos" loading="lazy"></div><div class="sh">← Swipe to see more →</div></div></div>

  <!-- Virtual Waiting Room -->
  <div class="pc an"><div class="pt"><div class="ptag">ER & Urgent Care Operations</div><h3>Virtual Waiting Room</h3><p>Automated queue management system deployed across the ER and Urgent Care hospital network. Clients check in digitally, see real-time wait estimates, and receive status updates — reducing lobby crowding and walk-away rates. Less stress on clients waiting with sick pets, less pressure on front-desk staff managing an unpredictable queue. Drove a 20% revenue lift by keeping clients in the funnel.</p><div class="pn"><div><span class="v">1,000+</span><span class="l">ER/Urgent Care Hospitals</span></div><div><span class="v">20%</span><span class="l">Revenue Lift</span></div><div><span class="v">Real-time</span><span class="l">Queue Management</span></div></div></div>
  <div class="pg"><div class="gr"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/4c434f2b-fb19-4f47-b7e1-75c6f1a9f84d/urgent-1.jpg" alt="Waiting Room" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/1705092307180-P9QXHGG8ZNW7TRFNU02X/urgent-4%2B%25281%2529.jpg" alt="Queue" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/f5b30b68-4834-4c73-b0b8-197f70487a7b/image000001.jpg" alt="Live View" loading="lazy"></div><div class="sh">← Swipe to see more →</div></div></div>

  <!-- Student Concierge -->
  <div class="pc an"><div class="pt"><div class="ptag">Talent Pipeline & Operations</div><h3>Student Concierge</h3><p>Scheduling, capacity, and placement platform for veterinary externs. Replaced manual hospital-by-hospital coordination with centralized matching. Integrated with Workday and ServiceNow. Built a talent pipeline that converted 80% of placed externs into full-time hires.</p><div class="pn"><div><span class="v">2,000+</span><span class="l">Students Placed</span></div><div><span class="v">80%</span><span class="l">Hire Conversion</span></div></div></div>
  <div class="pg"><div class="gr"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/ef1ddd55-8b06-459f-a577-f4850690d033/student+-+4.jpg" alt="Student Portal" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/1530ba7a-d921-4d92-b953-47808d4c618e/student+-+5.jpg" alt="Scheduling" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/e3a3a981-19c7-4c31-8bac-e89a0756f7c3/student+-+6.jpg" alt="Placement" loading="lazy"><img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/7c00dc03-e704-496f-9070-4236f1510407/student+-+3.jpg" alt="Dashboard" loading="lazy"></div><div class="sh">← Swipe to see more →</div></div></div>

</div></section>

<!-- ========== EXPERIENCE ========== -->
<section id="experience" class="sec"><div class="wrap">
  <div class="se">Career Journey</div>
  <h2 class="st">18 years of <em>growth</em></h2>
  <div class="tl an">
    <div class="ti">
      <div class="td">2024 — Present</div>
      <h3>Global VP of Product</h3>
      <h4>Mars Veterinary Health — Hybrid: CA, NY, FL, Europe/Asia</h4>
      <p>Leading strategy and delivery of a global digital product platform across 2,500+ hospitals and 70,000+ associates in North America, Europe, and Asia. Managing a $110M annual portfolio with a 62-person global team across product, design, engineering, and operations. Driving AI integration across clinical and commercial workflows, cutting administrative workload by 30%. Rebuilt the global product organization, introduced agile delivery, and established cross-regional governance.</p>
    </div>
    <div class="ti">
      <div class="td">2021 — 2024</div>
      <h3>Vice President, Digital Product</h3>
      <h4>VCA Inc — Santa Monica, CA</h4>
      <p>Directed digital transformation for 1,200+ hospitals, improving the care experience for 5 million clients. Built product and engineering departments from the ground up with clear KPIs. Managed $10M+ budgets, grew the product team to meet increasing scale and complexity, and delivered product strategy keynotes to executive leadership.</p>
    </div>
    <div class="ti">
      <div class="td">2021 — 2022</div>
      <h3>Senior Director, Digital Innovation</h3>
      <h4>VCA Inc — Hybrid: CA/CO</h4>
      <p>Created and launched the automated queue system for urgent care, reducing wait stress and improving flow — resulting in a 20% revenue lift. Relaunched digital platforms with an average 50% adoption rate across a non-standardized operational environment.</p>
    </div>
    <div class="ti">
      <div class="td">2019 — 2021</div>
      <h3>Director, Digital Innovation</h3>
      <h4>VCA Animal Hospitals — Hybrid: CA/CO</h4>
      <p>Scaled the client-facing digital experience across 1,000+ hospitals in the US and Canada. Launched the myVCA app and Text to Pay features, powering $1B+ in digital payment collection. Led the digital pandemic response — rolling out video telehealth and live chat across the entire network.</p>
    </div>
    <div class="ti">
      <div class="td">2018 — 2019</div>
      <h3>Senior Product Manager</h3>
      <h4>VCA Animal Hospitals — Denver, CO</h4>
      <p>Directed Scrum teams delivering mobile and web apps used across 800+ hospitals. Defined the roadmap and rollout for flagship tools: myVCA, Retriever+, and Messenger. Developed training programs for 20,000+ employees to support tool adoption across the network.</p>
    </div>
    <div class="ti">
      <div class="td">2009 — 2018</div>
      <h3>Product & Training Leader</h3>
      <h4>VCA Animal Hospitals — Traveling North America & Canada</h4>
      <p>Progressed from Program Leader to Product Manager over 9 years, leading digital transformation, training, and adoption initiatives across a 500-hospital network. Recruited by the COO/Co-Founder to design a management training program that reversed a 30% revenue decline to 3% growth within one year at a pilot hospital. Trained teams across 18 states, onboarding 75+ locations. Pitched and led digital transformation partnerships with startups and vendors, accelerating release cycles from annual to 3-week sprints. Grew product adoption from 3% to 50%+ across the network.</p>
    </div>
  </div>

  <!-- Education -->
  <div class="an" style="margin-top:48px">
    <div class="se">Education</div>
    <h2 class="st" style="margin-bottom:24px">Where I <em>studied</em></h2>
    <div class="edu-grid">
      <div class="edu-card">
        <div class="edu-deg">Master of Arts — Global Finance & Trade</div>
        <div class="edu-school">University of Denver, Korbel School of International Studies</div>
        <div class="edu-detail">Economic Integration · International Business · Homeland Security</div>
      </div>
      <div class="edu-card">
        <div class="edu-deg">Bachelor of Science — Business Information Technology</div>
        <div class="edu-school">University of Denver, Daniels College of Business</div>
        <div class="edu-detail">International Business</div>
      </div>
    </div>
    <div class="extras">
      <span class="ext-tag">Fluent in English & Arabic</span>
      <span class="ext-tag">Basic French</span>
      <span class="ext-tag">Mars Global Innovation Award</span>
      <span class="ext-tag">$110M Portfolio</span>
      <span class="ext-tag">62-Person Global Team</span>
    </div>
  </div>

</div></section>

<!-- ========== TESTIMONIALS ========== -->
<section id="refs" class="sec"><div class="wrap">
  <div class="se">References</div>
  <h2 class="st">What colleagues <em>say</em></h2>
  <div class="tg">
    <div class="tc an"><blockquote>"Abe has the ability to cut through the noise, make the right trade-offs, and deliver maximum value. He led the product development and launch of 4 mobile apps at a rate that would impress even the most aggressive start-up teams."</blockquote><div class="tw"><div class="tav">BL</div><div><div class="tn">Brendan Lynch</div><div class="tr">SVP, Product & Innovation</div></div></div></div>
    <div class="tc an d1"><blockquote>"I am proud of the profound impact Abe has had on VCA and me. He has such a passion and dedication towards anything he does. Anyone would be lucky to have him as part of their organization."</blockquote><div class="tw"><div class="tav">BA</div><div><div class="tn">Bob Antin</div><div class="tr">CEO & Founder, VCA</div></div></div></div>
    <div class="tc an d2"><blockquote>"An exceptional IT product leader who truly stands out for his innovative thinking, strategic vision, and unwavering passion. Abe approaches every challenge with a big-picture mindset, ensuring solutions position the business for future success."</blockquote><div class="tw"><div class="tav">AF</div><div><div class="tn">Aaron Frazier</div><div class="tr">COO, North America</div></div></div></div>
    <div class="tc an d3"><blockquote>"Abe has brought a collaborative, client-centric approach to each engagement. His down-to-earth, approachable demeanor makes him relatable to stakeholders at a variety of levels, and a fun person to have on a team."</blockquote><div class="tw"><div class="tav">MS</div><div><div class="tn">Martha Smith</div><div class="tr">Chief Client Officer</div></div></div></div>
  </div>
</div></section>

<!-- ========== CTA ========== -->
<section class="sec cta"><div class="wrap"><div class="an">
  <div class="se" style="justify-content:center">Contact</div>
  <h2 class="st" style="text-align:center">Let's talk about your next <em>product challenge</em></h2>
  <p class="cta-sub">Open to new opportunities in global product leadership. Happy to connect.</p>
  <div class="cta-b">
    <a href="mailto:abealmurjan@gmail.com" class="btn-g">✉ abealmurjan@gmail.com</a>
    <a href="https://www.linkedin.com/in/abealmurjan/" target="_blank" class="btn-o">LinkedIn Profile</a>
  </div>
</div></div></section>

<footer class="ft"><div class="wrap"><p>© 2026 Ibrahim Al-Murjan</p></div></footer>

<script>
const b=document.getElementById('nb'),o=document.getElementById('no');
b.addEventListener('click',()=>{b.classList.toggle('on');o.classList.toggle('on');document.body.style.overflow=o.classList.contains('on')?'hidden':'';});
o.querySelectorAll('a').forEach(a=>a.addEventListener('click',()=>{b.classList.remove('on');o.classList.remove('on');document.body.style.overflow='';}));
const io=new IntersectionObserver(e=>{e.forEach(x=>{if(x.isIntersecting)x.target.classList.add('vi')})},{threshold:0.08});
document.querySelectorAll('.an').forEach(el=>io.observe(el));
</script>
</body>
</html>
