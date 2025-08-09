<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Élec-Express — Dépannage Électrique</title>
  <meta name="description" content="Électricien — Intervention d'urgence, remise aux normes, dépannage"/>
  <style>
    :root{--bg:#071026;--card:#0f1724;--accent:#ff9b21;--muted:#bcd0e6;--danger:#ff3b30;--glass:rgba(255,255,255,0.03);--radius:14px;font-family:system-ui,-apple-system,'Segoe UI',Roboto,Arial}
    *{box-sizing:border-box}
    body{margin:0;min-height:100vh;background:linear-gradient(180deg,#071026 0%,#08162a 100%);color:#eaf2ff}
    .wrap{max-width:1000px;margin:28px auto;padding:20px}
    header{display:flex;justify-content:space-between;align-items:center}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:56px;height:56px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#ff6b3a);display:flex;align-items:center;justify-content:center;font-weight:800;color:#081018}
    nav a{color:var(--muted);text-decoration:none;margin-left:14px;font-weight:600}

    .hero{display:grid;grid-template-columns:1fr 420px;gap:20px;margin-top:20px;align-items:stretch}
    .card{background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);padding:22px;border-radius:var(--radius);box-shadow:0 10px 30px rgba(2,6,23,0.6)}
    h1{margin:4px 0 8px;font-size:28px}
    p.lead{color:var(--muted);line-height:1.5}
    .btn{display:inline-block;margin-top:12px;padding:11px 16px;border-radius:12px;background:linear-gradient(90deg,var(--accent),#ff6b3a);color:#081018;font-weight:700;text-decoration:none}

    /* visual */
    .visual{border-radius:12px;overflow:hidden;background:linear-gradient(180deg,#051224,#062034);display:flex;align-items:center;justify-content:center;padding:18px}
    svg{max-width:100%;height:auto}

    /* services */
    .services{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:14px;margin-top:18px}
    .serv{background:var(--glass);padding:14px;border-radius:12px}
    .serv h3{margin:6px 0}

    footer{margin-top:18px;display:flex;gap:16px;flex-wrap:wrap;align-items:flex-start}
    .contact{min-width:260px;max-width:420px}
    .form{display:flex;flex-direction:column;gap:8px}
    input,textarea{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px;border-radius:8px;color:var(--muted)}
    .note{font-size:13px;color:var(--muted)}

    .small{font-size:13px;color:rgba(255,255,255,0.6)}

    @media (max-width:980px){.hero{grid-template-columns:1fr;}.visual{order:2}}
    @media (max-width:560px){.wrap{padding:12px}.logo{width:48px;height:48px}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">EL</div>
        <div>
          <div style="font-weight:800">Élec-Express</div>
          <div class="small">Dépannage • Urgence • Mise aux normes</div>
        </div>
      </div>
      <nav>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
        <a href="tel:+33123456789">📞 06 12 34 56 78</a>
      </nav>
    </header>

    <main class="hero">
      <section class="card">
        <span style="display:inline-block;padding:6px 10px;background:rgba(255,91,91,0.12);border-radius:999px;color:var(--danger);font-weight:700;font-size:13px">Intervention 24/7</span>
        <h1>Électricien — Sécurité & Urgence</h1>
        <p class="lead">Intervention rapide en cas de court-circuit, fumée suspecte ou panne électrique. Remise aux normes, diagnostic et sécurisation de l'installation.</p>
        <a class="btn" href="#contact">Demander une intervention</a>

        <div style="margin-top:18px;display:flex;gap:12px;align-items:center">
          <div style="flex:1">
            <div style="font-weight:700">Interventions rapides</div>
            <div class="note">Déplacement dans la région — délai moyen : 30 min</div>
          </div>
          <div style="width:120px;text-align:center;background:rgba(255,255,255,0.02);padding:10px;border-radius:10px">✅ Assurance Pro</div>
        </div>
      </section>

      <aside class="visual card" aria-hidden="true">
        <!-- SVG illustratif simple : maison + flammes (décoratif) -->
        <svg viewBox="0 0 420 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Illustration appartement en feu (décoratif)">
          <defs>
            <linearGradient id="bg" x1="0" x2="1"><stop offset="0%" stop-color="#051224"/><stop offset="100%" stop-color="#062034"/></linearGradient>
          </defs>
          <rect width="100%" height="100%" fill="url(#bg)" rx="8"/>
          <g transform="translate(50,60)">
            <polygon points="50,0 0,40 0,140 120,140 120,40" fill="#0f2b3b" stroke="#184e5a"/>
            <rect x="16" y="70" width="30" height="46" fill="#07121a"/>
            <rect x="76" y="90" width="20" height="28" fill="#0b2730"/>
            <polygon points="-20,40 60,-36 140,40" fill="#102633"/>
            <!-- flammes décoratives -->
            <g transform="translate(70,140)">
              <path d="M0 40 C -12 10, 12 6, 0 -30 C 18 -8, 12 8, 0 40" fill="#ffb86b" opacity="0.9"/>
              <path d="M0 30 C -8 6, 8 2, 0 -20 C 12 -6, 8 6, 0 30" fill="#ff6b3a"/>
              <path d="M0 18 C -4 4, 4 0, 0 -10 C 8 -4, 6 4, 0 18" fill="#ff2e1e"/>
            </g>
          </g>
        </svg>
      </aside>
    </main>

    <section id="services" class="services">
      <div class="serv"><strong>Dépannage & Urgence</strong><h3>Courts-circuits & fumées</h3><p class="note">Coupe d'alimentation, sécurisation, coordination pompiers si besoin.</p></div>
      <div class="serv"><strong>Remise aux normes</strong><h3>Tableau électrique & mise à la terre</h3><p class="note">Rapport et devis clair — solutions conformes.</p></div>
      <div class="serv"><strong>Contrats</strong><h3>Maintenance préventive</h3><p class="note">Contrats de suivi pour réduire les risques et incidents.</p></div>
    </section>

    <footer id="contact">
      <div class="card contact">
        <div style="font-weight:700">Contact & Devis</div>
        <div class="note">Remplis le formulaire ci-dessous — le bouton ouvrira ton client mail (fonctionne sur GitHub Pages).</div>

        <form id="contactForm" class="form" onsubmit="return false;">
          <input id="name" name="name" placeholder="Votre nom" required />
          <input id="phone" name="phone" placeholder="Téléphone" required />
          <textarea id="message" name="message" rows="3" placeholder="Décris le problème (ex : fumée salon...)" required></textarea>
          <div style="display:flex;gap:8px;align-items:center">
            <button id="sendBtn" class="btn" type="submit">Envoyer la demande</button>
            <a class="small" href="tel:+33123456789">Appeler : 06 12 34 56 78</a>
          </div>
          <div id="status" class="small" style="margin-top:8px;color:rgba(255,255,255,0.7)"></div>
        </form>
      </div>

      <div style="flex:1;min-width:220px;align-self:flex-start">
        <div class="card">
          <strong>Conseils sécurité</strong>
          <ul class="note">
            <li>Coupe le courant si tu sens une odeur de brûlé.</li>
            <li>Éloigne les personnes et appelle les secours si nécessaire.</li>
            <li>Ne touche pas un appareil en feu — attends les secours.</li>
          </ul>
        </div>
      </div>
    </footer>

    <div style="text-align:center;color:rgba(255,255,255,0.12);font-size:12px;margin-top:12px">© Élec-Express — Démo statique (index.html)</div>
  </div>

  <script>
    // Form submit handler: ouvre le client mail via mailto: (fonctionne sans serveur)
    document.getElementById('contactForm').addEventListener('submit', function(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const phone = document.getElementById('phone').value.trim();
      const msg = document.getElementById('message').value.trim();
      if(!name || !phone || !msg){ document.getElementById('status').textContent = 'Merci de remplir tous les champs.'; return; }

      const to = 'contact@exemple.com'; // <-- change ici vers ton adresse
      const subject = encodeURIComponent('Demande intervention - ' + name);
      const body = encodeURIComponent('Nom: ' + name + '
Téléphone: ' + phone + '

Message:
' + msg);
      // Ouvre le client mail
      window.location.href = `mailto:${to}?subject=${subject}&body=${body}`;
      document.getElementById('status').textContent = 'Ton client mail va s'ouvrir pour envoyer la demande. Si rien ne se passe, copie les informations et envoie-les manuellement.';
    });

    // Pour permettre l'envoi depuis le bouton (sans appuyer sur Enter)
    document.getElementById('sendBtn').addEventListener('click', function(){ document.getElementById('contactForm').dispatchEvent(new Event('submit')); });
  </script>
</body>
</html>
