
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
    /* LOGO agrandi pour remplir le cercle */
    header img{
      width:180px; height:180px; border-radius:50%; object-fit:cover;
      border:4px solid rgba(255,255,255,0.95); box-shadow:0 14px 40px rgba(255,115,0,0.16);
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
    .card img{width:100%;height:200px;object-fit:cover;border-radius:8px;margin-bottom:12px}
    .card h3{margin:6px 0}
    .price{color:#cfefff;font-weight:700}

    form{display:block; margin-top:12px}
    input,select,textarea{width:100%;padding:10px;border-radius:8px;border:none;margin-bottom:10px;outline:none;background:rgba(255,255,255,0.04);color:#fff}
    .row{display:flex;gap:10px;flex-wrap:wrap}
    .row .btn{flex:1}

    .btn{
      display:inline-block;padding:10px 14px;border-radius:10px;background:var(--dark);color:#fff;text-decoration:none;border:none;cursor:pointer;font-weight:700;
      box-shadow: 0 6px 18px rgba(0,0,0,0.4);
    }
    .btn.secondary{background:transparent;border:1px solid rgba(255,255,255,0.08)}
    .muted{color:rgba(255,255,255,0.8)}

    footer{color:rgba(255,255,255,0.7);text-align:center;padding:30px 10px;margin-top:30px}

    /* small screens */
    @media(max-width:640px){
      header h1{font-size:1.6rem}
      .nav{left:12px; transform:none; top:12px}
      body{font-size:15px}
      header img{width:140px;height:140px}
    }

    /* helper */
    .contact-card{padding:12px;background:rgba(255,255,255,0.03);border-radius:10px}
  </style>
</head>
<body>

  <!-- NAV -->
  <nav class="nav" aria-label="Main navigation">
    <a href="index.html">Accueil</a>
    <a href="a-propos.html">À propos</a>
    <a href="formations.html">Formations</a>
    <a href="contact.html">Contact</a>
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
          <img src="informatique.jpg" alt="Informatique">
          <h3>Informatique — Bureautique & Maintenance</h3>
          <p class="muted">Word, Excel, PowerPoint, Internet et maintenance de base.</p>
          <p class="price">20 000 XOF</p>
        </div>

        <!-- Infographie -->
        <div class="card">
          <img src="infographie.jpg" alt="Infographie">
          <h3>Infographie — Photoshop & Illustrator</h3>
          <p class="muted">Design visuel, logos, affiches et supports marketing.</p>
          <p class="price">30 000 XOF</p>
        </div>

        <!-- Voix Off (image locale) -->
        <div class="card">
          <img src="voixoff.jpg" alt="Voix Off">
          <h3>Voix Off — Technique & Studio</h3>
          <p class="muted">Technique vocale, enregistrement, montage audio et livraison.</p>
          <p class="price">25 000 XOF</p>
        </div>
      </div>
    </section>

    <!-- INSCRIPTION & PAIEMENT -->
    <section id="inscription" class="section" style="margin-top:20px">
      <h2>Inscription</h2>

      <form id="register-form">
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px">
          <input type="text" name="prenom" placeholder="Prénom" required>
          <input type="text" name="nom" placeholder="Nom" required>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:8px">
          <input type="email" name="email" placeholder="Email" required>
          <input type="tel" name="telephone" placeholder="Téléphone (ex: +22177...)" required>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:8px">
          <select name="formation" required>
            <option value="">-- Choisissez une formation --</option>
            <option value="Informatique">Informatique — 20 000 XOF</option>
            <option value="Infographie">Infographie — 30 000 XOF</option>
            <option value="Voix Off">Voix Off — 25 000 XOF</option>
          </select>

          <input type="text" name="lieu" placeholder="Lieu (ville/centre)" required>
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:8px">
          <select name="niveau" required>
            <option value="">-- Niveau d'études --</option>
            <option value="Aucun">Aucun</option>
            <option value="Primaire">Primaire</option>
            <option value="Secondaire">Secondaire</option>
            <option value="Bac">Bac</option>
            <option value="Licence">Licence</option>
            <option value="Master">Master</option>
            <option value="Autre">Autre</option>
          </select>

          <input type="text" name="ville" placeholder="Ville" required>
        </div>

        <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
          <button type="submit" class="btn">Confirmer et envoyer</button>
          <button type="button" id="btn-pay-web" class="btn secondary">Payer via Web</button>
          <button type="button" id="btn-pay-wave" class="btn" style="background:linear-gradient(90deg,#00c0ff,#0088ff)">Payer via Wave</button>
          <button type="button" id="btn-pay-orange" class="btn" style="background:linear-gradient(90deg,#ff9a2a,#ff6b00)">Payer via Orange Money</button>
        </div>
      </form>

      <div id="register-status" style="margin-top:14px;color:#fff"></div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="section" style="margin-top:20px">
      <h2>Contact</h2>
      <p class="muted">Contactez-nous pour toute question, demande de formation sur mesure ou partenariat.</p>

      <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:12px">
        <div class="contact-card">
          <h3>Contact Wave</h3>
          <p class="muted">+221 77 541 42 27</p>
          <!-- bouton "Message" ouvre WhatsApp avec texte pré-rempli -->
          <p><a class="btn" id="wa-wave" href="#" target="_blank">Message</a></p>
        </div>

        <div class="contact-card">
          <h3>Contact Orange Money</h3>
          <p class="muted">+221 78 502 31 82</p>
          <p><a class="btn" id="wa-orange" href="#" target="_blank">Message</a></p>
        </div>
      </div>
    </section>
  </main>

  <footer>
    © 2025 Wilane Création — Tous droits réservés
  </footer>

  <script>
    /*******************************
     * CONFIGURATION (Personnalise)
     *******************************/
    const OWNER_EMAIL = "wilanethiernoabdourahmane@gmail.com"; // email destinataire des inscriptions
    const PAYMENT_WEB_LINK = "https://example.com/checkout"; // <-- remplace par ton lien web de paiement
    const WHATSAPP_WAVE = "+221775414227";   // sans espaces ni +
    const WHATSAPP_ORANGE = "+221785023182"; // sans espaces ni +
    // Pré-remplisable message pour contact rapide (remplacera {msg} ci-dessous)
    const CONTACT_MESSAGE = "Bonjour, je souhaite avoir des informations sur vos formations.";

    /* Si tu veux envoyer automatiquement depuis le client (sans ouvrir le mail client),
       tu peux utiliser EmailJS ou un service similaire. Remplace ces valeurs si tu utilises EmailJS.
       Si EmailJS n'est pas configuré, le code fait fallback vers mailto (ouvre la messagerie du visiteur). */
    const EMAILJS_USER_ID = "";    // ex: 'user_XXXXXXXX'  (laisser vide si pas utilisé)
    const EMAILJS_SERVICE_ID = ""; // ex: 'service_xxx'
    const EMAILJS_TEMPLATE_ID = ""; // ex: 'template_xxx'

    /***********************
     * Fonctions utilitaires
     ***********************/
    function urlEncode(str){ return encodeURIComponent(str).replace(/'/g,"%27"); }

    // Construire lien WhatsApp avec texte URL-encodé
    function whatsappLink(phone, text){
      // phone expected like '+221775414227' or '221775414227' or '+221775414227'
      let p = phone.replace(/\+/g,'').replace(/\s+/g,'');
      return "https://wa.me/" + p + "?text=" + encodeURIComponent(text);
    }

    // Afficher message de statut
    function setStatus(msg, color = "#cfefff"){
      const el = document.getElementById('register-status');
      el.style.color = color;
      el.innerHTML = msg;
    }

    /************************
     * Préparer boutons WA
     ************************/
    document.getElementById('wa-wave').href = whatsappLink(WHATSAPP_WAVE, CONTACT_MESSAGE);
    document.getElementById('wa-orange').href = whatsappLink(WHATSAPP_ORANGE, CONTACT_MESSAGE);

    /************************
     * Gestion du formulaire
     ************************/
    document.getElementById('register-form').addEventListener('submit', async function(ev){
      ev.preventDefault();
      setStatus('');
      const f = ev.target;
      const data = {
        prenom: f.prenom.value.trim(),
        nom: f.nom.value.trim(),
        email: f.email.value.trim(),
        telephone: f.telephone.value.trim(),
        formation: f.formation.value,
        lieu: f.lieu.value.trim(),
        niveau: f.niveau.value,
        ville: f.ville.value.trim()
      };
      // Validation simple
      if(!data.prenom || !data.nom || !data.email || !data.telephone || !data.formation){
        setStatus("Remplissez tous les champs obligatoires.", "#ffb3b3");
        return;
      }

      // Tenter EmailJS si configuré
      if(EMAILJS_USER_ID && EMAILJS_SERVICE_ID && EMAILJS_TEMPLATE_ID){
        try{
          // charger EmailJS si nécessaire (client-side)
          if(typeof emailjs === 'undefined'){
            const s = document.createElement('script');
            s.src = 'https://cdn.emailjs.com/sdk/3.2.0/email.min.js';
            document.head.appendChild(s);
            await new Promise(r=>s.onload=r);
            emailjs.init(EMAILJS_USER_ID);
          }
          const templateParams = {
            prenom: data.prenom,
            nom: data.nom,
            email: data.email,
            telephone: data.telephone,
            formation: data.formation,
            lieu: data.lieu,
            niveau: data.niveau,
            ville: data.ville,
            owner_email: OWNER_EMAIL
          };
          await emailjs.send(EMAILJS_SERVICE_ID, EMAILJS_TEMPLATE_ID, templateParams);
          setStatus("Inscription envoyée — nous avons reçu vos informations. Vérifiez votre WhatsApp pour le paiement.", "#cfefff");
        }catch(err){
          console.error(err);
          setStatus("Erreur lors de l'envoi automatique. Nous ouvrons votre messagerie pour envoyer les informations.", "#ffb3b3");
          // fallback to mailto below
          fallbackMailTo(data);
        }
      } else {
        // fallback : ouvrir mail client (mailto:) avec contenu pré-rempli pour t'envoyer l'email
        fallbackMailTo(data);
      }

      // Afficher options de paiement dynamiquement
      showPaymentOptions(data);
    });

    // fallback : ouvrir le client mail du visiteur pour envoyer à OWNER_EMAIL
    function fallbackMailTo(data){
      const subject = "Nouvelle inscription - Wilane Création - " + data.formation;
      const body =
        "Inscription Wilane Création %0A%0A" +
        "Prénom: " + encodeURIComponent(data.prenom) + "%0A" +
        "Nom: " + encodeURIComponent(data.nom) + "%0A" +
        "Email: " + encodeURIComponent(data.email) + "%0A" +
        "Téléphone: " + encodeURIComponent(data.telephone) + "%0A" +
        "Formation: " + encodeURIComponent(data.formation) + "%0A" +
        "Lieu: " + encodeURIComponent(data.lieu) + "%0A" +
        "Niveau d'études: " + encodeURIComponent(data.niveau) + "%0A" +
        "Ville: " + encodeURIComponent(data.ville) + "%0A";
      // ouverture du client mail
      window.location.href = `mailto:${OWNER_EMAIL}?subject=${encodeURIComponent(subject)}&body=${body}`;
    }

    /************************
     * Paiement après inscription
     ************************/
    function showPaymentOptions(data){
      const status = document.getElementById('register-status');
      // calcul montant selon formation
      const priceMap = {
        "Informatique": 20000,
        "Infographie": 30000,
        "Voix Off": 25000
      };
      const amount = priceMap[data.formation] || 0;
      const formatted = amount.toLocaleString() + " XOF";

      // message pré-rempli pour paiement (WhatsApp)
      const payTextWave = `Bonjour, je confirme mon paiement pour la formation ${data.formation} (${formatted}). Nom: ${data.prenom} ${data.nom}. Téléphone: ${data.telephone}. Email: ${data.email}.`;
      const payTextOrange = payTextWave; // même message

      // éléments de paiement
      status.innerHTML = `
        <div style="padding:12px;background:rgba(0,0,0,0.32);border-radius:10px">
          <p style="margin:0 0 8px">Inscription reçue pour <strong>${escapeHtml(data.formation)}</strong> — montant: <strong>${formatted}</strong></p>
          <div style="display:flex;gap:8px;flex-wrap:wrap;margin-top:8px">
            <a class="btn" href="${PAYMENT_WEB_LINK}" target="_blank">Payer via Web</a>
            <a class="btn" style="background:linear-gradient(90deg,#00c0ff,#0088ff)" href="${whatsappLink(WHATSAPP_WAVE,payTextWave)}" target="_blank">Payer via Wave</a>
            <a class="btn" style="background:linear-gradient(90deg,#ff9a2a,#ff6b00)" href="${whatsappLink(WHATSAPP_ORANGE,payTextOrange)}" target="_blank">Payer via Orange Money</a>
          </div>
          <p style="margin-top:10px;font-size:0.9em;color:#ddd">Après paiement, envoyez la capture via WhatsApp au même numéro pour confirmation.</p>
        </div>
      `;
    }

    // small helper to escape html in inserted text
    function escapeHtml(text){
      return String(text).replace(/[&<>"']/g, function(m){ return {'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[m]; });
    }

    /************************
     * Boutons paiement directs (si l'utilisateur clique avant inscription)
     ************************/
    document.getElementById('btn-pay-web').addEventListener('click', ()=> {
      window.open(PAYMENT_WEB_LINK, '_blank');
    });
    document.getElementById('btn-pay-wave').addEventListener('click', ()=> {
      // open simple payment message (generic)
      const text = "Bonjour, je souhaite payer une formation. Merci.";
      window.open(whatsappLink(WHATSAPP_WAVE, text), '_blank');
    });
    document.getElementById('btn-pay-orange').addEventListener('click', ()=> {
      const text = "Bonjour, je souhaite payer une formation via Orange Money. Merci.";
      window.open(whatsappLink(WHATSAPP_ORANGE, text), '_blank');
    });

  </script>
</body>
</html>
