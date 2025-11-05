# Biolog-.Edu.mx
<!doctype html>

<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Muerte Celular HP</title>
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--accent:#8dd3ff;--muted:#9aa7b2}
    html,body{height:100%;margin:0;font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;color:#e6eef6;background:linear-gradient(180deg,#071025 0%, #081827 60%, #071223 100%)}
    .container{max-width:1000px;margin:0 auto;padding:32px}
    header{display:flex;align-items:center;justify-content:space-between;gap:16px}
    h1{margin:0;font-size:1.6rem;letter-spacing:0.6px}
    .hero{display:grid;grid-template-columns:1fr 420px;gap:24px;align-items:center;margin-top:28px}
    .card{background:rgba(255,255,255,0.03);padding:20px;border-radius:12px;box-shadow:0 6px 20px rgba(2,6,23,0.6)}
    p.lead{color:var(--muted);margin:0 0 16px}
    .btn-enter{display:inline-block;padding:12px 18px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#5fb3ff);color:#042033;text-decoration:none;font-weight:600;box-shadow:0 6px 18px rgba(35,111,159,0.18)}/* Animated cells (SVG container) */
.svg-wrap{width:100%;height:100%;display:flex;align-items:center;justify-content:center}
svg{max-width:100%;height:auto;display:block}

/* sections */
#contenido{margin-top:28px;display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:18px}
.section{padding:18px;border-radius:10px;background:linear-gradient(180deg,rgba(255,255,255,0.02),rgba(255,255,255,0.01))}
.section h3{margin-top:0}
footer{margin-top:30px;color:var(--muted);text-align:center;font-size:0.9rem}

/* Small responsive */
@media (max-width:900px){.hero{grid-template-columns:1fr;}.svg-wrap{order:-1}}

/* Subtle floating animation for decorative cells */
.cell{transform-origin:center center;animation:float 6s ease-in-out infinite}
.cell.delay1{animation-delay:0.2s}
.cell.delay2{animation-delay:0.6s}
.cell.delay3{animation-delay:1s}
@keyframes float{0%{transform:translateY(0) scale(1);opacity:1}50%{transform:translateY(-12px) scale(1.06);opacity:0.9}100%{transform:translateY(0) scale(1);opacity:1}}

  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Muerte Celular HP</h1>
      <nav><a class="btn-enter" href="#contenido">Entrar</a></nav>
    </header><main class="hero">
  <div class="card">
    <p class="lead">Una página introductoria y visual sobre los principales tipos de muerte celular: <strong>apoptosis</strong>, <strong>necrosis</strong> y <strong>autofagia</strong>. Diseñada para estudiantes y curiosos de biología.</p>
    <ul>
      <li><strong>Apoptosis</strong>: muerte celular programada, ordenada y sin inflamación.</li>
      <li><strong>Necrosis</strong>: muerte por daño agudo; suele producir inflamación y liberación de contenido celular.</li>
      <li><strong>Autofagia</strong>: proceso de "reciclaje" interno que puede llevar a la supervivencia o a la muerte celular según el contexto.</li>
    </ul>
    <p style="margin-top:12px;color:var(--muted)">Usa el botón "Entrar" para leer más abajo.</p>
  </div>

  <div class="card svg-wrap" aria-hidden="true">
    <!-- Animated 'cells' made with SVG circles -->
    <svg viewBox="0 0 420 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustración animada de células">
      <defs>
        <radialGradient id="g1" cx="30%" cy="30%">
          <stop offset="0%" stop-color="#bfe9ff" stop-opacity="1" />
          <stop offset="100%" stop-color="#3aa0ff" stop-opacity="0.12" />
        </radialGradient>
        <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
          <feGaussianBlur stdDeviation="6" result="blur" />
          <feMerge><feMergeNode in="blur" /><feMergeNode in="SourceGraphic"/></feMerge>
        </filter>
      </defs>

      <!-- fondo de puntos -->
      <rect x="0" y="0" width="420" height="300" fill="url(#g1)" opacity="0.06"/>

      <!-- células -->
      <g transform="translate(40,40)">
        <g class="cell delay1">
          <circle cx="60" cy="40" r="36" fill="#98e6ff" opacity="0.95" filter="url(#glow)" />
          <circle cx="55" cy="35" r="8" fill="#1b6f9b" opacity="0.9" />
        </g>

        <g class="cell delay2" transform="translate(120,20)">
          <circle cx="60" cy="40" r="44" fill="#c7f0ff" opacity="0.9" filter="url(#glow)" />
          <circle cx="68" cy="48" r="10" fill="#17607f" opacity="0.85" />
          <circle cx="46" cy="28" r="6" fill="#2b8db3" opacity="0.8" />
        </g>

        <g class="cell delay3" transform="translate(40,110)">
          <circle cx="60" cy="40" r="28" fill="#9fe0ff" opacity="0.95" filter="url(#glow)" />
        </g>

        <g class="cell" transform="translate(180,110)">
          <circle cx="80" cy="50" r="30" fill="#bdefff" opacity="0.9" filter="url(#glow)" />
          <circle cx="88" cy="58" r="6" fill="#15627a" opacity="0.9" />
        </g>

      </g>
    </svg>
  </div>
</main>

<section id="contenido">
  <article class="section">
    <h3>Apoptosis</h3>
    <p>La apoptosis es la muerte celular programada. Es un proceso activo que la célula inicia y controla mediante rutas internas (ej. caspasas). Es esencial durante el desarrollo y para eliminar células dañadas sin provocar inflamación.</p>
  </article>

  <article class="section">
    <h3>Necrosis</h3>
    <p>La necrosis suele ser consecuencia de daños severos: falta de riego sanguíneo, toxinas o trauma. Produce pérdida de la integridad de la membrana, liberación de contenido intracelular e inflamación local.</p>
  </article>

  <article class="section">
    <h3>Autofagia</h3>
    <p>La autofagia es un mecanismo por el que la célula degrada y recicla componentes propios. Puede ser protector (permitiendo la supervivencia bajo estrés) o, en exceso, contribuir a la muerte celular.</p>
  </article>

  <article class="section">
    <h3>Recursos rápidos</h3>
    <p style="color:var(--muted)">Si quieres, puedo añadir más secciones: imágenes reales de microscopía, referencias bibliográficas, o transformar esto en una página multipágina con enlaces y descarga.</p>
  </article>
</section>

<footer>
  Página creada: <strong>Muerte Celular HP</strong> — Diseño pedagógico y visual. &nbsp; • &nbsp; Hecha para abrir localmente o integrar en un sitio.
</footer>

  </div>
</body>
</html>
