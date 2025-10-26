# Emmy-
hhhhhhhhhhhh
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>G-SAVAGEE 💀 | Official Gamer Bio</title>
  <link href="https://fonts.googleapis.com/css2?family=UnifrakturCook:wght@700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Poppins', sans-serif;
      color: #C0C0C0;
      background: #000;
      overflow-x: hidden;
      overflow-y: auto;
    }

    /* ---- Video Background ---- */
    video {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -3;
      opacity: 0;
      transition: opacity 2s ease-in-out;
    }
    .video-bg.loaded,
    .video-smoke.loaded {
      opacity: 1;
    }

    .video-smoke {
      z-index: -2;
      opacity: 0.45;
      mix-blend-mode: lighten;
    }

    /* ---- Spark Overlay ---- */
    .sparks::before, .sparks::after {
      content: '';
      position: fixed;
      width: 100%;
      height: 100%;
      background: repeating-radial-gradient(circle, rgba(255,69,0,0.15) 0, rgba(255,69,0,0.05) 2px, transparent 3px);
      animation: sparksFloat 12s linear infinite;
      mix-blend-mode: screen;
      z-index: -1;
      pointer-events: none;
    }

    @keyframes sparksFloat {
      0% {transform: translate(0, 0);}
      100% {transform: translate(-20px, -40px);}
    }

    /* ---- Overlay Content ---- */
    .overlay {
      background: rgba(0,0,0,0.65);
      min-height: 100vh;
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 2rem;
    }
    h1 {
      font-family: 'UnifrakturCook', cursive;
      font-size: 3rem;
      color: #8B0000;
      text-shadow: 0 0 15px #8B0000;
      animation: fadeIn 2s ease-out;
    }
    h2 {
      font-size: 1.5rem;
      color: #C0C0C0;
      margin-top: 0.5rem;
      animation: fadeIn 3s ease-out;
    }
    p {
      max-width: 600px;
      margin: 1rem auto;
      font-size: 1.1rem;
      line-height: 1.6;
      color: #ccc;
      animation: fadeIn 4s ease-out;
    }

    section {
      padding: 4rem 2rem;
      text-align: center;
      background: rgba(0,0,0,0.85);
      animation: fadeUp 2s;
    }
    .stats {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 2rem;
      margin-top: 2rem;
    }
    .stat {
      border: 1px solid #8B0000;
      padding: 1rem 2rem;
      border-radius: 10px;
      background: rgba(139,0,0,0.2);
      color: #C0C0C0;
      min-width: 120px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .stat:hover {
      transform: scale(1.1);
      box-shadow: 0 0 15px #8B0000;
    }
    .quote {
      font-style: italic;
      color: #C0C0C0;
      font-size: 1.3rem;
      margin-top: 2rem;
      animation: fadeUp 2s ease-out;
    }
    footer {
      background: #111;
      text-align: center;
      padding: 2rem;
      font-size: 0.9rem;
      color: #888;
    }
    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(10px);}
      to {opacity: 1; transform: translateY(0);}
    }
    @keyframes fadeUp {
      from {opacity: 0; transform: translateY(20px);}
      to {opacity: 1; transform: translateY(0);}
    }

    @media (max-width: 768px) {
      h1 { font-size: 2.4rem; }
      h2 { font-size: 1.2rem; }
      p { font-size: 1rem; }
      .stat { min-width: 100px; padding: 0.8rem 1.2rem; }
    }
  </style>
</head>
<body>
  <!-- Lazy-loaded background videos -->
  <video class="video-bg" src="fire_bg.mp4" autoplay muted loop playsinline preload="none"></video>
  <video class="video-smoke" src="smoke_loop.mp4" autoplay muted loop playsinline preload="none"></video>
  <div class="sparks"></div>

  <div class="overlay">
    <h1>𝕲-𝕾𝖆𝖛𝖆𝖌𝖊𝖊 💀</h1>
    <h2>"Shadows don’t talk. They strike."</h2>
    <p><em>Built from silence. Forged in fire.</em></p>
  </div>

  <section id="about">
    <h2>About</h2>
    <p>A silent hunter from the shadows, mastering rifles in Free Fire with ruthless precision.<br>
    Tactical. Patient. Deadly.</p>
  </section>

  <section id="stats">
    <h2>Stats</h2>
    <div class="stats">
      <div class="stat"><strong>Role:</strong><br>Rifler</div>
      <div class="stat"><strong>Region:</strong><br>Nigeria 🇳🇬</div>
      <div class="stat"><strong>Playstyle:</strong><br>Tactical · Patient · Precise</div>
    </div>
  </section>

  <section id="quote">
    <h2>Signature Quote</h2>
    <p class="quote">“I don’t shoot. I erase.”</p>
  </section>

  <footer>
    <p>© 2025 G-SAVAGEE 💀 | Forged in Silence, Born from Shadows</p>
  </footer>

  <!-- Fade-in loader script -->
  <script>
    window.addEventListener('load', () => {
      document.querySelectorAll('video').forEach(v => {
        v.classList.add('loaded');
      });
    });
  </script>
</body>
</html>
