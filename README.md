<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Saqib Anjum — Portfolio Readme</title>
  <meta name="description" content="Vishal Kumar Chaubey — Full Stack Developer (React Native, Node.js). Portfolio-style README converted to a modern single-file HTML/CSS layout." />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; /* dark navy */
      --card:#0b1220;
      --muted:#9aa4b2;
      --accent:#36bcf7;
      --glass: rgba(255,255,255,0.04);
      --glass-strong: rgba(255,255,255,0.06);
      --radius:14px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%;}
    body{
      margin:0;
      font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      background: linear-gradient(180deg,#071027 0%, #071428 45%, #051025 100%);
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding:40px 24px;
    }

    .container{
      max-width:1100px;
      margin:0 auto;
    }

    /* Header / hero */
    .hero{
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:26px;
      align-items:center;
      margin-bottom:28px;
    }
    .hero-card{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:var(--radius);
      padding:28px;
      box-shadow: 0 6px 20px rgba(2,6,23,0.6);
      border: 1px solid rgba(255,255,255,0.03);
    }

    .title{
      font-weight:800;
      font-size:28px;
      margin:0 0 8px 0;
    }
    .subtitle{
      display:block;
      margin-bottom:14px;
      color:var(--muted);
      font-size:14px;
    }
    .typing-banner{max-width:100%;border-radius:10px;overflow:hidden}

    .badges{display:flex;gap:8px;flex-wrap:wrap;margin-top:12px}
    .badge img{height:36px}

    /* Profile widget */
    .profile-card{background:linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:var(--radius);padding:18px;text-align:center;border:1px solid rgba(255,255,255,0.03);}
    .profile-card img.avatar{width:100%;border-radius:10px;display:block}
    .profile-links{display:flex;gap:8px;flex-direction:column;margin-top:12px}
    .profile-links a{display:inline-block}

    /* sections */
    section{margin-top:22px}
    h2{font-size:18px;margin:0 0 12px 0}
    p.lead{color:var(--muted);margin:0 0 12px 0}

    /* tech stack */
    .tech{
      display:flex;flex-wrap:wrap;gap:10px;align-items:center;justify-content:center;
      padding:14px;background:var(--glass);border-radius:12px;border:1px solid rgba(255,255,255,0.02)
    }
    .tech img{height:46px}

    /* stats */
    .stats{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:12px}
    .stat-card{background:var(--card);padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,0.02)}
    .stat-card img{width:100%;height:auto;display:block}

    /* projects grid */
    .projects-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:12px}
    .project{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,0.03);min-height:120px;display:flex;flex-direction:column;justify-content:space-between}
    .project h3{margin:0 0 8px 0;font-size:15px}
    .project p{margin:0;color:var(--muted);font-size:13px}
    .project .tag{font-size:12px;padding:6px 10px;border-radius:999px;background:rgba(255,255,255,0.02);display:inline-block;margin-top:10px}

    /* process */
    .process{display:flex;gap:10px;flex-wrap:wrap}
    .process .step{flex:1;min-width:160px;background:var(--glass-strong);padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.02)}
    .process .step h4{margin:0 0 6px 0}
    .process .step p{margin:0;color:var(--muted);font-size:13px}

    /* contact/footer */
    footer{margin-top:28px;padding:18px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));border:1px solid rgba(255,255,255,0.02)}
    .links{display:flex;gap:10px;flex-wrap:wrap}

    /* small screens */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr;}
      .projects-grid{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:520px){
      .projects-grid{grid-template-columns:1fr}
      .stats{grid-template-columns:1fr}
      .badges img{height:30px}
    }

    /* subtle hover */
    .project:hover{transform:translateY(-6px);transition:transform .2s ease;box-shadow:0 10px 30px rgba(2,8,23,0.6)}

    /* theme toggle */
    .theme-toggle{position:fixed;right:20px;bottom:20px;background:linear-gradient(90deg,#0b1220,#0e2230);padding:10px;border-radius:999px;border:1px solid rgba(255,255,255,0.03);cursor:pointer}
    .theme-toggle svg{display:block}
  </style>
</head>
<body>
  <div class="container">
    <header class="hero">
      <div class="hero-card">
        <h1 class="title">Saqib Anjum</h1>
        <div class="subtitle">MERN Stack Developer • Full Stack Developer • React Native &amp; Node.js • WordPress Developer</div>

        <div class="typing-banner">
          <!-- Re-using readme-typing SVG banner -->
          <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=32&pause=1000&color=36BCF7FF&center=true&vCenter=true&width=760&lines=Full+Stack+Developer;React+Native+Expert;Node.js+Developer;JavaScript+Educator" alt="typing" style="width:100%;border-radius:10px;display:block">
        </div>

        <p class="lead">I’m a MERN Stack Developer who loves crafting websites with React.js, Next.js,
 Node.js, and modern JavaScript. I thrive on writing clean, scalable code that helps
 projects grow and I’m always excited to learn new tools and stay ahead of the latest
 web trends.</p>

        <div class="badges">
          <div class="badge"><a href="https://www.linkedin.com/in/saqib-anjum/" target="_blank" rel="noopener"><img src="https://img.shields.io/badge/Saqib-5?style=for-the-badge&logo=any%20text%3A%20you%20like&logoColor=%23fff&label=LinkedIn" alt="LinkedIn"></a></div>
          <!-- <div class="badge"><a href="https://youtube.com/@_codsod" target="_blank" rel="noopener"><img src="https://img.shields.io/badge/YouTube-codsod-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube"></a></div> -->
          <div class="badge"><a href="mailto:saqib.id2050@gmail.com"><img src="https://img.shields.io/badge/Saqib-5?style=for-the-badge&logo=any%20text%3A%20you%20like&logoColor=%23fff&label=Email" alt="Email"></a></div>
          <div class="badge"><a href="https://github.com/Saqib-Anjum/" target="_blank" rel="noopener"><img src="https://img.shields.io/badge/Saqib-5?style=for-the-badge&logo=any%20text%3A%20you%20like&logoColor=%23fff&label=Github" alt="GitHub"></a></div>
        </div>

      </div>

      <aside class="profile-card">
        <!-- small profile widget: you can replace the img with a real avatar or a GitHub widget -->
        <img class="avatar" src="https://github-readme-stats.vercel.app/api?username=Saqib-Anjum&show_icons=true&theme=radical&hide_border=true" alt="GitHub Stats">
        <div class="profile-links">
          <a href="vercel.app" target="_blank">Portfolio • View site</a>
          <!-- <a href="https://youtube.com/@_codsod" target="_blank">YouTube • codsod</a> -->
          <a href="mailto:saqib.id2050@gmail.com">Email • saqib.id2050@gmail.com</a>
        </div>
      </aside>
    </header>

    <main>
      <section>
        <h2>🛠️ Tech Stack</h2>
        <div class="tech">
          <img src="https://skillicons.dev/icons?i=react,nodejs,express,js,ts,mongodb,html,css,git,vscode,Wordpress" alt="tech icons">
        </div>
      </section>

      <section>
        <h2>📊 GitHub Analytics</h2>
        <div class="stats">
          <div class="stat-card"><img src="https://github-readme-stats.vercel.app/api?username=Saqib-Anjum&show_icons=true&theme=radical&hide_border=true" alt="github-stats" /></div>
          <div class="stat-card"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Saqib-Anjum&layout=compact&theme=radical&hide_border=true" alt="top-langs" /></div>
        </div>
      </section>

      <section>
        <h2>🚀 Featured Projects</h2>
        <div class="projects-grid">
          <article class="project">
            <div>
             <h3>Ticket Dashboard</h3>
              <p>Responsive React/Node admin dashboard with real-time customizable menus.</p>
            </div>
            <div>
              <span class="tag">React • Node</span>
            </div>
          </article>

          <article class="project">
            <div>
              <h3>Business Appointment CRM</h3>
              <p> React/Node business CRM with real-time appointments, charts & notifications also along with role management system.</p>
            </div>
            <div>
              <span class="tag">React • Node.js</span>
            </div>
          </article>

          <article class="project">
            <div>
              <h3>Patient Dashboard</h3>
              <p>React/Node patient dashboard with real-time patients appointments.</p>
            </div>
            <div>
              <span class="tag">Node.js • Express</span>
            </div>
          </article>
        </div>
        <!-- <p style="margin-top:10px;color:var(--muted)">Tip: Replace these placeholders with screenshots and live links — images increase engagement.</p> -->
      </section>

      <section>
        <h2>♨️ Work Process</h2>
        <div class="process">
          <div class="step"><h4>1. Discover</h4><p>Understand the problem & roadmap.</p></div>
          <div class="step"><h4>2. Design</h4><p>API and component architecture.</p></div>
          <div class="step"><h4>3. Build</h4><p>Iterative development + tests.</p></div>
          <div class="step"><h4>4. Ship</h4><p>CI/CD and documentation.</p></div>
        </div>
      </section>

      <section>
        <h2>🎯 Learning & Teaching</h2>
        <p class="lead">Currently learning GraphQL, React Native, AWS Services, and Advanced Animations. </p>
      </section>

    </main>

    <footer>
      <div style="display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap">
        <div>
          <strong>📫 Contact</strong>
          <div style="color:var(--muted)">Email: <a href="mailto:saqib.id2050@gmail.com">saqib.id2050@gmail.com</a> • Portfolio: <a href="vercel.app" target="_blank">vercel.app</a></div>
        </div>
        <div class="links">
          <a href="https://www.linkedin.com/in/saqib-anjum/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="linkedin"></a>
          <a href="https://github.com/Saqib-Anjum/" target="_blank"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="github"></a>
        </div>
      </div>
    </footer>

  </div>

  <button class="theme-toggle" title="Toggle theme (light/dark)">
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none"><path d="M12 3v2" stroke="#9fb3c8" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/><path d="M21 12h-2" stroke="#9fb3c8" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/><path d="M12 21v-2" stroke="#9fb3c8" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/><path d="M3 12h2" stroke="#9fb3c8" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/><circle cx="12" cy="12" r="3" stroke="#9fb3c8" stroke-width="1.5"/></svg>
  </button>

  <script>
    // theme toggle: simple inversion (light mode adjustments)
    const toggle = document.querySelector('.theme-toggle');
    let light = false;
    toggle.addEventListener('click', ()=>{
      light = !light;
      if(light){
        document.documentElement.style.setProperty('--bg','#f7fafc');
        document.documentElement.style.setProperty('--card','#ffffff');
        document.documentElement.style.setProperty('--muted','#475569');
        document.documentElement.style.setProperty('--accent','#0ea5e9');
        document.documentElement.style.setProperty('--glass','rgba(2,6,23,0.03)');
        document.body.style.background = 'linear-gradient(180deg,#f8fafc 0%, #eef2f7 45%, #f8fafc 100%)';
        document.body.style.color = '#071124';
      } else {
        document.documentElement.style.setProperty('--bg','#0f1724');
        document.documentElement.style.setProperty('--card','#0b1220');
        document.documentElement.style.setProperty('--muted','#9aa4b2');
        document.documentElement.style.setProperty('--accent','#36bcf7');
        document.documentElement.style.setProperty('--glass','rgba(255,255,255,0.04)');
        document.body.style.background = 'linear-gradient(180deg,#071027 0%, #071428 45%, #051025 100%)';
        document.body.style.color = '#e6eef6';
      }
    });
  </script>

</body>
</html>
