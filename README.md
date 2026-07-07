#Portfolio
This is my portfolio wedsite
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
<link rel="stylesheet" href="styles.css">
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
      <a class="btn btn-ghost" href="https://github.com/USURUPATI-SUKUMAR" target="_blank" rel="noopener">View GitHub</a>
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
        <a class="project-link" href="https://github.com/USURUPATI-SUKUMAR" target="_blank" rel="noopener">View on GitHub →</a>
      </div>
      <div class="project-card">
        <div class="project-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><circle cx="12" cy="12" r="9"></circle><path d="M3 12h18M12 3a14 14 0 010 18M12 3a14 14 0 000 18"></path></svg></div>
        <h3>Web Development Projects</h3>
        <p>A collection of web projects built with HTML and CSS fundamentals, demonstrating responsive layout techniques and clean interface design.</p>
        <div class="project-tags"><span>HTML</span><span>CSS</span><span>Web</span></div>
        <a class="project-link" href="https://github.com/USURUPATI-SUKUMAR" target="_blank" rel="noopener">View on GitHub →</a>
      </div>
      <div class="project-card">
        <div class="project-icon"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><rect x="3" y="3" width="18" height="18" rx="2"></rect><path d="M3 9h18M8 21V9"></path></svg></div>
        <h3>Personal Portfolio Website</h3>
        <p>Designed and developed a personal portfolio showcasing my introduction, skills, projects, and experience — built with pure HTML, CSS, and JavaScript, dark mode, and animations.</p>
        <div class="project-tags"><span>HTML</span><span>CSS</span><span>JavaScript</span></div>
        <a class="project-link" href="https://github.com/USURUPATI-SUKUMAR/Portfolio" target="_blank" rel="noopener">View on GitHub →</a>
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
        <a href="https://github.com/USURUPATI-SUKUMAR" target="_blank" rel="noopener"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 19c-4.3 1.4-4.3-2.5-6-3m12 5v-3.5c0-1 .1-1.4-.5-2 2.8-.3 5.5-1.4 5.5-6a4.6 4.6 0 00-1.3-3.2 4.2 4.2 0 00-.1-3.2s-1.1-.3-3.5 1.3a12.3 12.3 0 00-6.2 0C6.7 2.8 5.6 3.1 5.6 3.1a4.2 4.2 0 00-.1 3.2A4.6 4.6 0 004.2 9.5c0 4.6 2.7 5.7 5.5 6-.6.6-.6 1.2-.5 2V21"></path></svg>GitHub</a>
        <a href="#about"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 6-9 12-9 12s-9-6-9-12a9 9 0 1118 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>Ongole, AP, India</a>
      </div>
    </div>
  </div>
</section>

<footer>
  &copy; <span id="year"></span> Sukumar Usurupati. Designed &amp; built with curiosity and code.
</footer>

<script src="script.js"></script>

</body>
</html>
