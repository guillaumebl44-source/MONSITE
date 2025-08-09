<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Électricien - Urgence & Sécurité</title>
  <meta name="description" content="Électricien professionnel — interventions d'urgence, diagnostics, mise aux normes."
  />
  <style>
    :root{
      --bg:#0b1020; --card:#0f1724; --accent:#ff9b21; --danger:#ff3b30; --muted:#cbd5e1;
      --glass: rgba(255,255,255,0.04);
      --radius:18px;
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;background:linear-gradient(180deg,#071022 0%,#061225 60%);color:#e6eef8}

    /* layout */
    .container{max-width:1100px;margin:0 auto;padding:28px}
    header{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .logo{display:flex;align-items:center;gap:12px}
    .logo .mark{width:54px;height:54px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#ff5e5e);display:flex;align-items:center;justify-content:center;font-weight:700}
    nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:stretch;margin-top:28px}
    .hero-card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:28px;border-radius:var(--radius);box-shadow:0 8px 30px rgba(2,6,23,0.6);min-height:420px;position:relative;overflow:hidden}
    .hero h1{font-size:32px;margin:0 0 10px}
    .hero p{color:var(--muted);line-height:1.45}
    .cta{display:inline-block;margin-top:16px;padding:12px 18px;border-radius:12px;background:linear-gradient(90deg,var(--accent),#ff6b3a);color:#08101a;font-weight:700;text-decoration:none}

    /* Right visual area */
    .scene{position:relative;height:100%;border-radius:12px;background:linear-gradient(180deg,#071226,#0b1422);overflow:hidden}
    /* simple house SVG container */
    .scene svg{width:100%;height:100%;display:block}

    /* flames */
    .flame{transform-origin:center bottom;filter:drop-shadow(0 8px 18px rgba(255,80,20,0.16))}
    .flame .f1{animation:flame 1.1s infinite ease-in-out}
    .flame .f2{animation:flame 1.25s infinite ease-in-out;opacity:0.9}
    @keyframes flame{0%{transform:translateY(6px) scaleY(.95)}50%{transform:translateY(0) scaleY(1.05)}100%{transform:translateY(6px) scaleY(.95)}}

    /* lightning */
    .bolt{position:absolute;left:18%;top:8%;width:64px;height:160px;opacity:0;pointer-events:none}
    .bolt path{stroke:#eaf6ff;stroke-width:6;stroke-linecap:round;stroke-linejoin:round}
    .bolt.animate{animation:flash 3.8s linear infinite}
    @keyframes flash{0%{opacity:0}6%{opacity:1}8%{opacity:0.9}10%{opacity:0}100%{opacity:0}}

    /* services & footer */
    .services{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px;margin-top:22px}
    .service{background:var(--glass);padding:16px;border-radius:12px}
    .service h3{margin:6px 0 0}
    footer{margin-top:26px;padding:18px;border-radius:12px;background:rgba(0,0,0,0.14);display:flex;justify-content:space-between;align-items:center}

    /* responsive */
    @media (max-width:980px){.hero{grid-template-columns:1fr;}.logo .mark{width:46px;height:46px}.bolt{left:65%}}
    @media (max-width:560px){.container{padding:18px}.hero-card{padding:18px}.hero h1{font-size:22px}}

    /* contact form small */
    .form{display:flex;flex-direction:column;gap:8px;margin-top:10px}
    .form input,.form textarea{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px;border-radius:8px;color:var(--muted)}
    .note{font-size:13px;color:rgba(255,255,255,0.65)}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo">
        <div class="mark">EL</div>
        <div>
          <div style="font-weight:700">Élec-Express</div>
          <div style="font-size:12px;color:var(--muted)">Urgence • Remise aux normes • Dépannage</div>
        </div>
      </div>
      <nav>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
        <a href="#tel">📞 06 12 34 56 78</a>
      </nav>
    </header>

    <main class="hero">
      <section class="hero-card">
        <span style="display:inline-block;padding:6px 10px;background:rgba(255,91,91,0.12);border-radius:999px;color:var(--danger);font-weight:700;font-size:13px">Intervention 24/7</span>
        <h1>Électricien — Sécurité & Urgence</h1>
        <p>Diagnostic rapide, remise aux normes et interventions d'urgence en cas d'incendie, court-circuit ou dégâts électriques. Notre équipe intervient sur place pour sécuriser le bâtiment et rétablir l'électricité en toute sécurité.</p>
        <a class="cta" href="#contact">Demander une intervention</a>

        <div style="position:absolute;right:22px;bottom:20px;text-align:right;color:var(--muted)">
          <div style="font-weight:700">Interventions rapides</div>
          <div class="note">Moyenne d'arrivée : 30 min dans la région</div>
        </div>

        <div style="position:absolute;left:-120px;bottom:-120px;width:340px;height:340px;background:radial-gradient(circle at 30% 30%, rgba(255,154,33,0.08), transparent 20%), radial-gradient(circle at 70% 60%, rgba(255,64,64,0.06), transparent 30%);transform:rotate(15deg);filter:blur(10px)"></div>
      </section>

      <aside class="scene" aria-hidden="true">
        <!-- Simple illustrative SVG: maison + flammes + petits éclairs -->
        <svg viewBox="0 0 600 420" preserveAspectRatio="xMidYMid meet" xmlns="http://www.w3.org/2000/svg">
          <defs>
            <linearGradient id="g1" x1="0" x2="1">
              <stop offset="0%" stop-color="#0a1a2b"/>
              <stop offset="100%" stop-color="#08203a"/>
            </linearGradient>
          </defs>
          <rect width="100%" height="100%" fill="url(#g1)" />

          <!-- maison -->
          <g transform="translate(120,120)">
            <polygon points="60,0 0,48 0,160 140,160 140,48" fill="#0f2b3b" stroke="#1f879e" stroke-width="2" rx="6"/>
            <rect x="18" y="68" width="36" height="56" fill="#071a23" stroke="#053041"/>
            <rect x="86" y="92" width="24" height="28" fill="#0b2730"/>
            <!-- toit -->
            <polygon points="-20,48 70,-28 160,48" fill="#102633" stroke="#1a3b4f"/>
          </g>

          <!-- flammes group -->
          <g class="flame" transform="translate(260,220)">
            <path class="f1" d="M0 40 C -10 10, 10 0, 0 -36 C 18 -10, 12 8, 0 40" fill="#ffb86b"/>
            <path class="f2" d="M0 30 C -6 6, 6 0, 0 -24 C 12 -8, 8 6, 0 30" fill="#ff6b3a"/>
            <path d="M0 16 C -3 4, 3 0, 0 -12 C 8 -5, 6 4, 0 16" fill="#ff2e1e"/>
          </g>

          <!-- petit éclair récurrent -->
          <g class="bolt" id="bolt1">
            <path d="M40 0 L18 48 L36 48 L12 120" fill="none"/>
          </g>
        </svg>
      </aside>
    </main>

    <section id="services" class="services">
      <div class="service">
        <strong>Dépannage & Urgence</strong>
        <h3>Courts-circuits & Incendies</h3>
        <p class="note">Sécurisation du site, coupure d'alimentation, intervention coordinateur pompier si nécessaire.</p>
      </div>
      <div class="service">
        <strong>Remise aux normes</strong>
        <h3>Tableau électrique, mise à la terre</h3>
        <p class="note">Diagnostic complet et rapport conforme RT 2012 / 2020 (selon besoin).</p>
      </div>
      <div class="service">
        <strong>Contrats & Maintenance</strong>
        <h3>Contrat de maintenance</h3>
        <p class="note">Visites régulières, vérifications des dispositifs différentiel et prévention.</p>
      </div>
    </section>

    <footer id="contact">
      <div>
        <div style="font-weight:700">Contact & Devis</div>
        <div class="note">Remplis le formulaire ou appelle directement pour une intervention urgente.</div>
      </div>
      <div style="min-width:260px;max-width:420px">
        <form class="form" action="/send_mail.php" method="post">
          <input name="name" placeholder="Votre nom" required />
          <input name="phone" placeholder="Téléphone" required />
          <textarea name="msg" rows="2" placeholder="Décris le problème (ex: fumée dans le salon...)" required></textarea>
          <button type="submit" class="cta" style="display:inline-block">Envoyer la demande</button>
        </form>
      </div>
    </footer>

    <div style="text-align:center;color:rgba(255,255,255,0.12);font-size:12px;margin-top:12px">© Élec-Express — Mise en page démo</div>
  </div>

  <script>
    // Simple JS pour déclencher l'animation d'éclair de façon aléatoire
    (function(){
      const bolt = document.getElementById('bolt1');
      function randInt(min,max){return Math.floor(Math.random()*(max-min+1))+min}
      function flash(){
        bolt.classList.add('animate');
        setTimeout(()=>bolt.classList.remove('animate'), 300);
        // prochain éclair aléatoire entre 2s et 7s
        setTimeout(flash, randInt(2000,7000));
      }
      setTimeout(flash, 1200);
    })();
  </script>
</body>
</html>
