<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ukasha FX Academy — Learn Forex Trading</title>

  <!-- ====== Basic security/meta (useful — but real headers should be set on your hosting/server) ====== -->
  <!-- Content-Security-Policy: restrict sources (adjust if you add external resources) -->
  <meta http-equiv="Content-Security-Policy"
        content="default-src 'self'; img-src 'self' data: https:; script-src 'self' 'unsafe-inline'; style-src 'self' 'unsafe-inline' https://fonts.googleapis.com; font-src https://fonts.gstatic.com; connect-src 'self' https:;">
  <meta http-equiv="X-Frame-Options" content="DENY">
  <meta http-equiv="X-Content-Type-Options" content="nosniff">
  <meta name="referrer" content="no-referrer-when-downgrade">

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#071025;
      --card:#0b1220;
      --muted:#94a3b8;
      --accent:#06b6d4;
      --accent-2:#7c3aed;
      --accent-3:#16a34a; /* green accent for finance */
      --radius:14px;
      --maxw:1100px;
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif;
      color-scheme:dark;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      background:linear-gradient(180deg,var(--bg) 0%, #071022 100%);
      color:#e6eef5;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
    }
    a{color:inherit;text-decoration:none}
    .container{max-width:var(--maxw);margin:0 auto;padding:28px}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:12px 0}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:52px;height:52px;border-radius:12px;background:linear-gradient(135deg,var(--accent),var(--accent-2));display:grid;place-items:center;font-weight:900;color:#021017}
    .site-title{font-weight:800}
    .nav-links{display:flex;gap:14px;align-items:center}
    .nav-links a{padding:8px 12px;border-radius:10px;font-weight:600}
    .btn{background:linear-gradient(90deg,var(--accent),var(--accent-2));padding:10px 16px;border-radius:12px;font-weight:700;color:#021017;border:none;cursor:pointer}
    .menu-toggle{display:none;padding:8px;border-radius:8px;background:rgba(255,255,255,0.03);cursor:pointer}

    /* HERO */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:36px;align-items:center;padding:36px 0}
    .hero h1{font-size:32px;margin:0 0 12px}
    .hero p{color:var(--muted);margin:0 0 18px}
    .hero .kicker{display:inline-block;background:rgba(255,255,255,0.03);padding:6px 10px;border-radius:999px;font-weight:700;margin-bottom:12px}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:var(--radius);box-shadow:0 6px 18px rgba(2,6,23,0.6)}

    /* FEATURES */
    .features{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:18px}
    .feature{padding:18px;border-radius:12px;background:var(--card);transition:0.28s;overflow:hidden}
    .feature:hover{transform:translateY(-6px);box-shadow:0 18px 30px rgba(0,0,0,0.5)}
    .feature img{display:block;margin-bottom:10px}

    /* CONTACT */
    #contact{margin-top:28px}
    input[type="email"]{width:100%;padding:10px;border-radius:10px;border:0;background:rgba(255,255,255,0.02);color:inherit}
    .social-row{display:flex;gap:10px;align-items:center;margin-top:12px}

    footer{padding:28px 0;color:var(--muted);border-top:1px solid rgba(255,255,255,0.03);margin-top:28px}
    .footer-socials{display:flex;gap:12px;align-items:center}

    /* small helpers */
    .muted{color:var(--muted)}
    .badge{background:rgba(255,255,255,0.03);padding:6px 10px;border-radius:999px;font-weight:700;display:inline-block}

    /* Animations & hover */
    .btn{transition:0.22s}
    .btn:hover{transform:scale(1.04);box-shadow:0 8px 20px rgba(6,182,212,0.12)}
    .nav-links a{transition:0.18s}
    .nav-links a:hover{color:var(--accent)}
    .hero img{opacity:0;animation:fadeIn 1s forwards}
    @keyframes fadeIn{to{opacity:1}}

    /* Responsive */
    @media(max-width:900px){
      .hero{grid-template-columns:1fr}
      .features{grid-template-columns:repeat(2,1fr)}
    }
    @media(max-width:640px){
      .container{padding:18px}
      .nav-links{display:none}
      .menu-toggle{display:block}
      .features{grid-template-columns:1fr}
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- NAVBAR -->
    <header class="nav" role="banner">
      <div class="brand" aria-label="Ukasha FX Academy">
        <div class="logo">UK</div>
        <div>
          <div class="site-title">Ukasha FX Academy</div>
          <div class="muted" style="font-size:12px">Learn Forex — From Beginner to Pro</div>
        </div>
      </div>

      <nav class="nav-links" role="navigation" aria-label="Main menu">
        <a href="#home">Home</a>
        <a href="#features">What you will learn</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
        <a class="btn" href="#features">Start Learning</a>
      </nav>

      <button class="menu-toggle" aria-label="Open menu" onclick="toggleMenu()">☰</button>
    </header>

    <!-- HERO -->
    <main id="home" class="hero" role="main">
      <section>
        <div class="kicker">Forex Education • Live Reviews • Mentorship</div>
        <h1>Welcome to Ukasha FX Academy</h1>
        <p>Ukasha FX Academy focuses on teaching beginners and intermediate traders practical, hands-on Forex skills: price-action trading, risk management, chart analysis, and trading psychology. Step-by-step lessons, real market examples, and mentorship to help you become consistently profitable.</p>

        <div style="display:flex;gap:12px;margin-top:18px;flex-wrap:wrap">
          <a class="btn" href="#features">Start Learning</a>
          <a style="padding:10px 14px;border-radius:12px;background:transparent;border:1px solid rgba(255,255,255,0.06);font-weight:700" href="#contact">Contact</a>
        </div>

        <div style="margin-top:18px;color:var(--muted);font-size:14px">
          <strong>Tip:</strong> Join our Telegram channel for live market reviews and signals.
        </div>
      </section>

      <aside>
        <div class="card" aria-hidden="false">
          <img src="images/forex-hero.jpg" alt="Forex charts and trading desk" style="width:100%;border-radius:12px">
          <div style="margin-top:12px">
            <div style="font-weight:800">Ukasha</div>
            <div class="muted" style="font-size:13px">Professional Forex trader & instructor — 3+ years experience</div>
          </div>
        </div>
      </aside>
    </main>

    <!-- FEATURES (What you will learn) -->
    <section id="features" aria-labelledby="features-heading">
      <h2 id="features-heading">What You Will Learn</h2>
      <p class="muted">Topics are designed from beginner → advanced, with live examples and strategy building.</p>

      <div class="features" role="list">
        <div class="feature" role="listitem">
          <img src="images/strategy.png" alt="Strategy icon" width="56">
          <h4>Trading Strategies</h4>
          <p class="muted">Proven price-action and breakout strategies you can apply immediately.</p>
        </div>

        <div class="feature" role="listitem">
          <img src="images/chart.png" alt="Chart icon" width="56">
          <h4>Chart Analysis</h4>
          <p class="muted">Candlestick patterns, indicators, support/resistance and confluence.</p>
        </div>

        <div class="feature" role="listitem">
          <img src="images/risk.png" alt="Risk icon" width="56">
          <h4>Risk Management</h4>
          <p class="muted">Position sizing, R:R, drawdown control and protecting your capital.</p>
        </div>

        <div class="feature" role="listitem">
          <img src="images/psychology.png" alt="Psychology" width="56">
          <h4>Trading Psychology</h4>
          <p class="muted">Discipline, journaling, emotion control and routine building.</p>
        </div>

        <div class="feature" role="listitem">
          <img src="images/live.png" alt="Live reviews" width="56">
          <h4>Live Market Reviews</h4>
          <p class="muted">Regular live sessions analysing real market opportunities.</p>
        </div>

        <div class="feature" role="listitem">
          <img src="images/backtest.png" alt="Backtest" width="56">
          <h4>Strategy Building & Backtesting</h4>
          <p class="muted">How to build, test and improve your strategies for consistent results.</p>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about" style="margin-top:22px">
      <h2>About Ukasha</h2>
      <p class="muted">Ukasha is a professional Forex trader and instructor with 3+ years trading experience across major currency pairs. He specializes in price-action strategies, risk control, and practical methods that beginners can apply immediately. Ukasha runs live trading sessions, free lessons, and paid courses for serious students.</p>
    </section>

    <!-- CONTACT -->
    <section id="contact" style="margin-top:22px">
      <h2>Stay Updated & Contact</h2>
      <p class="muted">Subscribe or contact me directly at <strong>hubf2029@gmail.com</strong> for latest Forex tips, strategies, and webinars.</p>

      <div style="max-width:480px">
        <input type="email" value="hubf2029@gmail.com" readonly aria-label="Email">
        <a href="mailto:hubf2029@gmail.com"><button class="btn" style="width:100%">Send Email</button></a>

        <div class="social-row" aria-label="Social links">
          <!-- Social icons (simple SVGs) -->
          <a href="https://www.facebook.com/profile.php?id=61584080877781" target="_blank" rel="noopener noreferrer" aria-label="Facebook">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="6" fill="rgba(255,255,255,0.03)"/><path d="M15 8h-2c-.6 0-1 .4-1 1v2h3l-.5 3H12v7H9v-7H7v-3h2V9a4 4 0 014-4h2v3z" fill="#3b82f6"/></svg>
          </a>

          <a href="https://www.instagram.com/forexhub23?igsh=NTc4MTIwNjQ2YQ==" target="_blank" rel="noopener noreferrer" aria-label="Instagram">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="6" fill="rgba(255,255,255,0.03)"/><path d="M7 2h10a5 5 0 015 5v10a5 5 0 01-5 5H7a5 5 0 01-5-5V7a5 5 0 015-5zm5 6.2A4.8 4.8 0 1016.8 13 4.8 4.8 0 0012 8.2zm6.4-3.6a1.12 1.12 0 110 2.24 1.12 1.12 0 010-2.24z" fill="#e95950"/></svg>
          </a>

          <a href="https://www.tiktok.com/@forex.hub6?_r=1&_t=ZS-91YUecKVlyx" target="_blank" rel="noopener noreferrer" aria-label="TikTok">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="6" fill="rgba(255,255,255,0.03)"/><path d="M17 6.5a4 4 0 01-2.5-.9v6.4A4.6 4.6 0 0110 16 4.5 4.5 0 118.5 6v.7a6.2 6.2 0 005 6.1V8a6 6 0 004.5-1.6z" fill="#00f2ea"/></svg>
          </a>

          <a href="https://youtube.com/@ukashamuhammadsaraki?si=EypqPcdInmEziIrG" target="_blank" rel="noopener noreferrer" aria-label="YouTube">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="6" fill="rgba(255,255,255,0.03)"/><path d="M10 8l6 4-6 4V8z" fill="#FF0000"/></svg>
          </a>

          <a href="https://t.me/Uk45h4" target="_blank" rel="noopener noreferrer" aria-label="Telegram">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="6" fill="rgba(255,255,255,0.03)"/><path d="M4 12l15-6-6 10-3-2-6 2z" fill="#2AABEE"/></svg>
          </a>

          <a href="https://x.com/saraki50028?t=t1_CKIZ3k1e2rzy1dJBuiA&s=09" target="_blank" rel="noopener noreferrer" aria-label="X">
            <svg width="34" height="34" viewBox="0 0 24 24" fill="none" aria-hidden="true"><rect width="24" height="24" rx="6" fill="rgba(255,255,255,0.03)"/><path d="M7 8l5 5 5-5" stroke="#1D9BF0" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg>
          </a>
        </div>
      </div>
    </section>

    <!-- FOOTER -->
    <footer>
      <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:12px">
        <div>
          <div style="font-weight:700">Ukasha FX Academy</div>
          <div class="muted" style="font-size:13px">© Ukasha • 2025</div>
        </div>

        <div class="footer-socials" aria-hidden="false">
          <!-- repeat small icons -->
          <a href="https://www.facebook.com/profile.php?id=61584080877781" target="_blank" rel="noopener noreferrer" aria-label="Facebook small">FB</a>
          <a href="https://www.instagram.com/forexhub23?igsh=NTc4MTIwNjQ2YQ==" target="_blank" rel="noopener noreferrer" aria-label="Instagram small">IG</a>
          <a href="https://www.tiktok.com/@forex.hub6?_r=1&_t=ZS-91YUecKVlyx" target="_blank" rel="noopener noreferrer" aria-label="TikTok small">TT</a>
          <a href="https://youtube.com/@ukashamuhammadsaraki?si=EypqPcdInmEziIrG" target="_blank" rel="noopener noreferrer" aria-label="YouTube small">YT</a>
          <a href="https://t.me/Uk45h4" target="_blank" rel="noopener noreferrer" aria-label="Telegram small">TG</a>
          <a href="https://x.com/saraki50028?t=t1_CKIZ3k1e2rzy1dJBuiA&s=09" target="_blank" rel="noopener noreferrer" aria-label="X small">X</a>
        </div>
      </div>
    </footer>
  </div>

  <script>
    // Mobile menu toggle
    function toggleMenu(){
      const nav = document.querySelector('.nav-links');
      if(!nav) return;
      if(nav.style.display === 'flex'){ nav.style.display = 'none'; }
      else {
        nav.style.display = 'flex';
        nav.style.flexDirection = 'column';
        nav.style.position = 'absolute';
        nav.style.right = '20px';
        nav.style.top = '66px';
        nav.style.background = 'linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01))';
        nav.style.padding = '12px';
        nav.style.borderRadius = '12px';
      }
    }

    // Accessibility: allow Enter to open mailto from keyboard when focused
    document.addEventListener('keydown', function(e){
      if(e.key === 'Enter'){
        const active = document.activeElement;
        if(active && active.getAttribute('href') && active.getAttribute('href').startsWith('mailto:')){
          window.location = active.getAttribute('href');
        }
      }
    });

    // Basic client-side form sanity (no backend yet)
    // Prevent accidental editing of the displayed email
    const emailInput = document.querySelector('input[type="email"]');
    if(emailInput) emailInput.addEventListener('focus', () => emailInput.blur());
  </script>
</body>
</html>
