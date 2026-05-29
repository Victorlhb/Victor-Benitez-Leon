<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Currículum web profesional de Víctor Benítez León, perfil DAM junior con experiencia práctica en desarrollo web, automatización de procesos, Microsoft 365, SharePoint y soporte técnico." />
  <title>Víctor Benítez León | Currículum Web DAM</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { box-sizing: border-box; }

    :root {
      --bg: #0f172a;
      --bg-soft: #111827;
      --card: rgba(15, 23, 42, 0.72);
      --card-strong: rgba(30, 41, 59, 0.82);
      --line: rgba(148, 163, 184, 0.22);
      --line-soft: rgba(148, 163, 184, 0.13);
      --text: #f8fafc;
      --text-soft: #cbd5e1;
      --muted: #94a3b8;
      --accent: #60a5fa;
      --accent-strong: #3b82f6;
      --accent-2: #93c5fd;
      --warning: #facc15;
      --shadow: 0 22px 70px rgba(2, 6, 23, 0.36);
      --radius-xl: 26px;
      --radius-lg: 18px;
      --radius-md: 12px;
      --max: 1160px;
      --font-body: "Inter", system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      --font-mono: "JetBrains Mono", ui-monospace, SFMono-Regular, Menlo, Consolas, monospace;
    }

    html { scroll-behavior: smooth; }

    body {
      margin: 0;
      min-height: 100vh;
      color: var(--text);
      font-family: var(--font-body);
      line-height: 1.65;
      background:
        radial-gradient(circle at top left, rgba(59, 130, 246, 0.12), transparent 34rem),
        radial-gradient(circle at top right, rgba(96, 165, 250, 0.08), transparent 32rem),
        linear-gradient(180deg, #0f172a 0%, #0b1220 52%, #090f1a 100%);
      overflow-x: hidden;
    }

    body::before {
      content: "";
      position: fixed;
      inset: 0;
      pointer-events: none;
      background-image:
        linear-gradient(rgba(255, 255, 255, 0.035) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255, 255, 255, 0.035) 1px, transparent 1px);
      background-size: 64px 64px;
      mask-image: linear-gradient(to bottom, rgba(0,0,0,0.8), transparent 62%);
      z-index: -1;
    }

    a { color: inherit; }

    .container {
      width: min(100% - 40px, var(--max));
      margin-inline: auto;
    }

    .topbar {
      position: sticky;
      top: 0;
      z-index: 100;
      border-bottom: 1px solid var(--line-soft);
      background: rgba(9, 15, 26, 0.86);
      backdrop-filter: blur(18px);
    }

    .nav {
      min-height: 76px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 24px;
    }

    .brand {
      display: inline-flex;
      align-items: center;
      gap: 12px;
      color: var(--text);
      text-decoration: none;
      font-weight: 800;
      letter-spacing: -0.04em;
    }

    .brand-mark {
      width: 42px;
      height: 42px;
      display: grid;
      place-items: center;
      border-radius: 14px;
      color: #07111f;
      background: linear-gradient(135deg, var(--accent-strong), var(--accent));
      box-shadow: 0 14px 34px rgba(59, 130, 246, 0.18);
      font-family: var(--font-mono);
      font-size: 0.9rem;
      letter-spacing: -0.08em;
    }

    .brand small {
      display: block;
      margin-top: 1px;
      color: var(--muted);
      font-weight: 500;
      letter-spacing: 0;
      font-size: 0.76rem;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 4px;
      list-style: none;
      padding: 0;
      margin: 0;
    }

    .nav-links a {
      display: inline-flex;
      padding: 10px 12px;
      border-radius: 999px;
      color: var(--text-soft);
      text-decoration: none;
      font-size: 0.88rem;
      font-weight: 600;
      transition: 160ms ease;
    }

    .nav-links a:hover {
      color: var(--text);
      background: rgba(255, 255, 255, 0.075);
    }

    .hero {
      padding: 88px 0 54px;
    }

    .hero-card {
      position: relative;
      overflow: hidden;
      border: 1px solid var(--line);
      border-radius: var(--radius-xl);
      background:
        linear-gradient(135deg, rgba(30, 41, 59, 0.92), rgba(15, 23, 42, 0.76)),
        rgba(15, 23, 42, 0.72);
      box-shadow: var(--shadow);
    }

    .hero-card::after {
      content: "";
      position: absolute;
      right: -180px;
      top: -170px;
      width: 520px;
      height: 520px;
      border-radius: 999px;
      background: radial-gradient(circle, rgba(96, 165, 250, 0.16), rgba(96, 165, 250, 0.035) 50%, transparent 70%);
      pointer-events: none;
    }

    .hero-inner {
      position: relative;
      z-index: 1;
      display: grid;
      grid-template-columns: minmax(0, 1.35fr) minmax(300px, 0.65fr);
      gap: 42px;
      padding: clamp(34px, 5vw, 64px);
      align-items: center;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      width: fit-content;
      padding: 8px 12px;
      margin-bottom: 24px;
      border: 1px solid rgba(96, 165, 250, 0.34);
      border-radius: 999px;
      color: #dbeafe;
      background: rgba(59, 130, 246, 0.09);
      font-family: var(--font-mono);
      font-size: 0.78rem;
      font-weight: 600;
    }

    .status-dot {
      width: 8px;
      height: 8px;
      border-radius: 999px;
      background: var(--accent-2);
      box-shadow: 0 0 0 6px rgba(96, 165, 250, 0.10);
    }

    h1, h2, h3, p { margin: 0; }

    h1 {
      max-width: 850px;
      font-size: clamp(3.1rem, 8vw, 6.75rem);
      line-height: 0.94;
      letter-spacing: -0.075em;
      font-weight: 800;
    }

    .gradient-text {
      color: transparent;
      background: linear-gradient(135deg, #ffffff, #bfdbfe 42%, #60a5fa 82%);
      background-clip: text;
      -webkit-background-clip: text;
    }

    .lead {
      max-width: 710px;
      margin-top: 28px;
      color: var(--text-soft);
      font-size: clamp(1rem, 1.5vw, 1.16rem);
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 34px;
    }

    .button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      min-height: 48px;
      padding: 0 18px;
      border-radius: 999px;
      border: 1px solid transparent;
      text-decoration: none;
      font-weight: 700;
      font-size: 0.94rem;
      transition: 180ms ease;
      cursor: pointer;
    }

    .button.primary {
      color: #06101d;
      background: linear-gradient(135deg, var(--accent), var(--accent-2));
      box-shadow: 0 16px 36px rgba(59, 130, 246, 0.18);
    }

    .button.secondary {
      color: var(--text);
      background: rgba(255, 255, 255, 0.065);
      border-color: var(--line);
    }

    .button:hover { transform: translateY(-2px); }

    .hero-panel {
      border: 1px solid var(--line);
      border-radius: var(--radius-lg);
      background: rgba(8, 12, 24, 0.56);
      box-shadow: 0 18px 60px rgba(0, 0, 0, 0.24);
      overflow: hidden;
    }

    .panel-header {
      display: flex;
      gap: 7px;
      align-items: center;
      min-height: 44px;
      padding: 0 16px;
      border-bottom: 1px solid var(--line-soft);
      background: rgba(255,255,255,0.045);
    }

    .panel-dot { width: 10px; height: 10px; border-radius: 999px; background: rgba(255,255,255,0.24); }

    .panel-body { padding: 22px; }

    .profile-list {
      display: grid;
      gap: 16px;
      margin: 0;
    }

    .profile-row {
      display: grid;
      gap: 3px;
      padding-bottom: 14px;
      border-bottom: 1px solid var(--line-soft);
    }

    .profile-row:last-child { border-bottom: 0; padding-bottom: 0; }

    .profile-row dt {
      color: var(--muted);
      font-family: var(--font-mono);
      font-size: 0.72rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    .profile-row dd {
      margin: 0;
      color: var(--text);
      font-size: 0.98rem;
      font-weight: 650;
    }

    .section {
      padding: 76px 0;
    }

    .section-head {
      display: grid;
      grid-template-columns: 0.45fr 1fr;
      gap: 36px;
      align-items: end;
      margin-bottom: 30px;
    }

    .section-kicker {
      color: var(--accent);
      font-family: var(--font-mono);
      font-size: 0.78rem;
      font-weight: 600;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    .section-title {
      font-size: clamp(2rem, 4vw, 3.35rem);
      line-height: 1.04;
      letter-spacing: -0.06em;
      font-weight: 800;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: 0.95fr 1.05fr;
      gap: 24px;
    }

    .card {
      border: 1px solid var(--line);
      border-radius: var(--radius-lg);
      background: var(--card);
      box-shadow: 0 18px 50px rgba(0, 0, 0, 0.16);
    }

    .card-pad { padding: clamp(22px, 3vw, 30px); }

    .text-block {
      display: grid;
      gap: 16px;
      color: var(--text-soft);
    }

    .text-block strong { color: var(--text); font-weight: 750; }

    .highlights {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 12px;
    }

    .highlight {
      min-height: 132px;
      padding: 18px;
      border: 1px solid var(--line-soft);
      border-radius: var(--radius-md);
      background: rgba(255, 255, 255, 0.045);
    }

    .highlight strong {
      display: block;
      margin-bottom: 6px;
      font-size: 1.36rem;
      letter-spacing: -0.05em;
      color: var(--text);
    }

    .highlight span {
      display: block;
      color: var(--text-soft);
      font-size: 0.9rem;
      line-height: 1.45;
    }

    .skills-grid {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 12px;
    }

    .skill {
      display: grid;
      gap: 8px;
      min-height: 126px;
      padding: 18px;
      border: 1px solid var(--line-soft);
      border-radius: var(--radius-md);
      background: rgba(255, 255, 255, 0.045);
      transition: 180ms ease;
    }

    .skill:hover {
      transform: translateY(-3px);
      border-color: rgba(96, 165, 250, 0.34);
      background: rgba(96, 165, 250, 0.065);
    }

    .skill .icon { font-size: 1.25rem; }

    .skill strong {
      color: var(--text);
      line-height: 1.2;
      letter-spacing: -0.02em;
    }

    .skill span {
      color: var(--muted);
      font-size: 0.82rem;
      line-height: 1.35;
    }

    .timeline {
      display: grid;
      gap: 18px;
    }

    .experience-item {
      display: grid;
      grid-template-columns: 180px 1fr;
      gap: 28px;
      padding: 26px;
      border: 1px solid var(--line);
      border-radius: var(--radius-lg);
      background: var(--card);
      box-shadow: 0 16px 48px rgba(0, 0, 0, 0.14);
    }

    .date {
      color: var(--accent);
      font-family: var(--font-mono);
      font-size: 0.82rem;
      font-weight: 600;
    }

    .experience-content h3 {
      margin-bottom: 5px;
      font-size: 1.18rem;
      letter-spacing: -0.03em;
    }

    .company {
      margin-bottom: 14px;
      color: var(--text-soft);
      font-size: 0.94rem;
    }

    .bullets {
      margin: 0;
      padding: 0;
      list-style: none;
      display: grid;
      gap: 9px;
      color: var(--text-soft);
    }

    .bullets li {
      position: relative;
      padding-left: 22px;
    }

    .bullets li::before {
      content: "";
      position: absolute;
      top: 0.72em;
      left: 0;
      width: 8px;
      height: 8px;
      border-radius: 999px;
      background: linear-gradient(135deg, var(--accent), var(--accent-2));
      transform: translateY(-50%);
    }

    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 16px;
    }

    .tag {
      display: inline-flex;
      align-items: center;
      min-height: 28px;
      padding: 0 10px;
      border: 1px solid rgba(125, 211, 252, 0.22);
      border-radius: 999px;
      color: #dbeafe;
      background: rgba(125, 211, 252, 0.065);
      font-family: var(--font-mono);
      font-size: 0.72rem;
      font-weight: 500;
    }

    .projects-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 16px;
    }

    .project {
      position: relative;
      overflow: hidden;
      min-height: 295px;
      padding: 26px;
      border: 1px solid var(--line);
      border-radius: var(--radius-lg);
      background: var(--card);
      box-shadow: 0 16px 48px rgba(0, 0, 0, 0.14);
    }

    .project::before {
      content: "";
      position: absolute;
      inset: 0;
      background: radial-gradient(circle at top right, rgba(96, 165, 250, 0.10), transparent 48%);
      opacity: 0;
      transition: opacity 180ms ease;
    }

    .project:hover::before { opacity: 1; }

    .project > * { position: relative; z-index: 1; }

    .project-number {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 42px;
      height: 42px;
      margin-bottom: 28px;
      border: 1px solid var(--line);
      border-radius: 14px;
      color: var(--accent);
      background: rgba(255,255,255,0.05);
      font-family: var(--font-mono);
      font-weight: 700;
      font-size: 0.8rem;
    }

    .project h3 {
      margin-bottom: 10px;
      font-size: 1.18rem;
      line-height: 1.25;
      letter-spacing: -0.035em;
    }

    .project p {
      color: var(--text-soft);
      font-size: 0.95rem;
    }

    .project .tags { margin-top: 22px; }

    .education-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 16px;
    }

    .education-card {
      padding: 24px;
      border: 1px solid var(--line);
      border-radius: var(--radius-lg);
      background: var(--card);
    }

    .badge {
      display: inline-flex;
      align-items: center;
      min-height: 28px;
      padding: 0 10px;
      margin-bottom: 18px;
      border-radius: 999px;
      border: 1px solid rgba(96, 165, 250, 0.26);
      color: #dbeafe;
      background: rgba(96, 165, 250, 0.075);
      font-family: var(--font-mono);
      font-size: 0.72rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.05em;
    }

    .education-card h3 {
      margin-bottom: 6px;
      font-size: 1.06rem;
      letter-spacing: -0.03em;
    }

    .education-card p {
      color: var(--text-soft);
      font-size: 0.94rem;
    }

    .contact-card {
      position: relative;
      overflow: hidden;
      padding: clamp(28px, 5vw, 56px);
      border: 1px solid var(--line);
      border-radius: var(--radius-xl);
      background:
        linear-gradient(135deg, rgba(30, 41, 59, 0.88), rgba(15, 23, 42, 0.72)),
        rgba(15, 23, 42, 0.72);
      box-shadow: var(--shadow);
    }

    .contact-card::after {
      content: "";
      position: absolute;
      right: -80px;
      bottom: -120px;
      width: 360px;
      height: 360px;
      border-radius: 999px;
      background: radial-gradient(circle, rgba(96, 165, 250, 0.12), transparent 70%);
    }

    .contact-content {
      position: relative;
      z-index: 1;
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 28px;
      align-items: center;
    }

    .contact-card h2 {
      margin-bottom: 12px;
      font-size: clamp(2rem, 4vw, 3.2rem);
      line-height: 1.05;
      letter-spacing: -0.06em;
    }

    .contact-card p {
      max-width: 650px;
      color: var(--text-soft);
    }

    .contact-list {
      display: grid;
      gap: 10px;
      min-width: 285px;
    }

    .contact-link {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 14px;
      min-height: 48px;
      padding: 0 16px;
      border: 1px solid var(--line);
      border-radius: 999px;
      color: var(--text);
      background: rgba(8, 12, 24, 0.44);
      text-decoration: none;
      font-weight: 650;
      font-size: 0.93rem;
      transition: 180ms ease;
    }

    .contact-link:hover {
      transform: translateY(-2px);
      border-color: rgba(96, 165, 250, 0.40);
    }

    footer {
      padding: 28px 0 44px;
      color: var(--muted);
      font-size: 0.86rem;
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      gap: 18px;
      border-top: 1px solid var(--line-soft);
      padding-top: 24px;
    }

    .reveal {
      opacity: 0;
      transform: translateY(18px);
      transition: opacity 650ms ease, transform 650ms ease;
    }

    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }

    @media (max-width: 980px) {
      .hero-inner,
      .grid-2,
      .section-head,
      .contact-content {
        grid-template-columns: 1fr;
      }

      .skills-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
      .experience-item { grid-template-columns: 1fr; gap: 12px; }
      .contact-list { min-width: 0; }
    }

    @media (max-width: 760px) {
      .container { width: min(100% - 28px, var(--max)); }
      .topbar { position: relative; }
      .nav { min-height: 68px; }
      .brand small { display: none; }
      .nav-links { display: none; }
      .hero { padding-top: 34px; }
      .hero-inner { padding: 26px; }
      h1 { font-size: clamp(3rem, 17vw, 4.8rem); }
      .section { padding: 54px 0; }
      .highlights,
      .skills-grid,
      .projects-grid,
      .education-grid {
        grid-template-columns: 1fr;
      }
      .footer-inner {
        flex-direction: column;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation-duration: 0.001ms !important;
        scroll-behavior: auto !important;
        transition-duration: 0.001ms !important;
      }
      .reveal { opacity: 1; transform: none; }
    }
  </style>
</head>
<body>
  <header class="topbar">
    <nav class="nav container" aria-label="Navegación principal">
      <a class="brand" href="#inicio" aria-label="Ir al inicio">
        <span class="brand-mark">VBL</span>
        <span>Víctor Benítez León<small>Desarrollador DAM · Granada</small></span>
      </a>
      <ul class="nav-links">
        <li><a href="#perfil">Perfil</a></li>
        <li><a href="#experiencia">Experiencia</a></li>
        <li><a href="#proyectos">Proyectos</a></li>
        <li><a href="#tecnologias">Tecnologías</a></li>
        <li><a href="#formacion">Formación</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <main id="inicio">
    <section class="hero container" aria-labelledby="titulo-principal">
      <div class="hero-card reveal">
        <div class="hero-inner">
          <div>
            <div class="eyebrow"><span class="status-dot"></span>Disponible para oportunidades profesionales</div>
            <h1 id="titulo-principal">Perfil DAM junior en desarrollo, automatización y soporte IT.</h1>
            <p class="lead">
              Soy Víctor Benítez León, perfil junior de <strong>DAM</strong>. He trabajado en soluciones útiles para empresas, incluyendo aplicaciones web, automatización de procesos, Microsoft 365, SharePoint y soporte técnico en el día a día.
            </p>
            <div class="hero-actions">
              <a class="button primary" href="#experiencia">Ver experiencia</a>
              <a class="button secondary" href="mailto:victorbenitezleon@gmail.com">Contactar</a>
            </div>
          </div>

          <aside class="hero-panel" aria-label="Resumen profesional">
            <div class="panel-header" aria-hidden="true">
              <span class="panel-dot"></span><span class="panel-dot"></span><span class="panel-dot"></span>
            </div>
            <div class="panel-body">
              <dl class="profile-list">
                <div class="profile-row">
                  <dt>Perfil</dt>
                  <dd>Técnico Superior DAM</dd>
                </div>
                <div class="profile-row">
                  <dt>Especialidad</dt>
                  <dd>Desarrollo web · Automatización · Microsoft 365</dd>
                </div>
                <div class="profile-row">
                  <dt>Ubicación</dt>
                  <dd>Granada, España</dd>
                </div>
                <div class="profile-row">
                  <dt>Stack principal</dt>
                  <dd>Java · Spring Boot · React · Next.js · Supabase</dd>
                </div>
              </dl>
            </div>
          </aside>
        </div>
      </div>
    </section>

    <section id="perfil" class="section container" aria-labelledby="perfil-title">
      <div class="section-head reveal">
        <p class="section-kicker">Perfil profesional</p>
        <h2 id="perfil-title" class="section-title">Experiencia práctica en desarrollo, automatización y soporte técnico.</h2>
      </div>
      <div class="grid-2">
        <article class="card card-pad reveal">
          <div class="text-block">
            <p>
              Actualmente estoy finalizando el ciclo de <strong>Desarrollo de Aplicaciones Multiplataforma</strong>. Durante mi formación y experiencia en empresa he trabajado con programación, automatización y soporte de sistemas dentro de procesos internos de oficina.
            </p>
            <p>
              He participado en tareas relacionadas con documentación de PRL/RRHH, flujos en Microsoft 365, organización de información en SharePoint, despliegues web y soporte a usuarios.
            </p>
            <p>
              Esta experiencia me ha permitido entender tanto la parte técnica como las necesidades de departamentos no técnicos, ayudando a convertir problemas reales en soluciones simples, ordenadas y mantenibles.
            </p>
          </div>
        </article>
        <aside class="card card-pad reveal">
          <div class="highlights">
            <div class="highlight">
              <strong>DAM</strong>
              <span>Formación técnica en desarrollo multiplataforma.</span>
            </div>
            <div class="highlight">
              <strong>M365</strong>
              <span>SharePoint, OneDrive, buzones, permisos y flujos.</span>
            </div>
            <div class="highlight">
              <strong>Web</strong>
              <span>React, Next.js, Supabase, GitHub y Vercel.</span>
            </div>
            <div class="highlight">
              <strong>Sistemas</strong>
              <span>Soporte Windows, NAS Synology y backups.</span>
            </div>
          </div>
        </aside>
      </div>
    </section>


    <section id="experiencia" class="section container" aria-labelledby="experiencia-title">
      <div class="section-head reveal">
        <p class="section-kicker">Experiencia</p>
        <h2 id="experiencia-title" class="section-title">Experiencia práctica en empresa.</h2>
      </div>
      <div class="timeline">
        <article class="experience-item reveal">
          <div class="date">2026</div>
          <div class="experience-content">
            <h3>Técnico en sistemas, automatización y desarrollo</h3>
            <p class="company">Limpiezas Las Nieves · Prácticas DAM</p>
            <ul class="bullets">
              <li>Automatización de procesos documentales de PRL, RRHH y archivo mediante Power Automate y SharePoint.</li>
              <li>Diseño de soluciones internas para reducir tareas manuales y mejorar la organización de documentación empresarial.</li>
              <li>Configuración de NAS Synology DS925+ y apoyo en copias de seguridad de Microsoft 365.</li>
              <li>Soporte técnico en entorno Windows y Microsoft 365: permisos, buzones, usuarios, incidencias y documentación interna.</li>
              <li>Desarrollo y despliegue de aplicaciones web internas con React, Next.js, Supabase, GitHub y Vercel.</li>
            </ul>
            <div class="tags">
              <span class="tag">Power Automate</span><span class="tag">SharePoint</span><span class="tag">Microsoft 365</span><span class="tag">React</span><span class="tag">Next.js</span><span class="tag">Supabase</span><span class="tag">Synology</span>
            </div>
          </div>
        </article>

        <article class="experience-item reveal">
          <div class="date">2025</div>
          <div class="experience-content">
            <h3>Desarrollador multiplataforma</h3>
            <p class="company">NanoBytes · Prácticas DAM</p>
            <ul class="bullets">
              <li>Uso de Odoo ERP en entorno empresarial para tareas de facturación, clientes y procesos de gestión.</li>
              <li>Familiarización con el funcionamiento interno de un ERP y su relación con procesos de negocio.</li>
            </ul>
            <div class="tags"><span class="tag">Odoo ERP</span><span class="tag">Gestión empresarial</span><span class="tag">PostgreSQL</span></div>
          </div>
        </article>

        <article class="experience-item reveal">
          <div class="date">2024</div>
          <div class="experience-content">
            <h3>Distribuidor · Logística de reparto</h3>
            <p class="company">Panadería Tito</p>
            <ul class="bullets">
              <li>Planificación y realización de rutas de reparto, organización diaria y trato con clientes.</li>
            </ul>
          </div>
        </article>

        <article class="experience-item reveal">
          <div class="date">06/2022 – 04/2023</div>
          <div class="experience-content">
            <h3>Operario de limpieza viaria</h3>
            <p class="company">Ayuntamiento de Gójar · Granada</p>
            <ul class="bullets">
              <li>Limpieza de espacios públicos, uso de maquinaria y cumplimiento de tareas operativas asignadas.</li>
            </ul>
          </div>
        </article>
      </div>
    </section>

    <section id="proyectos" class="section container" aria-labelledby="proyectos-title">
      <div class="section-head reveal">
        <p class="section-kicker">Proyectos</p>
        <h2 id="proyectos-title" class="section-title">Soluciones aplicadas a casos reales.</h2>
      </div>
      <div class="projects-grid">
        <article class="project reveal">
          <span class="project-number">01</span>
          <h3>Automatización documental para PRL y RRHH</h3>
          <p>Flujos con Power Automate para guardar, clasificar y organizar documentación en SharePoint, reduciendo tareas repetitivas y errores manuales.</p>
          <div class="tags"><span class="tag">Power Automate</span><span class="tag">SharePoint</span><span class="tag">Microsoft 365</span></div>
        </article>

        <article class="project reveal">
          <span class="project-number">02</span>
          <h3>Aplicaciones web internas</h3>
          <p>Desarrollo de herramientas web para empresa, conectadas a Supabase y desplegadas con Vercel, manteniendo control de versiones en GitHub.</p>
          <div class="tags"><span class="tag">React</span><span class="tag">Next.js</span><span class="tag">Supabase</span><span class="tag">Vercel</span></div>
        </article>

        <article class="project reveal">
          <span class="project-number">03</span>
          <h3>Infraestructura NAS y copias M365</h3>
          <p>Apoyo en configuración de NAS Synology DS925+ y planteamiento de copias de seguridad para OneDrive, Exchange y SharePoint.</p>
          <div class="tags"><span class="tag">Synology</span><span class="tag">Backups</span><span class="tag">Microsoft 365</span></div>
        </article>

        <article class="project reveal">
          <span class="project-number">04</span>
          <h3>Gestión ERP con Odoo</h3>
          <p>Uso de Odoo en procesos de gestión empresarial, especialmente facturación, clientes y comprensión del flujo de trabajo de un ERP.</p>
          <div class="tags"><span class="tag">Odoo</span><span class="tag">ERP</span><span class="tag">Gestión</span></div>
        </article>
      </div>
    </section>

    <section id="tecnologias" class="section container" aria-labelledby="tecnologias-title">
      <div class="section-head reveal">
        <p class="section-kicker">Tecnologías</p>
        <h2 id="tecnologias-title" class="section-title">Herramientas con las que he trabajado.</h2>
      </div>
      <div class="skills-grid reveal">
        <div class="skill"><span class="icon">☕</span><strong>Java</strong><span>Backend y programación orientada a objetos.</span></div>
        <div class="skill"><span class="icon">🌱</span><strong>Spring Boot</strong><span>APIs, capas y acceso a datos.</span></div>
        <div class="skill"><span class="icon">⚛️</span><strong>React / Next.js</strong><span>Interfaces web y despliegue moderno.</span></div>
        <div class="skill"><span class="icon">🟨</span><strong>JavaScript</strong><span>Lógica de frontend e integración.</span></div>
        <div class="skill"><span class="icon">🐘</span><strong>PostgreSQL</strong><span>Modelado y consulta de datos.</span></div>
        <div class="skill"><span class="icon">🐬</span><strong>MySQL</strong><span>Bases de datos relacionales.</span></div>
        <div class="skill"><span class="icon">⚡</span><strong>Supabase</strong><span>Backend como servicio y storage.</span></div>
        <div class="skill"><span class="icon">🔁</span><strong>Power Automate</strong><span>Automatización documental y procesos.</span></div>
        <div class="skill"><span class="icon">📂</span><strong>SharePoint</strong><span>Bibliotecas, listas y permisos.</span></div>
        <div class="skill"><span class="icon">🐳</span><strong>Docker</strong><span>Entornos y despliegues controlados.</span></div>
        <div class="skill"><span class="icon">🐙</span><strong>GitHub</strong><span>Control de versiones y repositorios.</span></div>
        <div class="skill"><span class="icon">🚀</span><strong>Vercel</strong><span>Publicación de proyectos web.</span></div>
      </div>
    </section>

    <section id="formacion" class="section container" aria-labelledby="formacion-title">
      <div class="section-head reveal">
        <p class="section-kicker">Formación</p>
        <h2 id="formacion-title" class="section-title">Formación académica y complementaria.</h2>
      </div>
      <div class="education-grid reveal">
        <article class="education-card">
          <span class="badge">En curso</span>
          <h3>Técnico Superior en Desarrollo de Aplicaciones Multiplataforma</h3>
          <p>Atlántida CIDEP · 2024 – 2026</p>
        </article>
        <article class="education-card">
          <span class="badge">Completado</span>
          <h3>Bachillerato de Humanidades</h3>
          <p>IES Juan XIII · Granada</p>
        </article>
        <article class="education-card">
          <span class="badge">80 horas</span>
          <h3>Formación en JavaScript</h3>
          <p>Curso especializado orientado a desarrollo web.</p>
        </article>
        <article class="education-card">
          <span class="badge">40 horas</span>
          <h3>Ciberseguridad</h3>
          <p>Formación complementaria en conceptos de seguridad informática.</p>
        </article>
      </div>
    </section>

    <section id="contacto" class="section container" aria-labelledby="contacto-title">
      <div class="contact-card reveal">
        <div class="contact-content">
          <div>
            <p class="section-kicker">Contacto</p>
            <h2 id="contacto-title">Datos de contacto.</h2>
            <p>Puedes contactar conmigo para procesos de selección, entrevistas o puestos junior relacionados con desarrollo web, soporte técnico, sistemas, Microsoft 365 o automatización de procesos internos.</p>
          </div>
          <div class="contact-list" aria-label="Datos de contacto">
            <a class="contact-link" href="mailto:victorbenitezleon@gmail.com"><span>Email</span><span>→</span></a>
            <a class="contact-link" href="tel:+34680121683"><span>680 121 683</span><span>→</span></a>
            <span class="contact-link"><span>Granada · 18150</span><span>ES</span></span>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container footer-inner">
      <span>© 2026 Víctor Benítez León</span>
      <span>Currículum web profesional · Desarrollo DAM</span>
    </div>
  </footer>

  <script>
    const revealObserver = new IntersectionObserver((entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          revealObserver.unobserve(entry.target);
        }
      });
    }, { threshold: 0.12 });

    document.querySelectorAll('.reveal').forEach((element) => revealObserver.observe(element));
  </script>
</body>
</html>
