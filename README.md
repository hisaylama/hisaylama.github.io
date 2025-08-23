<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Hisay Lama — Portfolio</title>
  <meta name="description" content="Portfolio of Hisay Lama — experimental soft‑matter physicist exploring statistical physics, quantitative image analysis, and machine learning." />
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='0.9em' font-size='80'>🧪</text></svg>">
  <meta property="og:title" content="Hisay Lama — Portfolio" />
  <meta property="og:description" content="Experimental soft‑matter physics · statistical physics · ML · quantitative research" />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://hisaylama.github.io" />
  <style>
    :root{
      --bg: #0b0c0f; --bg-soft:#12141a; --text:#e7e9ea; --muted:#9aa0a6; --card:#161922; --accent:#7cc5ff; --chip:#222630; --border:#23272f; --link:#9fd3ff;
    }
    [data-theme="light"]{ --bg:#ffffff; --bg-soft:#f7f9fc; --text:#0b0c0f; --muted:#495057; --card:#ffffff; --accent:#0ea5e9; --chip:#eef2f7; --border:#e6eaf0; --link:#0369a1; }
    html,body{margin:0;padding:0;background:var(--bg);color:var(--text);font:16px/1.6 system-ui, -apple-system, Segoe UI, Roboto, Inter, "Helvetica Neue", Arial, Noto Sans, "Apple Color Emoji","Segoe UI Emoji";}
    a{color:var(--link);text-decoration:none} a:hover{text-decoration:underline}
    .wrap{max-width:1050px;margin:0 auto;padding:24px}
    header{position:sticky;top:0;backdrop-filter:saturate(180%) blur(8px);background:color-mix(in hsl, var(--bg) 88%, transparent);border-bottom:1px solid var(--border);z-index:50}
    nav{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;align-items:center;gap:10px;font-weight:700}
    .brand .dot{width:10px;height:10px;border-radius:50%;background:var(--accent)}
    .navlinks{display:flex;gap:18px;flex-wrap:wrap}
    .navlinks a{padding:8px 10px;border-radius:10px}
    .navlinks a:hover{background:var(--chip)}
    .toggle{border:1px solid var(--border);background:var(--chip);padding:6px 10px;border-radius:999px;cursor:pointer}

    .hero{display:grid;grid-template-columns:1.2fr .8fr;gap:28px;align-items:center;padding:44px 0}
    .badge{display:inline-flex;gap:8px;align-items:center;background:var(--chip);border:1px solid var(--border);padding:6px 10px;border-radius:999px;font-size:12px;color:var(--muted)}
    h1{font-size:clamp(28px, 4vw, 42px);margin:10px 0 6px}
    .lead{font-size:clamp(16px, 1.8vw, 19px);color:var(--muted);margin:0 0 12px}
    .cta{display:flex;gap:12px;flex-wrap:wrap;margin-top:12px}
    .btn{display:inline-flex;align-items:center;gap:8px;border:1px solid var(--border);padding:10px 14px;border-radius:12px;background:var(--card)}
    .btn.primary{background:var(--accent);color:#051018;border-color:transparent}

    .chips{display:flex;gap:8px;flex-wrap:wrap;margin-top:14px}
    .chip{background:var(--chip);border:1px solid var(--border);padding:6px 10px;border-radius:999px;font-size:12px;color:var(--muted)}

    section{padding:18px 0 28px}
    .section-title{display:flex;align-items:center;justify-content:space-between;margin:4px 0 16px}
    .section-title h2{margin:0;font-size:22px}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:16px}

    .card{background:var(--card);border:1px solid var(--border);border-radius:16px;padding:16px}
    .card h3{margin:0 0 6px;font-size:18px}
    .card p{margin:0 0 8px;color:var(--muted)}
    .card .meta{display:flex;gap:8px;flex-wrap:wrap}
    .meta span{font-size:12px;color:var(--muted);background:var(--chip);border:1px solid var(--border);padding:4px 8px;border-radius:999px}

    .two-col{display:grid;grid-template-columns:1fr 1fr;gap:16px}
    .two-col .card ul{margin:0 0 0 20px}

    footer{border-top:1px solid var(--border);padding:24px 0;margin-top:32px;color:var(--muted)}

    @media (max-width:900px){.hero{grid-template-columns:1fr}.navlinks{display:none}}
  </style>
  <script>
    // Simple theme toggle persisted in localStorage
    const setTheme = (t)=>{ document.documentElement.setAttribute('data-theme', t); localStorage.setItem('theme', t); };
    const stored = typeof localStorage !== 'undefined' && localStorage.getItem('theme');
    if(stored){ document.documentElement.setAttribute('data-theme', stored); }
    function toggleTheme(){ setTheme(document.documentElement.getAttribute('data-theme')==='light'?'dark':'light'); }
  </script>
</head>
<body>
  <header>
    <div class="wrap">
      <nav>
        <div class="brand"><span class="dot"></span><span>Hisay Lama</span></div>
        <div class="navlinks">
          <a href="#projects">Projects</a>
          <a href="#pubs">Publications</a>
          <a href="#teaching">Teaching</a>
          <a href="#contact">Contact</a>
        </div>
        <button class="toggle" onclick="toggleTheme()" aria-label="Toggle theme">Toggle theme</button>
      </nav>
    </div>
  </header>

  <main class="wrap">
    <section class="hero">
      <div>
        <span class="badge">Experimental Soft‑Matter Physics · Statistical Physics · ML</span>
        <h1>Hi, I’m <span style="white-space:nowrap">Hisay Lama</span>.</h1>
        <p class="lead">I explore the physics of soft and complex materials and use quantitative image analysis, simulation, and machine learning to extract structure, dynamics, and function. I also build tools and models for data‑driven research and quantitative finance.</p>
        <div class="cta">
          <a class="btn primary" href="#projects">See projects</a>
          <a class="btn" href="cv.pdf" target="_blank" rel="noopener">Download CV</a>
          <a class="btn" href="mailto:hisaylama@gmail.com">Email me</a>
        </div>
        <div class="chips">
          <span class="chip">Monte Carlo</span>
          <span class="chip">Image Processing</span>
          <span class="chip">PyTorch / JAX</span>
          <span class="chip">MATLAB</span>
          <span class="chip">Quant Research</span>
        </div>
      </div>
      <div class="card">
        <h3>At a glance</h3>
        <p class="muted" style="margin-top:-4px">Researcher · Imperial College London · Open‑source contributor</p>
        <div class="two-col" style="margin-top:10px">
          <div>
            <strong>Areas</strong>
            <ul>
              <li>Soft‑Matter & Statistical Physics</li>
              <li>Quantitative Image Analysis</li>
              <li>Machine Learning & Simulation</li>
            </ul>
          </div>
          <div>
            <strong>Now</strong>
            <ul>
              <li>Modeling intermittent search & MFPT</li>
              <li>Financial ML: sentiment & volatility</li>
              <li>Molecular graph learning</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section id="projects">
      <div class="section-title">
        <h2>Featured Projects</h2>
        <a href="https://github.com/hisaylama" target="_blank" rel="noopener">All repositories →</a>
      </div>
      <div class="grid">
        <article class="card">
          <h3><a href="https://github.com/hisaylama/AFM-data-height-profile-analysis" target="_blank" rel="noopener">AFM HeightProfileApp</a></h3>
          <p>MATLAB app to visualize AFM surfaces, extract line profiles, perform baseline correction, and fit peaks; exports results to CSV.</p>
          <div class="meta"><span>MATLAB</span><span>AFM</span><span>Gaussian fits</span></div>
        </article>
        <article class="card">
          <h3><a href="https://github.com/hisaylama/Statistical_Physics_Algorithm_Computation" target="_blank" rel="noopener">Statistical Physics Algorithms</a></h3>
          <p>Notebook collection: sampling/integration, path integrals, Bose‑Einstein stats, and Ising model Monte Carlo.</p>
          <div class="meta"><span>Jupyter</span><span>Monte Carlo</span><span>Ising</span></div>
        </article>
        <article class="card">
          <h3><a href="https://github.com/hisaylama/Phase-Mask-for-Spatial-Light-Modulator" target="_blank" rel="noopener">Phase Masks for SLM</a></h3>
          <p>Implements Gerchberg–Saxton algorithm to generate phase masks for spatial light modulators in Fourier optics.</p>
          <div class="meta"><span>Fourier optics</span><span>SLM</span><span>MATLAB</span></div>
        </article>
        <article class="card">
          <h3><a href="https://www.kaggle.com/code/hisaylama/titanic-probelm" target="_blank" rel="noopener">Kaggle: Titanic</a></h3>
          <p>Classic ML workflow baseline with feature engineering and model comparison for the Titanic dataset.</p>
          <div class="meta"><span>Kaggle</span><span>Classification</span></div>
        </article>
      </div>
    </section>

    <section id="pubs">
      <div class="section-title">
        <h2>Publications & Preprints</h2>
        <a href="#" onclick="alert('Replace this list with your publications — see HTML comments in source.');return false;">How to edit</a>
      </div>
      <div class="card">
        <ul>
          <!-- Replace with real entries; sample format below -->
          <li><strong>Author</strong>, <em>Paper title</em>, Journal (Year). <a href="#">PDF</a> · <a href="#">DOI</a></li>
          <li><strong>Author</strong>, <em>Paper title</em>, arXiv:xxxx.xxxxx (Year). <a href="#">arXiv</a></li>
        </ul>
      </div>
    </section>

    <section id="teaching">
      <div class="section-title"><h2>Teaching & Talks</h2></div>
      <div class="grid">
        <div class="card">
          <h3>Selected talks</h3>
          <ul>
            <li>Intermittent search strategies: MFPT scaling</li>
            <li>Quantitative imaging of soft interfaces</li>
          </ul>
        </div>
        <div class="card">
          <h3>Course & mentoring</h3>
          <ul>
            <li>Computational Finance — self‑designed syllabus</li>
            <li>Harvard Stats — probability & inference</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="section-title"><h2>Contact & Links</h2></div>
      <div class="grid">
        <div class="card">
          <p><strong>Email:</strong> <a href="mailto:hisaylama@gmail.com">hisaylama@gmail.com</a></p>
          <p><strong>GitHub:</strong> <a href="https://github.com/hisaylama" target="_blank" rel="noopener">@hisaylama</a></p>
          <p><strong>Kaggle:</strong> <a href="https://www.kaggle.com/hisaylama" target="_blank" rel="noopener">/hisaylama</a></p>
          <p><strong>LinkedIn:</strong> <a href="#" target="_blank" rel="noopener">Add your link</a></p>
          <p><strong>Location:</strong> London, U.K.</p>
        </div>
        <div class="card">
          <h3>How to edit</h3>
          <ol>
            <li>Click the ✏️ icon in the GitHub web editor, or edit this file locally and push.</li>
            <li>Update the <code>Projects</code> links, fill in Publications, and add a <code>cv.pdf</code> to this repo root.</li>
            <li>Optional: create <code>favicon.ico</code> and place in the repo root.</li>
          </ol>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="wrap">
      <div class="two-col">
        <div>© <span id="year"></span> Hisay Lama. Built with vanilla HTML/CSS and hosted on GitHub Pages.</div>
        <div style="text-align:right">Theme toggle • <a href="https://github.com/hisaylama/hisaylama.github.io">View source</a></div>
      </div>
    </div>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>

  <!--
  Quick edit tips
  1) Replace text content above with your latest roles / projects.
  2) Add new project cards by duplicating an <article class="card"> in #projects.
  3) To add analytics later, paste your script before </body>.
  4) Want a blog? Add a /blog/ folder and separate HTML files, or switch to Jekyll.
  -->
</body>
</html>
