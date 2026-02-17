[index.html.html](https://github.com/user-attachments/files/25370598/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ibrahim Al-Murjan — Digital Product Leader</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;1,9..40,300;1,9..40,400&display=swap" rel="stylesheet">
<style>
:root {
  --bg: #0C0C0E;
  --bg-elevated: #141418;
  --bg-card: #1A1A20;
  --text-primary: #F0EDE6;
  --text-secondary: #9A958B;
  --text-muted: #5E5A52;
  --accent: #D4A853;
  --accent-dim: rgba(212,168,83,0.12);
  --accent-glow: rgba(212,168,83,0.25);
  --border: rgba(240,237,230,0.06);
  --serif: 'Instrument Serif', Georgia, serif;
  --sans: 'DM Sans', sans-serif;
}
*, *::before, *::after { margin:0; padding:0; box-sizing:border-box; }
html { scroll-behavior: smooth; font-size: 16px; }
body {
  font-family: var(--sans);
  background: var(--bg);
  color: var(--text-primary);
  line-height: 1.6;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
}
::selection { background: var(--accent); color: var(--bg); }

/* Noise texture overlay */
body::before {
  content: '';
  position: fixed;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
  pointer-events: none;
  z-index: 9999;
}

/* Utility */
.container { max-width: 1200px; margin: 0 auto; padding: 0 clamp(24px, 5vw, 64px); }
section { padding: clamp(60px, 10vh, 120px) 0; }

/* Navigation */
nav {
  position: fixed; top: 0; left: 0; right: 0;
  z-index: 100;
  padding: 20px 0;
  backdrop-filter: blur(20px);
  background: rgba(12,12,14,0.7);
  border-bottom: 1px solid var(--border);
  transition: all 0.4s ease;
}
nav .container {
  display: flex; justify-content: space-between; align-items: center;
}
.nav-name {
  font-family: var(--serif);
  font-size: 1.25rem;
  color: var(--text-primary);
  text-decoration: none;
  letter-spacing: -0.02em;
}
.nav-name span { color: var(--accent); }
.nav-links { display: flex; gap: 32px; align-items: center; }
.nav-links a {
  color: var(--text-secondary);
  text-decoration: none;
  font-size: 0.85rem;
  font-weight: 400;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  transition: color 0.3s;
}
.nav-links a:hover { color: var(--accent); }
.nav-cta {
  background: var(--accent) !important;
  color: var(--bg) !important;
  padding: 10px 24px;
  border-radius: 100px;
  font-weight: 500 !important;
  letter-spacing: 0.02em !important;
  text-transform: none !important;
  font-size: 0.9rem !important;
  transition: transform 0.3s, box-shadow 0.3s !important;
}
.nav-cta:hover {
  transform: translateY(-1px);
  box-shadow: 0 4px 20px var(--accent-glow);
  color: var(--bg) !important;
}

/* Mobile nav toggle */
.nav-toggle {
  display: none;
  background: none; border: none; cursor: pointer;
  width: 28px; height: 20px; position: relative; z-index: 101;
}
.nav-toggle span {
  display: block; width: 100%; height: 2px; background: var(--text-primary);
  transition: all 0.3s; position: absolute; left: 0;
}
.nav-toggle span:nth-child(1) { top: 0; }
.nav-toggle span:nth-child(2) { top: 9px; }
.nav-toggle span:nth-child(3) { top: 18px; }

/* Hero */
.hero {
  min-height: 100vh;
  display: flex; align-items: center;
  position: relative;
  padding-top: 100px;
}
.hero::before {
  content: '';
  position: absolute;
  top: -20%; right: -10%;
  width: 600px; height: 600px;
  background: radial-gradient(circle, var(--accent-dim) 0%, transparent 70%);
  filter: blur(80px);
  pointer-events: none;
}
.hero-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
  align-items: center;
}
.hero-label {
  display: inline-flex; align-items: center; gap: 10px;
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--accent);
  margin-bottom: 24px;
  font-weight: 500;
}
.hero-label::before {
  content: '';
  width: 24px; height: 1px;
  background: var(--accent);
}
.hero h1 {
  font-family: var(--serif);
  font-size: clamp(2.8rem, 5.5vw, 4.5rem);
  line-height: 1.05;
  letter-spacing: -0.03em;
  color: var(--text-primary);
  margin-bottom: 28px;
}
.hero h1 em {
  font-style: italic;
  color: var(--accent);
}
.hero-desc {
  font-size: 1.1rem;
  color: var(--text-secondary);
  line-height: 1.7;
  max-width: 520px;
  margin-bottom: 40px;
}
.hero-actions { display: flex; gap: 16px; flex-wrap: wrap; }
.btn-primary {
  display: inline-flex; align-items: center; gap: 8px;
  background: var(--accent);
  color: var(--bg);
  padding: 14px 32px;
  border-radius: 100px;
  text-decoration: none;
  font-weight: 500;
  font-size: 0.95rem;
  transition: all 0.3s;
  border: none; cursor: pointer;
}
.btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 30px var(--accent-glow); }
.btn-secondary {
  display: inline-flex; align-items: center; gap: 8px;
  background: transparent;
  color: var(--text-primary);
  padding: 14px 32px;
  border-radius: 100px;
  text-decoration: none;
  font-weight: 400;
  font-size: 0.95rem;
  border: 1px solid rgba(240,237,230,0.15);
  transition: all 0.3s;
}
.btn-secondary:hover { border-color: var(--accent); color: var(--accent); }

/* Hero visual */
.hero-visual {
  position: relative;
  display: flex; justify-content: center;
}
.hero-image-frame {
  position: relative;
  width: 380px; height: 460px;
  border-radius: 20px;
  overflow: hidden;
  border: 1px solid var(--border);
}
.hero-image-frame img {
  width: 100%; height: 100%;
  object-fit: cover;
}
.hero-image-frame::after {
  content: '';
  position: absolute; inset: 0;
  background: linear-gradient(180deg, transparent 50%, rgba(12,12,14,0.6) 100%);
}
.hero-badge {
  position: absolute;
  bottom: -20px; left: -30px;
  background: var(--bg-card);
  border: 1px solid var(--border);
  border-radius: 16px;
  padding: 16px 24px;
  backdrop-filter: blur(10px);
  z-index: 2;
}
.hero-badge-label {
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--text-muted);
  margin-bottom: 4px;
}
.hero-badge-value {
  font-family: var(--serif);
  font-size: 1.4rem;
  color: var(--accent);
}
.hero-badge-2 {
  position: absolute;
  top: -16px; right: -20px;
  background: var(--accent);
  color: var(--bg);
  border-radius: 12px;
  padding: 14px 20px;
  z-index: 2;
  text-align: center;
}
.hero-badge-2 .num {
  font-family: var(--serif);
  font-size: 1.6rem;
  display: block;
  line-height: 1;
}
.hero-badge-2 .lbl {
  font-size: 0.65rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  opacity: 0.8;
}

/* Stats bar */
.stats-bar {
  border-top: 1px solid var(--border);
  border-bottom: 1px solid var(--border);
  padding: 48px 0;
}
.stats-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 40px;
  text-align: center;
}
.stat-item { position: relative; }
.stat-item:not(:last-child)::after {
  content: '';
  position: absolute;
  right: -20px; top: 10%; height: 80%;
  width: 1px;
  background: var(--border);
}
.stat-number {
  font-family: var(--serif);
  font-size: clamp(2rem, 4vw, 3rem);
  color: var(--accent);
  display: block;
  line-height: 1;
  margin-bottom: 8px;
}
.stat-label {
  font-size: 0.85rem;
  color: var(--text-secondary);
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

/* Section headers */
.section-header {
  margin-bottom: 64px;
}
.section-eyebrow {
  display: inline-flex; align-items: center; gap: 10px;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--accent);
  margin-bottom: 16px;
  font-weight: 500;
}
.section-eyebrow::before {
  content: '';
  width: 24px; height: 1px;
  background: var(--accent);
}
.section-title {
  font-family: var(--serif);
  font-size: clamp(2rem, 4vw, 3.2rem);
  letter-spacing: -0.02em;
  line-height: 1.1;
  max-width: 600px;
}
.section-title em { font-style: italic; color: var(--accent); }

/* About / Story */
.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
  align-items: start;
}
.about-text p {
  font-size: 1.05rem;
  color: var(--text-secondary);
  line-height: 1.8;
  margin-bottom: 20px;
}
.about-text p:first-of-type::first-letter {
  font-family: var(--serif);
  font-size: 3.5rem;
  float: left;
  color: var(--accent);
  line-height: 1;
  margin-right: 12px;
  margin-top: 4px;
}
.principles-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
  margin-top: 40px;
}
.principle {
  background: var(--bg-elevated);
  border: 1px solid var(--border);
  border-radius: 14px;
  padding: 24px;
  transition: all 0.4s;
}
.principle:hover { border-color: var(--accent-dim); transform: translateY(-2px); }
.principle-icon {
  width: 36px; height: 36px;
  background: var(--accent-dim);
  border-radius: 10px;
  display: flex; align-items: center; justify-content: center;
  margin-bottom: 14px;
  color: var(--accent);
  font-size: 1rem;
}
.principle h4 {
  font-family: var(--serif);
  font-size: 1.05rem;
  margin-bottom: 6px;
  color: var(--text-primary);
}
.principle p {
  font-size: 0.82rem;
  color: var(--text-muted);
  line-height: 1.5;
}

/* Portfolio */
.portfolio { background: var(--bg-elevated); }
.portfolio-grid {
  display: grid;
  gap: 32px;
}
.portfolio-card {
  display: grid;
  grid-template-columns: 1fr 1fr;
  background: var(--bg-card);
  border: 1px solid var(--border);
  border-radius: 20px;
  overflow: hidden;
  transition: all 0.5s;
}
.portfolio-card:hover {
  border-color: rgba(212,168,83,0.15);
  transform: translateY(-4px);
  box-shadow: 0 20px 60px rgba(0,0,0,0.3);
}
.portfolio-card:nth-child(even) { direction: rtl; }
.portfolio-card:nth-child(even) > * { direction: ltr; }
.portfolio-content { padding: 48px; display: flex; flex-direction: column; justify-content: center; }
.portfolio-tag {
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--accent);
  margin-bottom: 12px;
  font-weight: 500;
}
.portfolio-card h3 {
  font-family: var(--serif);
  font-size: 1.8rem;
  letter-spacing: -0.02em;
  margin-bottom: 16px;
  line-height: 1.15;
}
.portfolio-card p {
  color: var(--text-secondary);
  font-size: 0.92rem;
  line-height: 1.7;
  margin-bottom: 24px;
}
.portfolio-metrics {
  display: flex; gap: 28px;
  padding-top: 20px;
  border-top: 1px solid var(--border);
}
.metric .metric-val {
  font-family: var(--serif);
  font-size: 1.5rem;
  color: var(--accent);
  display: block;
  line-height: 1.1;
}
.metric .metric-lbl {
  font-size: 0.72rem;
  color: var(--text-muted);
  text-transform: uppercase;
  letter-spacing: 0.06em;
}
.portfolio-visual {
  background: var(--bg);
  display: flex; align-items: center; justify-content: center;
  padding: 40px;
  position: relative;
  min-height: 360px;
  overflow: hidden;
}
.portfolio-visual::before {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(circle at 50% 50%, var(--accent-dim), transparent 70%);
  opacity: 0.5;
}
.app-mockup {
  position: relative; z-index: 1;
  width: 180px;
  background: var(--bg-card);
  border-radius: 24px;
  border: 1px solid rgba(255,255,255,0.08);
  padding: 8px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.4);
}
.app-mockup-inner {
  background: linear-gradient(135deg, var(--bg-elevated), var(--bg));
  border-radius: 18px;
  height: 320px;
  display: flex; flex-direction: column; align-items: center; justify-content: center;
  gap: 12px;
  color: var(--text-muted);
  font-size: 0.75rem;
  text-align: center;
  padding: 20px;
}
.app-mockup-icon {
  width: 48px; height: 48px;
  border-radius: 12px;
  background: var(--accent-dim);
  display: flex; align-items: center; justify-content: center;
  color: var(--accent);
  font-size: 1.2rem;
  margin-bottom: 4px;
}

/* Timeline / Experience */
.timeline-list { position: relative; padding-left: 32px; }
.timeline-list::before {
  content: '';
  position: absolute;
  left: 0; top: 0; bottom: 0;
  width: 1px;
  background: linear-gradient(180deg, var(--accent), var(--border), transparent);
}
.timeline-item {
  position: relative;
  padding-bottom: 48px;
}
.timeline-item::before {
  content: '';
  position: absolute;
  left: -36px; top: 8px;
  width: 10px; height: 10px;
  border-radius: 50%;
  background: var(--accent);
  box-shadow: 0 0 0 4px var(--bg), 0 0 0 5px var(--accent);
}
.timeline-date {
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--accent);
  margin-bottom: 8px;
  font-weight: 500;
}
.timeline-item h3 {
  font-family: var(--serif);
  font-size: 1.4rem;
  margin-bottom: 4px;
}
.timeline-item h4 {
  font-size: 0.9rem;
  color: var(--text-secondary);
  font-weight: 400;
  margin-bottom: 12px;
}
.timeline-item p {
  font-size: 0.88rem;
  color: var(--text-muted);
  line-height: 1.7;
  max-width: 560px;
}

/* Testimonials */
.testimonials-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 28px;
}
.testimonial-card {
  background: var(--bg-elevated);
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 40px;
  position: relative;
  transition: all 0.4s;
}
.testimonial-card:hover { border-color: rgba(212,168,83,0.12); }
.testimonial-card::before {
  content: '\201C';
  font-family: var(--serif);
  font-size: 5rem;
  color: var(--accent-dim);
  position: absolute;
  top: 16px; left: 32px;
  line-height: 1;
}
.testimonial-text {
  font-size: 0.95rem;
  color: var(--text-secondary);
  line-height: 1.75;
  margin-bottom: 28px;
  position: relative;
  z-index: 1;
  font-style: italic;
}
.testimonial-author { display: flex; align-items: center; gap: 12px; }
.testimonial-avatar {
  width: 44px; height: 44px;
  border-radius: 50%;
  background: var(--accent-dim);
  display: flex; align-items: center; justify-content: center;
  color: var(--accent);
  font-family: var(--serif);
  font-size: 1.1rem;
}
.testimonial-name {
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--text-primary);
}
.testimonial-role {
  font-size: 0.78rem;
  color: var(--text-muted);
}

/* CTA Section */
.cta-section {
  text-align: center;
  position: relative;
}
.cta-section::before {
  content: '';
  position: absolute;
  top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  width: 600px; height: 400px;
  background: radial-gradient(circle, var(--accent-dim), transparent 70%);
  filter: blur(60px);
  pointer-events: none;
}
.cta-section .section-title {
  max-width: 700px;
  margin: 0 auto 20px;
}
.cta-desc {
  color: var(--text-secondary);
  max-width: 500px;
  margin: 0 auto 40px;
  font-size: 1.05rem;
}
.cta-links {
  display: flex; gap: 16px; justify-content: center; flex-wrap: wrap;
  position: relative; z-index: 1;
}

/* Footer */
footer {
  border-top: 1px solid var(--border);
  padding: 40px 0;
  text-align: center;
}
footer p {
  color: var(--text-muted);
  font-size: 0.8rem;
}
footer a { color: var(--accent); text-decoration: none; }

/* Animations */
.fade-up {
  opacity: 0;
  transform: translateY(30px);
  transition: opacity 0.7s ease, transform 0.7s ease;
}
.fade-up.visible {
  opacity: 1;
  transform: translateY(0);
}
.stagger-1 { transition-delay: 0.1s; }
.stagger-2 { transition-delay: 0.2s; }
.stagger-3 { transition-delay: 0.3s; }
.stagger-4 { transition-delay: 0.4s; }

/* Responsive */
@media (max-width: 1024px) {
  .hero-grid { grid-template-columns: 1fr; gap: 48px; text-align: center; }
  .hero-desc { margin-left: auto; margin-right: auto; }
  .hero-actions { justify-content: center; }
  .hero-visual { order: -1; }
  .hero-image-frame { width: 300px; height: 380px; }
  .about-grid { grid-template-columns: 1fr; gap: 48px; }
  .portfolio-card { grid-template-columns: 1fr; }
  .portfolio-card:nth-child(even) { direction: ltr; }
  .portfolio-visual { min-height: 280px; }
  .testimonials-grid { grid-template-columns: 1fr; }
  .stats-grid { grid-template-columns: repeat(2, 1fr); gap: 32px; }
  .stat-item:nth-child(2)::after { display: none; }
}
@media (max-width: 768px) {
  .nav-links { 
    display: none; 
    position: fixed; inset: 0;
    background: rgba(12,12,14,0.97);
    flex-direction: column;
    justify-content: center; align-items: center;
    gap: 32px;
    backdrop-filter: blur(20px);
  }
  .nav-links.open { display: flex; }
  .nav-links a { font-size: 1.2rem; }
  .nav-toggle { display: block; }
  .hero-label { justify-content: center; }
  .hero-badge, .hero-badge-2 { display: none; }
  .principles-grid { grid-template-columns: 1fr; }
  .stats-grid { grid-template-columns: 1fr; }
  .stat-item::after { display: none !important; }
}
</style>
</head>
<body>

<!-- Navigation -->
<nav>
  <div class="container">
    <a href="#" class="nav-name">abe<span>.</span></a>
    <div class="nav-links" id="navLinks">
      <a href="#about">About</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#experience">Experience</a>
      <a href="#testimonials">Voices</a>
      <a href="mailto:abealmurjan@gmail.com" class="nav-cta">Let's Connect</a>
    </div>
    <button class="nav-toggle" id="navToggle" aria-label="Toggle menu">
      <span></span><span></span><span></span>
    </button>
  </div>
</nav>

<!-- Hero -->
<section class="hero">
  <div class="container">
    <div class="hero-grid">
      <div>
        <div class="hero-label">Digital Product Leader</div>
        <h1>18 years shipping<br>products that <em>scale</em></h1>
        <p class="hero-desc">
          I'm Ibrahim Al-Murjan. I build and scale digital platforms across complex, multi-site ecosystems — consumer apps, AI tools, enterprise workflow systems. Products from zero to millions of users, teams from the ground up.
        </p>
        <div class="hero-actions">
          <a href="mailto:abealmurjan@gmail.com" class="btn-primary">
            <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
            Get in Touch
          </a>
          <a href="#portfolio" class="btn-secondary">
            <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M6 9l6 6 6-6"/></svg>
            See the Work
          </a>
        </div>
      </div>
      <div class="hero-visual">
        <div class="hero-image-frame">
          <img src="https://images.squarespace-cdn.com/content/v1/6272e701b833b942c882586c/7bc9c342-47bf-48e0-bd09-e07d94b646dc/5+-+Abe.jpeg" alt="Ibrahim Al-Murjan presenting at VCA National Meeting 2024">
        </div>
        <div class="hero-badge">
          <div class="hero-badge-label">Award</div>
          <div class="hero-badge-value">Mars Global<br>Innovation Winner</div>
        </div>
        <div class="hero-badge-2">
          <span class="num">18+</span>
          <span class="lbl">Years in Product</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Stats Bar -->
<div class="stats-bar">
  <div class="container">
    <div class="stats-grid">
      <div class="stat-item fade-up">
        <span class="stat-number">1M+</span>
        <span class="stat-label">App Users</span>
      </div>
      <div class="stat-item fade-up stagger-1">
        <span class="stat-number">75M+</span>
        <span class="stat-label">Messages Exchanged</span>
      </div>
      <div class="stat-item fade-up stagger-2">
        <span class="stat-number">500K+</span>
        <span class="stat-label">AI Dictations</span>
      </div>
      <div class="stat-item fade-up stagger-3">
        <span class="stat-number">4.8★</span>
        <span class="stat-label">User Satisfaction</span>
      </div>
    </div>
  </div>
</div>

<!-- About -->
<section id="about">
  <div class="container">
    <div class="about-grid">
      <div class="about-text fade-up">
        <div class="section-header">
          <div class="section-eyebrow">Background</div>
          <h2 class="section-title">How I <em>work</em></h2>
        </div>
        <p>I started on the ground floor — training hospital teams on software, learning every operational pain point firsthand. That shaped how I approach product: start with the real problem, build for the people using it, measure what matters.</p>
        <p>Since then I've led product teams responsible for consumer apps, AI clinical tools, telehealth platforms, and enterprise workflow systems across a network of 1,000+ locations. I've shipped products in as little as 6 weeks and scaled them to millions of users.</p>
      </div>
      <div class="fade-up stagger-2">
        <div class="principles-grid">
          <div class="principle">
            <div class="principle-icon">⚡</div>
            <h4>0 → 1 Launches</h4>
            <p>Taken multiple products from concept to production — including one shipped in 6 weeks.</p>
          </div>
          <div class="principle">
            <div class="principle-icon">📐</div>
            <h4>Team Building</h4>
            <p>Built and scaled cross-functional product teams across engineering, design, and operations.</p>
          </div>
          <div class="principle">
            <div class="principle-icon">↗</div>
            <h4>Scale</h4>
            <p>Products deployed across 1,000+ locations serving millions of end users.</p>
          </div>
          <div class="principle">
            <div class="principle-icon">◉</div>
            <h4>AI & Innovation</h4>
            <p>Shipped production AI tools — dictation, triage, clinical automation — in a regulated healthcare environment.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Portfolio -->
<section id="portfolio" class="portfolio">
  <div class="container">
    <div class="section-header fade-up">
      <div class="section-eyebrow">Product Portfolio</div>
      <h2 class="section-title">What I've <em>shipped</em></h2>
    </div>
    <div class="portfolio-grid">

      <!-- myVCA App -->
      <div class="portfolio-card fade-up">
        <div class="portfolio-content">
          <div class="portfolio-tag">Consumer Mobile App</div>
          <h3>Consumer Healthcare App</h3>
          <p>Consumer mobile app for a 1,000+ location veterinary network. Handles check-in, document signing, digital checkout, and 24/7 care access. Grew to over 1M active users with a 4.8-star rating.</p>
          <div class="portfolio-metrics">
            <div class="metric"><span class="metric-val">1M+</span><span class="metric-lbl">Active Users</span></div>
            <div class="metric"><span class="metric-val">4.8</span><span class="metric-lbl">App Store Rating</span></div>
          </div>
        </div>
        <div class="portfolio-visual">
          <div class="app-mockup">
            <div class="app-mockup-inner">
              <div class="app-mockup-icon">🐾</div>
              <strong style="color:var(--text-primary)">myVCA</strong>
              <span>Consumer<br>Healthcare App</span>
            </div>
          </div>
        </div>
      </div>

      <!-- Scribe AI -->
      <div class="portfolio-card fade-up">
        <div class="portfolio-content">
          <div class="portfolio-tag">AI-Powered Healthcare</div>
          <h3>AI Medical Dictation</h3>
          <p>AI-powered dictation tool that cut manual medical record writing by 90%. Doctors dictate, the system transcribes and pushes structured notes into the practice management system. Concept to production in 6 weeks.</p>
          <div class="portfolio-metrics">
            <div class="metric"><span class="metric-val">500K+</span><span class="metric-lbl">Dictations in Year 1</span></div>
            <div class="metric"><span class="metric-val">95%</span><span class="metric-lbl">Accuracy Rate</span></div>
            <div class="metric"><span class="metric-val">6 wks</span><span class="metric-lbl">Built & Launched</span></div>
          </div>
        </div>
        <div class="portfolio-visual">
          <div class="app-mockup">
            <div class="app-mockup-inner">
              <div class="app-mockup-icon">🎙️</div>
              <strong style="color:var(--text-primary)">Scribe AI</strong>
              <span>Dictate. Transcribe.<br>Done.</span>
            </div>
          </div>
        </div>
      </div>

      <!-- Telehealth -->
      <div class="portfolio-card fade-up">
        <div class="portfolio-content">
          <div class="portfolio-tag">Virtual Care Platform</div>
          <h3>Telehealth & Live Chat</h3>
          <p>In-app teletriage chat launched in 2018, expanded to full video and 24/7 access in 2020. Omnichannel — web and mobile, integrated with medical records, real-time clinical data.</p>
          <div class="portfolio-metrics">
            <div class="metric"><span class="metric-val">24/7</span><span class="metric-lbl">Around-the-Clock</span></div>
            <div class="metric"><span class="metric-val">4.8★</span><span class="metric-lbl">Client Satisfaction</span></div>
          </div>
        </div>
        <div class="portfolio-visual">
          <div class="app-mockup">
            <div class="app-mockup-inner">
              <div class="app-mockup-icon">💬</div>
              <strong style="color:var(--text-primary)">Telehealth</strong>
              <span>24/7 Virtual<br>Pet Care</span>
            </div>
          </div>
        </div>
      </div>

      <!-- Retriever+ -->
      <div class="portfolio-card fade-up">
        <div class="portfolio-content">
          <div class="portfolio-tag">Enterprise Staff Platform</div>
          <h3>Staff Enablement & Direct Messaging</h3>
          <p>Mobile staff platform paired with a 2-way SMS system for client communication. Texting product launched in 2014. Digitized front-desk workflows, eliminated paper processes, and created a direct engagement channel across the full network.</p>
          <div class="portfolio-metrics">
            <div class="metric"><span class="metric-val">5M+</span><span class="metric-lbl">Client Engagements</span></div>
            <div class="metric"><span class="metric-val">75M+</span><span class="metric-lbl">Texts Exchanged</span></div>
            <div class="metric"><span class="metric-val">10M+</span><span class="metric-lbl">Sheets Saved</span></div>
          </div>
        </div>
        <div class="portfolio-visual">
          <div class="app-mockup">
            <div class="app-mockup-inner">
              <div class="app-mockup-icon">📱</div>
              <strong style="color:var(--text-primary)">Retriever+</strong>
              <span>Staff Tools<br>& Direct SMS</span>
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- Experience -->
<section id="experience">
  <div class="container">
    <div class="section-header fade-up">
      <div class="section-eyebrow">Career Journey</div>
      <h2 class="section-title">Where I've <em>been</em></h2>
    </div>
    <div class="timeline-list fade-up">
      <div class="timeline-item">
        <div class="timeline-date">Current</div>
        <h3>Senior Director, Digital Products & Innovation</h3>
        <h4>VCA Animal Hospitals (Mars Petcare)</h4>
        <p>Own product vision and delivery for consumer and enterprise digital products across 1,000+ veterinary hospitals. Portfolio includes AI medical documentation, telehealth, a consumer app (1M+ users), staff workflow tools, and direct client messaging. Mars "Make the Difference" Global Innovation Award winner.</p>
      </div>
      <div class="timeline-item">
        <div class="timeline-date">Previously</div>
        <h3>Product Manager → Senior Product Manager</h3>
        <h4>VCA Animal Hospitals</h4>
        <p>Grew from mobile PM to owning the digital product portfolio. Launched the first 2-way SMS platform for veterinary client engagement (2014), built the consumer app, and developed the virtual waiting room product that deployed network-wide.</p>
      </div>
      <div class="timeline-item">
        <div class="timeline-date">Earlier Career</div>
        <h3>Software Training & Implementation</h3>
        <h4>VCA Animal Hospitals</h4>
        <p>Trained hospital teams on practice management software across the network. Learned the operational workflow and pain points firsthand — context that informed every product decision since.</p>
      </div>
    </div>
  </div>
</section>

<!-- Testimonials -->
<section id="testimonials">
  <div class="container">
    <div class="section-header fade-up">
      <div class="section-eyebrow">References</div>
      <h2 class="section-title">What colleagues <em>say</em></h2>
    </div>
    <div class="testimonials-grid">
      <div class="testimonial-card fade-up">
        <p class="testimonial-text">"Abe has the ability to cut through the noise, make the right trade-offs, and deliver maximum value. He led the product development and launch of 4 mobile apps at a rate that would impress even the most aggressive start-up teams."</p>
        <div class="testimonial-author">
          <div class="testimonial-avatar">BL</div>
          <div>
            <div class="testimonial-name">Brendan Lynch</div>
            <div class="testimonial-role">SVP, Product & Innovation</div>
          </div>
        </div>
      </div>
      <div class="testimonial-card fade-up stagger-1">
        <p class="testimonial-text">"I am proud of the profound impact Abe has had on VCA and me. He has such a passion and dedication towards anything he does. Anyone would be lucky to have him as part of their organization."</p>
        <div class="testimonial-author">
          <div class="testimonial-avatar">BA</div>
          <div>
            <div class="testimonial-name">Bob Antin</div>
            <div class="testimonial-role">CEO & Founder, VCA</div>
          </div>
        </div>
      </div>
      <div class="testimonial-card fade-up stagger-2">
        <p class="testimonial-text">"An exceptional IT product leader who truly stands out for his innovative thinking, strategic vision, and unwavering passion. Abe approaches every challenge with a big-picture mindset, ensuring solutions position the business for future success."</p>
        <div class="testimonial-author">
          <div class="testimonial-avatar">AF</div>
          <div>
            <div class="testimonial-name">Aaron Frazier</div>
            <div class="testimonial-role">COO, North America</div>
          </div>
        </div>
      </div>
      <div class="testimonial-card fade-up stagger-3">
        <p class="testimonial-text">"Abe has brought a collaborative, client-centric approach to each engagement. His down-to-earth, approachable demeanor makes him relatable to stakeholders at a variety of levels, and a fun person to have on a team."</p>
        <div class="testimonial-author">
          <div class="testimonial-avatar">MS</div>
          <div>
            <div class="testimonial-name">Martha Smith</div>
            <div class="testimonial-role">Chief Client Officer</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- CTA -->
<section class="cta-section">
  <div class="container">
    <div class="fade-up">
      <div class="section-eyebrow" style="justify-content:center;">Contact</div>
      <h2 class="section-title" style="text-align:center;">Let's talk about<br>your next <em>product challenge</em></h2>
      <p class="cta-desc">Open to new opportunities in digital product leadership. Happy to connect.</p>
      <div class="cta-links">
        <a href="mailto:abealmurjan@gmail.com" class="btn-primary">
          <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
          abealmurjan@gmail.com
        </a>
        <a href="https://www.linkedin.com/in/abealmurjan/" target="_blank" class="btn-secondary">
          <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
          LinkedIn Profile
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Footer -->
<footer>
  <div class="container">
    <p>© 2026 Ibrahim Al-Murjan</p>
  </div>
</footer>

<script>
// Mobile nav
const toggle = document.getElementById('navToggle');
const links = document.getElementById('navLinks');
toggle.addEventListener('click', () => {
  links.classList.toggle('open');
});
links.querySelectorAll('a').forEach(a => {
  a.addEventListener('click', () => links.classList.remove('open'));
});

// Scroll animations
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('visible');
    }
  });
}, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });

document.querySelectorAll('.fade-up').forEach(el => observer.observe(el));
</script>

</body>
</html>
