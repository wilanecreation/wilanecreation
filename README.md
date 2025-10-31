<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Wilane Création — Formations</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
    :root{
      --accent:#ff7300;
      --dark:#111;
      --muted:rgba(255,255,255,0.8);
      --glass: rgba(255,255,255,0.08);
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:Poppins,system-ui,Arial;
      color:#fff;
      background:#000;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      overflow-x:hidden;
    }

    /* Animated gradient background (laser-like) */
    body::before{
      content:"";
      position:fixed; inset:0;
      background: linear-gradient(270deg,#ff6600,#ff3b00,#1a1a1a,#0b0b0b);
      background-size: 1200% 1200%;
      filter: blur(36px) saturate(120%);
      animation: bgMove 12s linear infinite;
      z-index:-2;
      opacity:0.95;
    }
    @keyframes bgMove{0%{background-position:0% 50%}50%{background-position:100% 50%}100%{background-position:0% 50%}}

    /* top navigation */
    .nav {
      position:fixed; top:12px; left:50%; transform:translateX(-50%);
      display:flex; gap:14px; z-index:40;
      background:linear-gradient(90deg, rgba(0,0,0,0.35), rgba(255,255,255,0.02));
      padding:8px 14px; border-radius:999px; backdrop-filter:blur(6px);
      box-shadow:0 8px 30px rgba(0,0,0,0.5);
    }
    .nav a{color:var(--muted); text-decoration:none; padding:8px 12px; border-radius:8px; font-weight:600}
    .nav a:hover{background:rgba(255,255,255,0.04); color:#fff}

    header{
      text-align:center; padding:80px 20px 40px; position:relative;
      margin-top:30px;
    }
    header img{
      width:120px; height:120px; border-radius:50%; object-fit:cover;
      border:3px solid rgba(255,255,255,0.9); box-shadow:0 10px 30px rgba(255,115,0,0.12);
      animation:float 4s ease-in-out infinite;
      background:#fff;
    }
    @keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-8px)}}

    header h1{margin:12px 0 6px; font-size:2.4rem; letter-spacing:1px}
    header p{margin:0;color:rgba(255,255,255,0.9)}

    main{max-width:1100px;margin:30px auto;padding:0 18px 80px}

    .section{
      margin-top:28px;
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      padding:18px;border-radius:14px; box-shadow:0 6px 20px rgba(0,0,0,0.5);
      backdrop-filter: blur(6px);
    }

    .courses{display:grid; grid-template-columns:repeat(auto-fit,minmax(280px,1fr)); gap:18px}
    .card{padding:14px;border-radius:12px;background:var(--glass); text-align:center}
    .card img{width:100%;height:180px;object-fit:cover;border-radius:8px;margin-bottom:12px}
    .card h3{margin:6px 0}
    .price{color:#cfefff;font-weight:700}

    form{display:block; margin-top:12px}
    input,select,textarea{width:100%;padding:10px;border-radius:8px;border:none;margin-bottom:10px;outline:none;background:rgba(255,255,255,0.04);color:#fff}
    .row{display:flex;gap:10px}
    .row .btn{flex:1}

    .btn{
      display:inline-block;padding:10px 14px;border-radius:10px;background:var(--dark);color:#fff;text-decoration:none;border:none;cursor:pointer;font-weight:700;
      box-shadow: 0 6px 18px rgba(0,0,0,0.4);
    }
    .btn.secondary{background:transparent;border:1px solid rgba(255,255,255,0.08)}
    .muted{color:rgba(255,255,255,0.8)}

    footer{color:rgba(255,255,255,0.7);text-align:center;padding:30px 10px;margin-top:30px}

    /* Responsive tweaks */
    @media(max-width:640px){
      header h1{font-size:1.6rem}
      .nav{left:12px; transform:none; top:12px}
      body{font-size:15px}
    }
  </style>
</head>
<body>

  <!-- NAV -->
  <nav class="nav" aria-label="Main navigation">
    <a href="#home">Accueil</a>
    <a href="#about">À propos</a>
    <a href="#formations">Formations</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- HEADER / BANNER -->
  <header id="home">
    <img src="logo-wilane.png" alt="Logo Wilane Création" />
    <h1>Wilane Création</h1>
    <p>Bienvenue — Formations professionnelles en informatique, infographie et voix-off</p>
  </header>

  <main>
    <!-- ABOUT -->
    <section id="about" class="section">
      <h2>À propos</h2>
      <p class="muted">Wilane Création est un centre de formation multimédia dédié à la montée en compétences : informatique (bureautique & maintenance), infographie (design, retouche) et voix-off (technique & production). Notre approche est pratique, accessible aux débutants et orientée vers l’emploi.</p>
      <p style="margin-top:8px">Email : <a href="mailto:wilanethiernoabdourahmane@gmail.com" class="muted">wilanethiernoabdourahmane@gmail.com</a> • WhatsApp : <span class="muted">+221 77 541 42 27</span>, <span class="muted">+221 78 502 31 82</span></p>
    </section>

    <!-- FORMATIONS -->
    <section id="formations" class="section" style="margin-top:20px">
      <h2>Formations</h2>
      <div class="courses">
        <!-- Informatique -->
        <div class="card">
          <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?auto=format&fit=crop&w=900&q=80" alt="Informatique">
          <h3>Informatique — Bureautique & Maintenance</h3>
          <p class="muted">Word, Excel, PowerPoint, Internet et maintenance de base.</p>
          <p class="price">20 000 XOF</p>
        </div>

        <!-- Infographie -->
        <div class="card">
          <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=900&q=80" alt="Infographie">
          <h3>Infographie — Photoshop & Illustrator</h3>
          <p class="muted">Design visuel, logos, affiches et supports marketing.</p>
          <p class="price">30 000 XOF</p>
        </div>

        <!-- Voix Off -->
        <div class="card">
          <img src="https://images.unsplash.com/photo-1590608897129-79da98d1593c?auto=format&fit=crop&w=900&q=80" alt="Voix Off">
          <h3>Voix Off — Technique & Studio</h3>
          <p class="muted">Technique vocale, enregistrement, montage audio et livraison.</p>
          <p class="price">25 000 XOF</p>
        </div>
      </div>
    </section>

    <!-- INSCRIPTION + PAIEMENT -->
    <section id="inscription" class="section" style="margin-top:20px">
      <h2>Inscription & Paiement</h2>

      <form id="enroll-form" onsubmit="return false;">
        <input type="text" name="fullName" placeholder="Nom complet" required>
        <input type="email" name="email" placeholder="Email" required>
        <select name="courseId" required>
          <option value="">-- Choisissez une formation --</option>
          <option value="informatique">Informatique — 20 000 XOF</option>
          <option value="infographie">Infographie — 30 000 XOF</option>
          <option value="voixoff">Voix Off — 25 000 XOF</option>
        </select>

        <div class="row">
          <button type="button" id="pay-wave" class="btn" style="background:linear-gradient(90deg,#00c0ff,#0088ff)">Payer avec Wave</button>
          <button type="button" id="pay-orange" class="btn" style="background:linear-gradient(90deg,#ff9a2a,#ff6b00)">Payer avec Orange Money</button>
        </div>
      </form>

      <div id="status" style="margin-top:14px;color:#fff"></div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="section" style="margin-top:20px">
      <h2>Contact</h2>
      <p class="muted">Contactez-nous pour toute question, demande de formation sur mesure, ou partenariat.</p>

      <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:12px">
        <div style="padding:12px;background:rgba(255,255,255,0.03);border-radius:10px">
          <h3>WhatsApp / Téléphone</h3>
          <p class="muted">Wave (principal) : <strong>+221 77 541 42 27</strong></p>
          <p><a class="btn" href="https://wa.me/221775414227" target="_blank">Message Wave</a></p>
          <p class="muted" style="margin-top:10px">Orange Money : <strong>+221 78 502 31 82</strong></p>
          <p><a class="btn" href="https://wa.me/221785023182" target="_blank">Message Orange</a></p>
        </div>

        <div style="padding:12px;background:rgba(255,255,255,0.03);border-radius:10px">
          <h3>Email</h3>
          <p class="muted">Écris-nous : <a href="mailto:wilanethiernoabdourahmane@gmail.com" class="muted">wilanethiernoabdourahmane@gmail.com</a></p>
          <h3 style="margin-top:12px">Envoyer un message</h3>
          <form id="contact-form" onsubmit="return false;">
            <input type="text" name="name" placeholder="Votre nom" required>
            <input type="email" name="contactEmail" placeholder="Votre email" required>
            <textarea name="message" rows="4" placeholder="Votre message" style="width:100%;padding:10px;border-radius:8px;border:none;background:rgba(255,255,255,0.04);color:#fff"></textarea>
            <div style="margin-top:8px">
              <button id="send-message" class="btn secondary">Envoyer (simulé)</button>
            </div>
            <div id="contact-status" style="margin-top:8px;color:#fff"></div>
          </form>
        </div>
      </div>
    </section>
  </main>

  <footer>
    © 2025 Wilane Création — Tous droits réservés
  </footer>

  <script>
    // Course data
    const COURSES = [
      { id: "informatique", name: "Informatique", price: 20000, currency: "XOF" },
      { id: "infographie", name: "Infographie", price: 30000, currency: "XOF" },
      { id: "voixoff", name: "Voix Off", price: 25000, currency: "XOF" }
    ];

    const statusDiv = document.getElementById('status');

    // Wave payment: show instructions and WhatsApp link
    document.getElementById('pay-wave').addEventListener('click', () => {
      const fullName = document.querySelector('input[name=fullName]').value.trim();
      const email = document.querySelector('input[name=email]').value.trim();
      const courseId = document.querySelector('select[name=courseId]').value;
      if(!fullName || !email || !courseId){
        statusDiv.textContent = 'Remplissez votre nom, email et choisissez une formation.';
        return;
      }
      const course = COURSES.find(c=>c.id===courseId);
      statusDiv.innerHTML = `
        <div style="padding:12px;background:rgba(0,0,0,0.25);border-radius:10px">
          <p>💳 <strong>Paiement Wave</strong></p>
          <p>Envoyez <strong>${course.price.toLocaleString()} ${course.currency}</strong> au numéro : <strong>+221 77 541 42 27</strong></p>
          <p>Après paiement, envoyez la capture via WhatsApp pour valider : <a href="https://wa.me/221775414227" target="_blank" class="btn">Contacter +221775414227</a></p>
        </div>
      `;
    });

    // Orange Money payment
    document.getElementById('pay-orange').addEventListener('click', () => {
      const fullName = document.querySelector('input[name=fullName]').value.trim();
      const email = document.querySelector('input[name=email]').value.trim();
      const courseId = document.querySelector('select[name=courseId]').value;
      if(!fullName || !email || !courseId){
        statusDiv.textContent = 'Remplissez votre nom, email et choisissez une formation.';
        return;
      }
      const course = COURSES.find(c=>c.id===courseId);
      statusDiv.innerHTML = `
        <div style="padding:12px;background:rgba(0,0,0,0.25);border-radius:10px">
          <p>📱 <strong>Paiement Orange Money</strong></p>
          <p>Envoyez <strong>${course.price.toLocaleString()} ${course.currency}</strong> au numéro : <strong>+221 78 502 31 82</strong></p>
          <p>Après paiement, envoyez la capture via WhatsApp pour valider : <a href="https://wa.me/221785023182" target="_blank" class="btn">Contacter +221785023182</a></p>
        </div>
      `;
    });

    // Contact form (simulé — sans serveur)
    document.getElementById('send-message').addEventListener('click', () => {
      const name = document.querySelector('#contact-form [name=name]').value.trim();
      const email = document.querySelector('#contact-form [name=contactEmail]').value.trim();
      const message = document.querySelector('#contact-form [name=message]').value.trim();
      const s = document.getElementById('contact-status');
      if(!name || !email || !message){ s.textContent = 'Remplissez tous les champs.'; return; }
      // Since there's no backend, we simulate success.
      s.style.color = '#cfefff';
      s.textContent = 'Message envoyé (simulation) — nous vous répondrons sur ' + email;
      // Optionally you could instruct user to send email to real mailbox:
      // window.location.href = `mailto:wilanethiernoabdourahmane@gmail.com?subject=Message%20depuis%20site%20Wilane&body=${encodeURIComponent(message)}`;
    });

    // Smooth scrolling when clicking nav anchors
    document.querySelectorAll('.nav a').forEach(a=>{
      a.addEventListener('click', (e)=>{
        e.preventDefault();
        const id = a.getAttribute('href').slice(1);
        const el = document.getElementById(id);
        if(el) el.scrollIntoView({behavior:'smooth', block:'start'});
      });
    });
  </script>
</body>
</html>
