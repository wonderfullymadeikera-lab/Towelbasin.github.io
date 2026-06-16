# Towelbasin.github.io
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>The Towel and Basin Society</title>
  <meta name="description" content="The Towel and Basin Society is where servanthood meets real talk, deep revelation, and a whole lot of laughter. Hosted by Ikera Jones and Rj Schumeier." />
  <style>
    :root{
      --bg:#050505;
      --panel:#111111;
      --panel-2:#161616;
      --text:#f5f5f5;
      --muted:#b7b7b7;
      --gold:#d4af37;
      --gold-2:#f2d66b;
      --border:rgba(212,175,55,.22);
      --shadow:0 24px 70px rgba(0,0,0,.45);
    }

    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family:Inter,system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
      color:var(--text);
      background:
        radial-gradient(circle at top, rgba(212,175,55,.16), transparent 28%),
        radial-gradient(circle at 80% 18%, rgba(242,214,107,.10), transparent 18%),
        linear-gradient(180deg, #0b0b0b 0%, #050505 100%);
    }

    a{color:inherit;text-decoration:none}
    .wrap{width:min(1120px, calc(100% - 32px)); margin:0 auto}

    header{
      position:sticky; top:0; z-index:20;
      background:rgba(5,5,5,.72);
      backdrop-filter:blur(14px);
      border-bottom:1px solid var(--border);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between; gap:20px;
      padding:16px 0;
    }
    .brand{
      display:flex; align-items:center; gap:12px;
      font-weight:800; letter-spacing:.02em;
    }
    .mark{
      width:44px; height:44px; border-radius:16px;
      display:grid; place-items:center;
      background:linear-gradient(135deg, var(--gold), var(--gold-2));
      color:#111; font-weight:900;
      box-shadow:var(--shadow);
    }
    .navlinks{
      display:flex; gap:18px; flex-wrap:wrap;
      color:var(--muted); font-weight:500; font-size:.95rem;
    }
    .navlinks a:hover{color:var(--gold-2)}

    .hero{padding:88px 0 58px}
    .hero-grid{
      display:grid; grid-template-columns:1.2fr .8fr; gap:28px; align-items:center;
    }
    .eyebrow{
      display:inline-flex; align-items:center; gap:8px;
      padding:8px 12px; border-radius:999px;
      background:rgba(255,255,255,.04);
      border:1px solid var(--border);
      color:var(--gold-2); font-size:.92rem;
    }
    h1{
      margin:18px 0 16px;
      font-size:clamp(3rem, 7vw, 5.8rem);
      line-height:.94;
      letter-spacing:-.06em;
      max-width:11ch;
    }
    .lede{
      margin:0;
      max-width:62ch;
      font-size:1.1rem;
      line-height:1.75;
      color:#d5d5d5;
    }
    .cta{display:flex; gap:14px; flex-wrap:wrap; margin-top:28px}
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      padding:14px 18px; border-radius:14px;
      border:1px solid var(--border);
      background:rgba(255,255,255,.04);
      font-weight:700;
    }
    .btn.primary{
      background:linear-gradient(135deg, var(--gold), var(--gold-2));
      color:#111;
      border:none;
    }

    .card{
      background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03));
      border:1px solid var(--border);
      border-radius:24px;
      box-shadow:var(--shadow);
    }
    .player{padding:22px}
    .art{
      aspect-ratio:1;
      border-radius:20px;
      background:
        radial-gradient(circle at 30% 30%, rgba(255,255,255,.22), transparent 18%),
        linear-gradient(135deg, #111 0%, #222 35%, #d4af37 100%);
      display:grid; place-items:center;
      color:#111; text-align:center;
      font-size:2rem; font-weight:900;
      padding:20px;
    }
    .art span{
      background:rgba(255,255,255,.85);
      padding:12px 16px;
      border-radius:14px;
    }
    .player-meta{
      display:flex; justify-content:space-between; gap:16px; flex-wrap:wrap;
      margin-top:16px; color:var(--muted); font-size:.95rem;
    }

    .section{padding:24px 0 8px}
    .section h2{
      margin:0 0 10px;
      font-size:2rem;
      letter-spacing:-.03em;
    }
    .section .head{
      margin:0 0 22px;
      max-width:70ch;
      color:var(--muted);
      line-height:1.7;
    }
    .grid3{
      display:grid; grid-template-columns:repeat(3, 1fr); gap:18px;
    }
    .panel{
      padding:22px;
      border-radius:22px;
      background:rgba(255,255,255,.03);
      border:1px solid var(--border);
    }
    .panel h3{margin:0 0 8px; font-size:1.05rem}
    .panel p{margin:0; color:var(--muted); line-height:1.7}

    .episodes{display:grid; gap:14px}
    .ep{
      display:grid; grid-template-columns:auto 1fr auto; gap:18px; align-items:center;
      padding:18px 20px;
      border-radius:18px;
      background:rgba(255,255,255,.03);
      border:1px solid var(--border);
    }
    .num{
      width:48px; height:48px; border-radius:14px;
      display:grid; place-items:center;
      background:rgba(212,175,55,.12);
      color:var(--gold-2); font-weight:800;
    }
    .ep h4{margin:0 0 6px; font-size:1.03rem}
    .ep .sub{color:var(--muted); font-size:.95rem; line-height:1.6}
    .links{display:flex; gap:10px; flex-wrap:wrap}
    .pill{
      padding:10px 14px;
      border-radius:999px;
      background:rgba(255,255,255,.05);
      border:1px solid var(--border);
      font-size:.95rem;
    }
    .pill:hover{border-color:rgba(242,214,107,.55); color:var(--gold-2)}

    footer{
      padding:34px 0 50px;
      color:var(--muted);
    }
    .footer{
      display:flex; justify-content:space-between; gap:16px; flex-wrap:wrap;
      border-top:1px solid var(--border); padding-top:22px;
    }

    @media (max-width: 900px){
      .hero-grid,.grid3{grid-template-columns:1fr}
      h1{max-width:none}
      .ep{grid-template-columns:auto 1fr}
      .ep .links{grid-column:1 / -1}
    }
  </style>
</head>
<body>
  <header>
    <div class="wrap nav">
      <div class="brand">
        <div class="mark">TB</div>
        <div>The Towel and Basin Society</div>
      </div>
      <nav class="navlinks">
        <a href="#about">About</a>
        <a href="#hosts">Hosts</a>
        <a href="#episodes">Episodes</a>
        <a href="#subscribe">Subscribe</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="wrap hero-grid">
        <div>
          <div class="eyebrow">New episodes • Hosted by Ikera + Rj</div>
          <h1>Servanthood, real talk, and a whole lot of laughter.</h1>
          <p class="lede">
            The Towel and Basin Society is where Kingdom servanthood meets honest conversation,
            deep revelation, and a warm listening experience.
          </p>
          <div class="cta">
            <a class="btn primary" href="https://open.spotify.com/show/7xmf9UbAWh1cNJNYcG7eBg?si=BNz28SUDRbGMeyMwM8FRKA" target="_blank" rel="noopener">Listen on Spotify</a>
            <a class="btn" href="#episodes">Latest Episodes</a>
          </div>
        </div>

        <div class="card player">
          <div class="art"><span>Towel &amp; Basin</span></div>
          <div class="player-meta">
            <span>Season 1</span>
            <span>Weekly Release</span>
            <span>45–60 min</span>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="about">
      <div class="wrap">
        <h2>About the show</h2>
        <p class="head">
          This podcast dives into the heart of Kingdom servanthood with honesty and purpose.
          Each episode blends reflection, practical insight, and meaningful conversation in a way
          that feels both grounded and engaging.
        </p>
        <div class="grid3">
          <div class="panel"><h3>Real conversations</h3><p>Open, thoughtful dialogue that feels natural and easy to follow.</p></div>
          <div class="panel"><h3>Faith-centered</h3><p>Built around servanthood, growth, and the everyday impact of Kingdom living.</p></div>
          <div class="panel"><h3>Listener-friendly</h3><p>Designed to help new listeners jump in quickly and keep coming back.</p></div>
        </div>
      </div>
    </section>

    <section class="section" id="hosts">
      <div class="wrap">
        <h2>Meet the hosts</h2>
        <p class="head">
          Ikera Jones and Rj Schumeier host the show with chemistry, clarity, and a style that
          makes deep topics feel personal and accessible.
        </p>
        <div class="grid3">
          <div class="panel"><h3>Ikera</h3><p>A warm, reflective voice that helps guide the conversation with focus and care.</p></div>
          <div class="panel"><h3>Rj</h3><p>A grounded co-host with energy, insight, and a strong sense of connection.</p></div>
          <div class="panel"><h3>Together</h3><p>Their back-and-forth creates a show that feels lively, meaningful, and memorable.</p></div>
        </div>
      </div>
    </section>

    <section class="section" id="episodes">
      <div class="wrap">
        <h2>Featured episodes</h2>
        <p class="head">Replace these placeholders with your real episode titles and links.</p>
        <div class="episodes">
          <article class="ep">
            <div class="num">01</div>
            <div>
              <h4>Why We Started Towel and Basin Society</h4>
              <div class="sub">An introduction to the vision, the voice, and the heart behind the podcast.</div>
            </div>
            <div class="links">
              <a class="pill" href="https://open.spotify.com/show/7xmf9UbAWh1cNJNYcG7eBg?si=BNz28SUDRbGMeyMwM8FRKA" target="_blank" rel="noopener">Spotify</a>
              <a class="pill" href="https://podcasts.apple.com/us/podcast/the-towel-and-basin-society/id1866085821" target="_blank" rel="noopener">Apple</a>
            </div>
          </article>
          <article class="ep">
            <div class="num">02</div>
            <div>
              <h4>What Servanthood Looks Like in Real Life</h4>
              <div class="sub">A conversation about humility, consistency, and practical Kingdom living.</div>
            </div>
            <div class="links">
              <a class="pill" href="https://youtube.com/@towelandbasinsociety?si=OHaYmyhjL6ym1dzW" target="_blank" rel="noopener">YouTube</a>
              <a class="pill" href="https://anchor.fm/s/fa006f54/podcast/rss" target="_blank" rel="noopener">RSS</a>
            </div>
          </article>
          <article class="ep">
            <div class="num">03</div>
            <div>
              <h4>Faith, Growth, and the Table We Share</h4>
              <div class="sub">Stories, lessons, and the moments that help shape a stronger community.</div>
            </div>
            <div class="links">
              <span class="pill">Clip</span>
              <span class="pill">New</span>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section class="section" id="subscribe">
      <div class="wrap">
        <h2>Subscribe</h2>
        <p class="head">Quick links to your podcast platforms.</p>
        <div class="links">
          <a class="pill" href="https://open.spotify.com/show/7xmf9UbAWh1cNJNYcG7eBg?si=BNz28SUDRbGMeyMwM8FRKA" target="_blank" rel="noopener">Spotify</a>
          <a class="pill" href="https://podcasts.apple.com/us/podcast/the-towel-and-basin-society/id1866085821" target="_blank" rel="noopener">Apple Podcasts</a>
          <a class="pill" href="https://youtube.com/@towelandbasinsociety?si=OHaYmyhjL6ym1dzW" target="_blank" rel="noopener">YouTube</a>
          <a class="pill" href="https://anchor.fm/s/fa006f54/podcast/rss" target="_blank" rel="noopener">RSS Feed</a>
        </div>
      </div>
    </section>

    <section class="section" id="contact">
      <div class="wrap">
        <h2>Contact</h2>
        <p class="head">
          For bookings, guest ideas, or partnerships, use <strong>hello@towelandbasin.com</strong>.
        </p>
      </div>
    </section>
  </main>

  <footer>
    <div class="wrap footer">
      <div>© 2026 The Towel and Basin Society</div>
      <div>Hosted by Ikera Jones and Rj Schumeier</div>
    </div>
  </footer>
</body>
</html>
