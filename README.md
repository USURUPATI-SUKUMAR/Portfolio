# Portfolio
This is my portfolio
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sukumar Usurupati — AI &amp; Computer Engineering Student</title>
<meta name="description" content="Portfolio of Sukumar Usurupati — B.Tech Computer Science &amp; Engineering (AI) student, QIS College of Engineering and Technology.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #fafbfe;
    --surface: #ffffff;
    --surface-2: #f2f4fb;
    --ink: #12141c;
    --muted: #5b6272;
    --border: rgba(18,20,28,0.09);
    --accent: #4a56e2;
    --accent-2: #8b5cf6;
    --accent-soft: rgba(74,86,226,0.10);
    --shadow: 0 1px 2px rgba(18,20,28,0.04), 0 8px 24px rgba(18,20,28,0.06);
    --radius: 14px;
    color-scheme: light;
  }
  html.dark{
    --bg: #0a0d16;
    --surface: #10141f;
    --surface-2: #141826;
    --ink: #e9ebf5;
    --muted: #9aa1b5;
    --border: rgba(255,255,255,0.08);
    --accent: #7c8bff;
    --accent-2: #a78bfa;
    --accent-soft: rgba(124,139,255,0.14);
    --shadow: 0 1px 2px rgba(0,0,0,0.3), 0 12px 30px rgba(0,0,0,0.35);
    color-scheme: dark;
  }
  *{ box-sizing: border-box; }
  html{ scroll-behavior: smooth; }
  @media (prefers-reduced-motion: reduce){
    html{ scroll-behavior: auto; }
    *{ animation-duration: 0.001ms !important; animation-iteration-count: 1 !important; transition-duration: 0.001ms !important; }
  }
  body{
    margin:0;
    background: var(--bg);
    color: var(--ink);
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
    -webkit-font-smoothing: antialiased;
    transition: background 0.35s ease, color 0.35s ease;
  }
  h1,h2,h3,h4{
    font-family: 'Space Grotesk', 'Inter', sans-serif;
    margin: 0;
    letter-spacing: -0.02em;
  }
  a{ color: inherit; text-decoration: none; }
  .mono{ font-family: 'JetBrains Mono', monospace; }
  .wrap{ max-width: 1100px; margin: 0 auto; padding: 0 28px; }
  img{ max-width: 100%; display:block; }

  header.nav{
    position: sticky; top: 0; z-index: 100;
    backdrop-filter: saturate(180%) blur(14px);
    -webkit-backdrop-filter: saturate(180%) blur(14px);
    background: color-mix(in srgb, var(--bg) 78%, transparent);
    border-bottom: 1px solid var(--border);
  }
  .nav-inner{
    display:flex; align-items:center; justify-content:space-between;
    padding: 16px 28px; max-width: 1100px; margin: 0 auto;
  }
  .brand{ display:flex; align-items:center; gap:10px; font-weight:600; font-size:16px; }
  .brand .dot{
    width:9px; height:9px; border-radius: 50%;
    background: linear-gradient(135deg, var(--accent), var(--accent-2));
    box-shadow: 0 0 0 4px var(--accent-soft);
  }
  nav.links{ display:flex; gap: 24px; align-items:center; }
  nav.links a{
    font-size: 13.5px; color: var(--muted); font-weight: 500;
    position: relative; padding: 4px 0; white-space:nowrap;
    transition: color 0.2s ease;
  }
  nav.links a:hover{ color: var(--ink); }
  nav.links a::after{
    content:''; position:absolute; left:0; bottom:-2px; height:1px; width:0%;
    background: var(--accent); transition: width 0.25s ease;
  }
  nav.links a:hover::after{ width:100%; }
  .nav-right{ display:flex; align-items:center; gap: 14px; }
  .toggle-btn{
    width:38px; height:38px; border-radius: 50%; border:1px solid var(--border);
    background: var(--surface); display:flex; align-items:center; justify-content:center;
    cursor:pointer; color: var(--ink); transition: transform 0.2s ease, background 0.2s ease;
    flex-shrink:0;
  }
  .toggle-btn:hover{ transform: scale(1.06); }
  .toggle-btn svg{ width:17px; height:17px; }

  @media (max-width: 900px){
    nav.links{ display:none; }
  }

  .hero{
    position: relative; overflow: hidden;
    padding: 110px 0 0;
    border-bottom: 1px solid var(--border);
  }
  .hero canvas{
    position:absolute; inset:0; width:100%; height:100%; opacity: 0.5;
    pointer-events:none;
  }
  .hero-inner{ position: relative; z-index: 2; padding-bottom: 64px; }
  .eyebrow{
    display:inline-flex; align-items:center; gap:8px;
    font-family:'JetBrains Mono', monospace; font-size: 12.5px; color: var(--accent);
    background: var(--accent-soft); border: 1px solid var(--border);
    padding: 6px 12px; border-radius: 100px; margin-bottom: 26px;
    letter-spacing: 0.02em;
  }
  .eyebrow .pulse{
    width:6px; height:6px; border-radius:50%; background: var(--accent);
    animation: pulse 2s infinite;
  }
  @keyframes pulse{
    0%,100%{ opacity:1; transform:scale(1); }
    50%{ opacity:0.4; transform:scale(0.7); }
  }
  .hero h1{
    font-size: clamp(2.3rem, 5.6vw, 4.1rem);
    font-weight: 700; line-height: 1.06; max-width: 760px;
  }
  .hero h1 .grad{
    background: linear-gradient(120deg, var(--accent), var(--accent-2));
    -webkit-background-clip: text; background-clip: text; color: transparent;
  }
  .hero p.lead{
    margin-top: 22px; font-size: 17.5px; color: var(--muted); max-width: 580px; line-height: 1.65;
  }
  .hero-meta{
    margin-top: 18px; display:flex; gap: 18px; flex-wrap:wrap; color: var(--muted); font-size: 14px;
  }
  .hero-meta span{ display:flex; align-items:center; gap:7px; }
  .hero-meta svg{ width:15px; height:15px; opacity:0.8; }
  .cta-row{ margin-top: 36px; display:flex; gap:14px; flex-wrap:wrap; }
  .btn{
    padding: 13px 24px; border-radius: 10px; font-weight:600; font-size:14.5px;
    display:inline-flex; align-items:center; gap:8px; cursor:pointer; border:1px solid transparent;
    transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
  }
  .btn:hover{ transform: translateY(-2px); }
  .btn-primary{
    background: linear-gradient(120deg, var(--accent), var(--accent-2)); color:#fff;
    box-shadow: 0 8px 24px var(--accent-soft);
  }
  .btn-ghost{ background: var(--surface); border-color: var(--border); color: var(--ink); }

  .stats-bar{
    position: relative; z-index: 2;
    display:grid; grid-template-columns: repeat(3, 1fr);
    border-top: 1px solid var(--border);
  }
  .stat{
    padding: 26px 20px; text-align:center; border-left: 1px solid var(--border);
  }
  .stat:first-child{ border-left:none; }
  .stat .num{
    font-family:'Space Grotesk', sans-serif; font-weight:700; font-size: clamp(1.6rem, 3vw, 2.1rem);
    background: linear-gradient(120deg, var(--accent), var(--accent-2));
    -webkit-background-clip:text; background-clip:text; color:transparent;
  }
  .stat .label{ margin-top:4px; font-size:13px; color: var(--muted); }
  @media (max-width: 600px){ .stats-bar{ grid-template-columns: 1fr; } .stat{ border-left:none; border-top:1px solid var(--border); } .stat:first-child{ border-top:none; } }

  section{ padding: 92px 0; border-bottom: 1px solid var(--border); }
  section:last-of-type{ border-bottom: none; }
  .section-head{ margin-bottom: 46px; max-width: 640px; }
  .section-head .tag{
    font-family:'JetBrains Mono', monospace; font-size:12.5px; color: var(--accent);
    letter-spacing: 0.04em; text-transform: uppercase;
  }
  .section-head h2{ font-size: clamp(1.65rem, 3.2vw, 2.2rem); margin-top: 10px; }
  .section-head p{ margin-top: 14px; color: var(--muted); font-size: 15.5px; line-height:1.65; }

  .reveal{ opacity:0; transform: translateY(24px); transition: opacity 0.7s ease, transform 0.7s ease; }
  .reveal.in{ opacity:1; transform: translateY(0); }

  .about-grid{ display:grid; grid-template-columns: 120px 1fr; gap: 40px; align-items:start; }
  .avatar{
    width: 110px; height: 110px; border-radius: 24px;
    background: linear-gradient(135deg, var(--accent), var(--accent-2));
    display:flex; align-items:center; justify-content:center;
    font-family:'Space Grotesk', sans-serif; font-weight:700; font-size: 34px; color:#fff;
    box-shadow: var(--shadow); flex-shrink:0;
  }
  .about-text p{ color: var(--muted); font-size:16px; line-height:1.75; margin:0 0 14px; }
  .about-text p:last-child{ margin-bottom:0; }
  @media (max-width: 640px){ .about-grid{ grid-template-columns: 1fr; } .avatar{ width:80px; height:80px; font-size:24px; } }

  .skill-group{ margin-bottom: 28px; }
  .skill-group:last-child{ margin-bottom:0; }
  .skill-group h4{
    font-size:12.5px; text-transform:uppercase; letter-spacing:0.05em; color: var(--muted);
    font-family:'JetBrains Mono', monospace; font-weight:500; margin-bottom:14px;
  }
  .skills-wrap{ display:flex; flex-wrap:wrap; gap:10px; }
  .skill-chip{
    padding: 9px 15px; border-radius: 10px; background: var(--surface);
    border: 1px solid var(--border); font-size: 13.5px; font-weight:500;
    display:flex; align-items:center; gap:8px; box-shadow: var(--shadow);
    transition: transform 0.2s ease, border-color 0.2s ease;
  }
  .skill-chip:hover{ transform: translateY(-3px); border-color: var(--accent); }
  .skill-chip .bar{ width:6px; height:6px; border-radius:50%; background: var(--accent); flex-shrink:0; }

  .timeline{ position:relative; padding-left: 32px; }
  .timeline::before{
    content:''; position:absolute; left:5px; top:6px; bottom:6px; width:1px; background: var(--border);
  }
  .tl-item{ position:relative; padding-bottom: 40px; }
  .tl-item:last-child{ padding-bottom:0; }
  .tl-dot{
    position:absolute; left:-32px; top:4px; width:11px; height:11px; border-radius:50%;
    background: linear-gradient(135deg, var(--accent), var(--accent-2));
    box-shadow: 0 0 0 4px var(--accent-soft);
  }
  .tl-head{ display:flex; justify-content:space-between; align-items:baseline; flex-wrap:wrap; gap:8px; margin-bottom:6px; }
  .tl-role{ font-size:17px; font-weight:600; font-family:'Space Grotesk', sans-serif; }
  .tl-date{ font-family:'JetBrains Mono', monospace; font-size:12.5px; color: var(--accent); white-space:nowrap; }
  .tl-org{ font-size:14px; color: var(--muted); font-weight:500; margin-bottom: 12px; }
  .tl-bullets{ margin:0; padding-left: 18px; color: var(--muted); font-size:14.5px; line-height:1.7; }
  .tl-bullets li{ margin-bottom: 5px; }
  .tl-bullets li:last-child{ margin-bottom:0; }

  .projects-grid{ display:grid; grid-template-columns: repeat(3, 1fr); gap: 20px; }
  .project-card{
    background: var(--surface); border:1px solid var(--border); border-radius: var(--radius);
    padding: 26px; box-shadow: var(--shadow); display:flex; flex-direction:column;
    transition: transform 0.25s ease, border-color 0.25s ease;
  }
  .project-card:hover{ transform: translateY(-4px); border-color: var(--accent); }
  .project-icon{
    width:42px; height:42px; border-radius:11px; background: var(--accent-soft); color: var(--accent);
    display:flex; align-items:center; justify-content:center; margin-bottom:18px;
  }
  .project-card h3{ font-size:16.5px; margin-bottom:8px; }
  .project-card p{ color: var(--muted); font-size:14px; line-height:1.6; margin:0 0 18px; flex-grow:1; }
  .project-tags{ display:flex; flex-wrap:wrap; gap:7px; margin-bottom:18px; }
  .project-tags span{
    font-family:'JetBrains Mono', monospace; font-size:11px; padding:4px 9px; border-radius:6px;
    background: var(--surface-2); color: var(--muted); border:1px solid var(--border);
  }
  .project-link{ font-size:13.5px; font-weight:600; color: var(--accent); display:inline-flex; align-items:center; gap:5px; }
  @media (max-width: 900px){ .projects-grid{ grid-template-columns: 1fr 1fr; } }
  @media (max-width: 640px){ .projects-grid{ grid-template-columns: 1fr; } }

  .cert-grid{ display:grid; grid-template-columns: repeat(4, 1fr); gap: 14px; }
  .cert-card{
    background: var(--surface); border:1px solid var(--border); border-radius: 12px;
    padding: 18px; text-align:center; box-shadow: var(--shadow);
    transition: transform 0.2s ease, border-color 0.2s ease;
  }
  .cert-card:hover{ transform: translateY(-3px); border-color: var(--accent); }
  .cert-badge{
    width:34px; height:34px; margin: 0 auto 12px; border-radius:9px;
    background: var(--accent-soft);
    color: var(--accent); display:flex; align-items:center; justify-content:center;
  }
  .cert-card .name{ font-size:13.5px; font-weight:600; line-height:1.4; margin-bottom:4px; }
  .cert-card .cat{ font-size:11.5px; color: var(--muted); font-family:'JetBrains Mono', monospace; }
  @media (max-width: 900px){ .cert-grid{ grid-template-columns: repeat(2, 1fr); } }

  .edu-list{ display:flex; flex-direction:column; gap:16px; }
  .edu-card{
    display:flex; gap: 20px; align-items:flex-start; background: var(--surface);
    border:1px solid var(--border); border-radius: var(--radius); padding: 26px; box-shadow: var(--shadow);
    flex-wrap:wrap; justify-content:space-between;
  }
  .edu-left{ display:flex; gap:20px; align-items:flex-start; flex:1; min-width:240px; }
  .edu-icon{
    width:44px; height:44px; border-radius:11px; flex-shrink:0;
    background: linear-gradient(135deg, var(--accent), var(--accent-2));
    display:flex; align-items:center; justify-content:center; color:#fff;
  }
  .edu-card h3{ font-size: 16.5px; margin-bottom:5px; }
  .edu-card .school{ color: var(--accent); font-weight:600; font-size:13.5px; margin-bottom:4px; }
  .edu-card .yr{ color: var(--muted); font-size:12.5px; font-family:'JetBrains Mono', monospace; }
  .edu-score{ text-align:right; }
  .edu-score .pct{ font-family:'Space Grotesk', sans-serif; font-weight:700; font-size:22px; color: var(--accent); }
  .edu-score .pctl{ font-size:11.5px; color: var(--muted); }

  .ach-grid{ display:grid; grid-template-columns: repeat(3, 1fr); gap: 16px; }
  .ach-card{
    display:flex; align-items:center; gap:14px; background: var(--surface); border:1px solid var(--border);
    border-radius: 12px; padding: 18px; box-shadow: var(--shadow);
    transition: transform 0.2s ease, border-color 0.2s ease;
  }
  .ach-card:hover{ transform: translateY(-3px); border-color: var(--accent); }
  .ach-icon{ width:36px; height:36px; border-radius:9px; background: var(--accent-soft); color: var(--accent); display:flex; align-items:center; justify-content:center; flex-shrink:0; }
  .ach-card span.txt{ font-size:13.5px; font-weight:500; line-height:1.4; }
  @media (max-width: 900px){ .ach-grid{ grid-template-columns: 1fr 1fr; } }
  @media (max-width: 560px){ .ach-grid{ grid-template-columns: 1fr; } }

  .contact-card{
    background: linear-gradient(135deg, var(--accent), var(--accent-2));
    border-radius: 20px; padding: 56px 44px; text-align:center; color:#fff;
    position:relative; overflow:hidden;
  }
  .contact-card h2{ font-size: clamp(1.7rem, 3.6vw, 2.4rem); }
  .contact-card p{ margin-top:14px; opacity:0.92; font-size:16px; }
  .contact-links{ margin-top:32px; display:flex; gap:12px; justify-content:center; flex-wrap:wrap; }
  .contact-links a{
    background: rgba(255,255,255,0.14); border:1px solid rgba(255,255,255,0.3);
    padding:12px 20px; border-radius:10px; font-weight:600; font-size:14px;
    display:flex; align-items:center; gap:8px; transition: background 0.2s ease, transform 0.2s ease;
  }
  .contact-links a:hover{ background: rgba(255,255,255,0.24); transform: translateY(-2px); }

  footer{ padding: 34px 0; text-align:center; color: var(--muted); font-size:13.5px; }
</style>
</head>
<body>

<header class="nav">
  <div class="nav-inner">
    <div class="brand"><span class="dot"></span>Sukumar Usurupati</div>
    <nav class="links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#experience">Experience</a>
      <a href="#projects">Projects</a>
      <a href="#certifications">Certifications</a>
      <a href="#education">Education</a>
      <a href="#achievements">Achievements</a>
      <a href="#contact">Contact</a>
    </nav>
    <div class="nav-right">
      <button class="toggle-btn" id="themeToggle" aria-label="Toggle dark mode">
        <svg id="iconSun" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><circle cx="12" cy="12" r="4"></circle><path d="M12 2v2M12 20v2M4.9 4.9l1.4 1.4M17.7 17.7l1.4 1.4M2 12h2M20 12h2M4.9 19.1l1.4-1.4M17.7 6.3l1.4-1.4"></path></svg>
        <svg id="iconMoon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" style="display:none"><path d="M21 12.8A9 9 0 1111.2 3 7 7 0 0021 12.8z"></path></svg>
      </button>
    </div>
  </div>
</header>

<section class="hero">
  <canvas id="heroCanvas"></canvas>
  <div class="wrap hero-inner">
    <div class="eyebrow"><span class="pulse"></span>Open to internships &amp; junior software / AI roles</div>
    <h1>Building at the edge of <span class="grad">AI &amp; software</span>, one project at a time.</h1>
    <p class="lead">I'm Sukumar Usurupati, a B.Tech Computer Science &amp; Engineering (AI) student who learns by building — turning coursework, internships, and curiosity about AI into working software.</p>
    <div class="hero-meta">
      <span><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 6-9 12-9 12s-9-6-9-12a9 9 0 1118 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>Ongole, Andhra Pradesh, India</span>
      <span><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"></rect><path d="M3 8h18"></path></svg>QIS College of Engineering and Technology</span>
    </div>
    <div class="cta-row">
      <a class="btn btn-primary" href="mailto:usurupatisukumar@gmail.com">Get in touch</a>
      <a class="btn btn-ghost" href="https://github.com/SukumarUsurupati-2007" target="_blank" rel="noopener">View GitHub</a>
      <a class="btn btn-ghost" href="https://www.linkedin.com/in/sukumar-usurupati-3a812331b" target="_blank" rel="noopener">LinkedIn</a>
    </div>
  </div>
  <div class="wrap">
    <div class="stats-bar reveal">
      <div class="stat"><div class="num">80%</div><div class="label">B.Tech Score</div></div>
      <div class="stat"><div class="num">5+</div><div class="label">Internships</div></div>
      <div class="stat"><div class="num">Top 3</div><div class="label">In B.Tech Batch</div></div>
    </div>
  </div>
</section>

<section id="about">
  <div class="wrap reveal">
    <div class="section-head">
      <span class="tag">About</span>
      <h2>A student who learns by shipping</h2>
    </div>
    <div class="about-grid">
      <div class="avatar">SU</div>
      <div class="about-text">
        <p>I'm a B.Tech Computer Science &amp; Engineering student (with an Artificial Intelligence specialization) at QIS College of Engineering and Technology, passionate about programming and AI. I build beginner-friendly technology solutions that simplify learning and improve accessibility to AI tools.</p>
        <p>Alongside coursework, I've completed five virtual internships across cybersecurity, software engineering, data science, AI analytics, and cloud solutions architecture — each one sharpening how I approach real-world problems with a mix of technical skill and analytical thinking.</p>
      </div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="wrap reveal">
    <div class="section-head">
      <span class="tag">Skills</span>
      <h2>Tools I reach for</h2>
      <p>A toolkit built from coursework, internships, and self-study.</p>
    </div>
    <div class="skill-group">
      <h4>Languages &amp; Development</h4>
      <div class="skills-wrap">
        <div class="skill-chip"><span class="bar"></span>Python</div>
        <div class="skill-chip"><span class="bar"></span>Java</div>
        <div class="skill-chip"><span class="bar"></span>C Programming</div>
        <div class="skill-chip"><span class="bar"></span>HTML / CSS</div>
        <div class="skill-chip"><span class="bar"></span>Flutter</div>
        <div class="skill-chip"><span class="bar"></span>Android Studio</div>
        <div class="skill-chip"><span class="bar"></span>DBMS</div>
      </div>
    </div>
    <div class="skill-group">
      <h4>AI, Data &amp; Cloud</h4>
      <div class="skills-wrap">
        <div class="skill-chip"><span class="bar"></span>Artificial Intelligence</div>
        <div class="skill-chip"><span class="bar"></span>Machine Learning</div>
        <div class="skill-chip"><span class="bar"></span>Data Analysis</div>
        <div class="skill-chip"><span class="bar"></span>Cybersecurity Basics</div>
        <div class="skill-chip"><span class="bar"></span>AWS Solutions Architecture</div>
      </div>
    </div>
    <div class="skill-group">
      <h4>Core &amp; Aptitude</h4>
      <div class="skills-wrap">
        <div class="skill-chip"><span class="bar"></span>Problem Solving</div>
        <div class="skill-chip"><span class="bar"></span>Quantitative Aptitude</div>
        <div class="skill-chip"><span class="bar"></span>Verbal Ability</div>
        <div class="skill-chip"><span class="bar"></span>Computer Technology</div>
      </div>
    </div>
  </div>
</section>

<section id="experience">
  <div class="wrap reveal">
    <div class="section-head">
      <span class="tag">Experience</span>
      <h2>Where I've worked</h2>
      <p>Five virtual internships across security, engineering, data, AI, and cloud.</p>
    </div>
    <div class="timeline">
      <div class="tl-item">
        <div class="tl-dot"></div>
        <div class="tl-head"><span class="tl-role">Cybersecurity Virtual Intern</span><span class="tl-date">December 2025</span></div>
        <div class="tl-org">Deloitte</div>
        <ul class="tl-bullets">
          <li>Participated in Deloitte's job simulation on Forage, gaining insight into the responsibilities of a cybersecurity team.</li>
          <li>Developed understanding of real-world security challenges faced by enterprise organizations.</li>
          <li>Applied analytical thinking to cybersecurity scenarios and threat assessment exercises.</li>
        </ul>
      </div>
      <div class="tl-item">
        <div class="tl-dot"></div>
        <div class="tl-head"><span class="tl-role">Software Engineering Virtual Intern</span><span class="tl-date">May – Aug 2025</span></div>
        <div class="tl-org">Accenture</div>
        <ul class="tl-bullets">
          <li>Gained exposure to multiple technical skills across the software engineering domain.</li>
          <li>Explored the software engineering field through a structured virtual internship program.</li>
          <li>Improved programming knowledge and sharpened problem-solving and analytical abilities.</li>
        </ul>
      </div>
      <div class="tl-item">
        <div class="tl-dot"></div>
        <div class="tl-head"><span class="tl-role">Data Science Virtual Intern</span><span class="tl-date">June 2025</span></div>
        <div class="tl-org">British Airways</div>
        <ul class="tl-bullets">
          <li>Participated in British Airways' job simulation on Forage, understanding data science team workflows.</li>
          <li>Gained hands-on experience with data analysis techniques used in the airline industry.</li>
          <li>Developed insights into how data science drives business decisions in large organizations.</li>
        </ul>
      </div>
      <div class="tl-item">
        <div class="tl-dot"></div>
        <div class="tl-head"><span class="tl-role">AI Analytics Virtual Intern</span><span class="tl-date">June 2025</span></div>
        <div class="tl-org">Tata</div>
        <ul class="tl-bullets">
          <li>Learned about AI analytics and its applications in real-world business contexts.</li>
          <li>Gained understanding of how AI-driven insights inform strategic decision-making.</li>
          <li>Applied foundational AI concepts to practical business problem-solving scenarios.</li>
        </ul>
      </div>
      <div class="tl-item">
        <div class="tl-dot"></div>
        <div class="tl-head"><span class="tl-role">Solutions Architecture Virtual Intern</span><span class="tl-date">May 2025</span></div>
        <div class="tl-org">Amazon Web Services (AWS)</div>
        <ul class="tl-bullets">
          <li>Participated in AWS's virtual job simulation on Forage, gaining understanding of solutions architecture.</li>
          <li>Created an architecture diagram for a real-world cloud infrastructure use case.</li>
          <li>Drafted a plain-language email explaining design decisions and cost calculations to a client.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="projects">
  <div class="wrap reveal">
    <div class="section-head">
      <span class="tag">Projects</span>
      <h2>What I've built</h2>
    </div>
    <div class="projects-grid">
      <div class="project-card">
        <div class="project-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><rect x="3" y="11" width="18" height="10" rx="2"></rect><circle cx="12" cy="5" r="2"></circle><path d="M12 7v4M8 16h.01M16 16h.01"></path></svg></div>
        <h3>AI Learning Assistant</h3>
        <p>A beginner-friendly AI tool that helps students learn new topics easily, using structured explanations focused on accessibility for those new to programming and AI.</p>
        <div class="project-tags"><span>Python</span><span>AI</span><span>Education</span></div>
        <a class="project-link" href="https://github.com/SukumarUsurupati-2007" target="_blank" rel="noopener">View on GitHub →</a>
      </div>
      <div class="project-card">
        <div class="project-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><circle cx="12" cy="12" r="9"></circle><path d="M3 12h18M12 3a14 14 0 010 18M12 3a14 14 0 000 18"></path></svg></div>
        <h3>Web Development Projects</h3>
        <p>A collection of web projects built with HTML and CSS fundamentals, demonstrating responsive layout techniques and clean interface design.</p>
        <div class="project-tags"><span>HTML</span><span>CSS</span><span>Web</span></div>
        <a class="project-link" href="https://github.com/SukumarUsurupati-2007" target="_blank" rel="noopener">View on GitHub →</a>
      </div>
      <div class="project-card">
        <div class="project-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><rect x="3" y="3" width="18" height="18" rx="2"></rect><path d="M3 9h18M8 21V9"></path></svg></div>
        <h3>Personal Portfolio Website</h3>
        <p>Designed and developed a personal portfolio showcasing my introduction, skills, projects, and experience — built with pure HTML, CSS, and JavaScript, dark mode, and animations.</p>
        <div class="project-tags"><span>HTML</span><span>CSS</span><span>JavaScript</span></div>
        <a class="project-link" href="https://github.com/SukumarUsurupati-2007/Portfolio" target="_blank" rel="noopener">View on GitHub →</a>
      </div>
    </div>
  </div>
</section>

<section id="certifications">
  <div class="wrap reveal">
    <div class="section-head">
      <span class="tag">Credentials</span>
      <h2>Certifications</h2>
    </div>
    <div class="cert-grid">
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2l3 7h7l-5.5 4.5L18 21l-6-4-6 4 1.5-7.5L2 9h7z"></path></svg></div><div class="name">Entrepreneurship &amp; Innovation</div><div class="cat">Job Simulation</div></div>
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16v16H4z"></path><path d="M9 9h6v6H9z"></path></svg></div><div class="name">CSS Basics</div><div class="cat">Web Development</div></div>
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="8" width="14" height="10" rx="2"></rect><path d="M9 8V6a3 3 0 016 0v2M9 13h.01M15 13h.01"></path></svg></div><div class="name">Robotics &amp; Controls</div><div class="cat">Job Simulation</div></div>
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="9" cy="8" r="3"></circle><circle cx="17" cy="8" r="2.4"></circle><path d="M3 20c0-3.3 2.7-6 6-6s6 2.7 6 6M15.5 14.3c2.5.4 4.5 2.6 4.5 5.7"></path></svg></div><div class="name">Professional Networking</div><div class="cat">Career Growth</div></div>
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 19V9M10 19V5M16 19v-7M4 19h16"></path></svg></div><div class="name">Data Analysis for Flipkart</div><div class="cat">Data Analytics</div></div>
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"></circle><path d="M12 8v4l3 2"></path></svg></div><div class="name">AI Fluency: Framework &amp; Foundations</div><div class="cat">Artificial Intelligence</div></div>
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9.5 3a5.5 5.5 0 015.5 5.5c0 1.6-.7 3-1.8 4M14.5 21a5.5 5.5 0 01-5.5-5.5c0-1.6.7-3 1.8-4"></path></svg></div><div class="name">AIML &amp; Data Science</div><div class="cat">AI &amp; ML</div></div>
      <div class="cert-card"><div class="cert-badge"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2l3 7h7l-5.5 4.5L18 21l-6-4-6 4 1.5-7.5L2 9h7z"></path></svg></div><div class="name">Naukri Campus Young Turks 2025</div><div class="cat">Campus Recognition</div></div>
    </div>
  </div>
</section>

<section id="education">
  <div class="wrap reveal">
    <div class="section-head">
      <span class="tag">Education</span>
      <h2>Academic journey</h2>
    </div>
    <div class="edu-list">
      <div class="edu-card">
        <div class="edu-left">
          <div class="edu-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M22 10L12 5 2 10l10 5 10-5z"></path><path d="M6 12.5V17c0 1.5 3 3 6 3s6-1.5 6-3v-4.5"></path></svg></div>
          <div>
            <div class="school">QIS College of Engineering and Technology, Prakasam</div>
            <h3>B.Tech in Computer Science &amp; Engineering (AI)</h3>
            <div class="yr">Currently pursuing</div>
          </div>
        </div>
        <div class="edu-score"><div class="pct">80%</div><div class="pctl">Current Score</div></div>
      </div>
      <div class="edu-card">
        <div class="edu-left">
          <div class="edu-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M22 10L12 5 2 10l10 5 10-5z"></path><path d="M6 12.5V17c0 1.5 3 3 6 3s6-1.5 6-3v-4.5"></path></svg></div>
          <div>
            <div class="school">Board of Intermediate Education, Andhra Pradesh</div>
            <h3>Intermediate — Class XII</h3>
            <div class="yr">Year of Passing: 2024</div>
          </div>
        </div>
        <div class="edu-score"><div class="pct">78.8%</div><div class="pctl">Score</div></div>
      </div>
      <div class="edu-card">
        <div class="edu-left">
          <div class="edu-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M22 10L12 5 2 10l10 5 10-5z"></path><path d="M6 12.5V17c0 1.5 3 3 6 3s6-1.5 6-3v-4.5"></path></svg></div>
          <div>
            <div class="school">Board of Secondary Education, Andhra Pradesh</div>
            <h3>Secondary School — Class X</h3>
            <div class="yr">Year of Passing: 2022</div>
          </div>
        </div>
        <div class="edu-score"><div class="pct">79%</div><div class="pctl">Score</div></div>
      </div>
    </div>
  </div>
</section>

<section id="achievements">
  <div class="wrap reveal">
    <div class="section-head">
      <span class="tag">Recognition</span>
      <h2>Achievements</h2>
    </div>
    <div class="ach-grid">
      <div class="ach-card"><div class="ach-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2l3 7h7l-5.5 4.5L18 21l-6-4-6 4 1.5-7.5L2 9h7z"></path></svg></div><span class="txt">Top 3 Student in B.Tech Program</span></div>
      <div class="ach-card"><div class="ach-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"></circle><path d="M12 7v5l3 3"></path></svg></div><span class="txt">School Topper &amp; Academic Achiever</span></div>
      <div class="ach-card"><div class="ach-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="9" cy="8" r="3"></circle><circle cx="17" cy="8" r="2.4"></circle><path d="M3 20c0-3.3 2.7-6 6-6s6 2.7 6 6"></path></svg></div><span class="txt">Recognized for Leadership &amp; Teamwork</span></div>
      <div class="ach-card"><div class="ach-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 19.5A2.5 2.5 0 016.5 17H20"></path><path d="M6.5 2H20v20H6.5A2.5 2.5 0 014 19.5v-15A2.5 2.5 0 016.5 2z"></path></svg></div><span class="txt">Community Tutor &amp; Volunteer Educator</span></div>
      <div class="ach-card"><div class="ach-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 20V10M18 20V4M6 20v-6"></path></svg></div><span class="txt">JEE Mains Rank: 50,000</span></div>
      <div class="ach-card"><div class="ach-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2l8 4v6c0 5-3.5 8-8 10-4.5-2-8-5-8-10V6z"></path></svg></div><span class="txt">NCC Certificate Holder</span></div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="wrap reveal">
    <div class="contact-card">
      <h2>Let's build something together</h2>
      <p>Open to internships, entry-level roles, and collaborative projects in AI &amp; software development.</p>
      <div class="contact-links">
        <a href="mailto:usurupatisukumar@gmail.com"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="4" width="20" height="16" rx="2"></rect><path d="M2 7l10 6 10-6"></path></svg>Email</a>
        <a href="tel:+917013578544"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.9v3a2 2 0 01-2.2 2 19.8 19.8 0 01-8.6-3.1 19.5 19.5 0 01-6-6A19.8 19.8 0 012.1 4.2 2 2 0 014.1 2h3a2 2 0 012 1.7c.1 1 .3 2 .7 3a2 2 0 01-.4 2.1L8 10.3a16 16 0 006 6l1.5-1.4a2 2 0 012.1-.4c1 .4 2 .6 3 .7a2 2 0 011.7 2z"></path></svg>+91 7013578544</a>
        <a href="https://www.linkedin.com/in/sukumar-usurupati-3a812331b" target="_blank" rel="noopener"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle><path d="M10 9v12M10 13a4 4 0 018 0v8"></path></svg>LinkedIn</a>
        <a href="https://github.com/SukumarUsurupati-2007" target="_blank" rel="noopener"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 19c-4.3 1.4-4.3-2.5-6-3m12 5v-3.5c0-1 .1-1.4-.5-2 2.8-.3 5.5-1.4 5.5-6a4.6 4.6 0 00-1.3-3.2 4.2 4.2 0 00-.1-3.2s-1.1-.3-3.5 1.3a12.3 12.3 0 00-6.2 0C6.7 2.8 5.6 3.1 5.6 3.1a4.2 4.2 0 00-.1 3.2A4.6 4.6 0 004.2 9.5c0 4.6 2.7 5.7 5.5 6-.6.6-.6 1.2-.5 2V21"></path></svg>GitHub</a>
        <a href="#about"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 6-9 12-9 12s-9-6-9-12a9 9 0 1118 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>Ongole, AP, India</a>
      </div>
    </div>
  </div>
</section>

<footer>
  &copy; <span id="year"></span> Sukumar Usurupati. Designed &amp; built with curiosity and code.
</footer>

<script>
  const root = document.documentElement;
  const themeToggle = document.getElementById('themeToggle');
  const iconSun = document.getElementById('iconSun');
  const iconMoon = document.getElementById('iconMoon');

  function applyTheme(t){
    if(t === 'dark'){
      root.classList.add('dark');
      iconSun.style.display = 'none';
      iconMoon.style.display = 'block';
    } else {
      root.classList.remove('dark');
      iconSun.style.display = 'block';
      iconMoon.style.display = 'none';
    }
  }
  let saved = null;
  try{ saved = localStorage.getItem('portfolio-theme'); }catch(e){}
  const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
  applyTheme(saved || (prefersDark ? 'dark' : 'light'));

  themeToggle.addEventListener('click', () => {
    const isDark = root.classList.contains('dark');
    const next = isDark ? 'light' : 'dark';
    applyTheme(next);
    try{ localStorage.setItem('portfolio-theme', next); }catch(e){}
  });

  document.getElementById('year').textContent = new Date().getFullYear();

  const revealEls = document.querySelectorAll('.reveal');
  const io = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if(entry.isIntersecting){
        entry.target.classList.add('in');
        io.unobserve(entry.target);
      }
    });
  }, { threshold: 0.12 });
  revealEls.forEach(el => io.observe(el));

  const canvas = document.getElementById('heroCanvas');
  const ctx = canvas.getContext('2d');
  let w, h, nodes = [];
  const reduceMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;

  function resize(){
    const hero = canvas.parentElement;
    w = canvas.width = hero.offsetWidth;
    h = canvas.height = hero.offsetHeight;
  }
  function initNodes(){
    const count = Math.min(46, Math.floor((w*h)/26000));
    nodes = Array.from({length: count}, () => ({
      x: Math.random()*w,
      y: Math.random()*h,
      vx: (Math.random()-0.5)*0.25,
      vy: (Math.random()-0.5)*0.25,
    }));
  }
  function getAccentColor(){
    return getComputedStyle(root).getPropertyValue('--accent').trim() || '#4a56e2';
  }
  function draw(){
    ctx.clearRect(0,0,w,h);
    const accent = getAccentColor();
    nodes.forEach(n => {
      n.x += n.vx; n.y += n.vy;
      if(n.x < 0 || n.x > w) n.vx *= -1;
      if(n.y < 0 || n.y > h) n.vy *= -1;
    });
    for(let i=0;i<nodes.length;i++){
      for(let j=i+1;j<nodes.length;j++){
        const dx = nodes[i].x-nodes[j].x, dy = nodes[i].y-nodes[j].y;
        const dist = Math.sqrt(dx*dx+dy*dy);
        if(dist < 140){
          ctx.strokeStyle = accent;
          ctx.globalAlpha = (1 - dist/140) * 0.35;
          ctx.lineWidth = 1;
          ctx.beginPath();
          ctx.moveTo(nodes[i].x, nodes[i].y);
          ctx.lineTo(nodes[j].x, nodes[j].y);
          ctx.stroke();
        }
      }
    }
    ctx.globalAlpha = 0.8;
    nodes.forEach(n => {
      ctx.fillStyle = accent;
      ctx.beginPath();
      ctx.arc(n.x, n.y, 2, 0, Math.PI*2);
      ctx.fill();
    });
    ctx.globalAlpha = 1;
    if(!reduceMotion) requestAnimationFrame(draw);
  }
  function start(){
    resize(); initNodes(); draw();
  }
  window.addEventListener('resize', () => { resize(); initNodes(); if(reduceMotion) draw(); });
  start();

  document.querySelectorAll('nav.links a').forEach(link => {
    link.addEventListener('click', (e) => {
      const target = document.querySelector(link.getAttribute('href'));
      if(target){
        e.preventDefault();
        target.scrollIntoView({ behavior: 'smooth', block: 'start' });
      }
    });
  });
</script>

</body>
</html>
