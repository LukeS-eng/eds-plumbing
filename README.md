[eds-plumbing.html](https://github.com/user-attachments/files/26256510/eds-plumbing.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ed's Plumbing — Walla Walla, WA</title>
  <meta name="description" content="Licensed & bonded plumber in Walla Walla, WA. Residential & commercial plumbing, new construction, remodels, and repairs. 15+ years experience. Call for a free quote."/>
  <link rel="preconnect" href="https://fonts.googleapis.com"/>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
  <link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;600;700;800&family=Lora:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --navy: #0d1b2a;
      --navy-mid: #162033;
      --navy-light: #1e2d42;
      --copper: #c8732a;
      --copper-light: #e08840;
      --copper-glow: #f0a060;
      --cream: #f5f0e8;
      --cream-dark: #ede5d8;
      --white: #ffffff;
      --gray: #8a9ab0;
      --gray-light: #b8c5d4;
      --text-dark: #0d1b2a;
      --star: #f5b942;
      --font-head: 'Barlow Condensed', sans-serif;
      --font-body: 'Lora', serif;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      font-family: var(--font-body);
      background: var(--cream);
      color: var(--text-dark);
      overflow-x: hidden;
    }

    /* ── HEADER ── */
    header {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 100;
      background: var(--navy);
      border-bottom: 2px solid var(--copper);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 clamp(1rem, 4vw, 2.5rem);
      height: 64px;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .logo-icon {
      width: 36px;
      height: 36px;
      background: var(--copper);
      border-radius: 6px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 18px;
      flex-shrink: 0;
    }

    .logo-text {
      font-family: var(--font-head);
      font-weight: 800;
      font-size: 1.25rem;
      color: var(--white);
      letter-spacing: 0.04em;
      text-transform: uppercase;
      line-height: 1.1;
    }

    .logo-text span {
      display: block;
      font-size: 0.65rem;
      font-weight: 400;
      color: var(--gray-light);
      letter-spacing: 0.12em;
      text-transform: uppercase;
    }

    .header-cta {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .phone-link {
      font-family: var(--font-head);
      font-weight: 700;
      font-size: clamp(1rem, 2.5vw, 1.2rem);
      color: var(--copper-glow);
      text-decoration: none;
      letter-spacing: 0.03em;
      transition: color 0.2s;
    }
    .phone-link:hover { color: var(--white); }

    .btn-call {
      background: var(--copper);
      color: var(--white);
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 0.9rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      text-decoration: none;
      padding: 10px 20px;
      border-radius: 4px;
      transition: background 0.2s, transform 0.15s;
      white-space: nowrap;
    }
    .btn-call:hover { background: var(--copper-light); transform: translateY(-1px); }

    /* ── HERO ── */
    .hero {
      background: var(--navy);
      padding: 120px clamp(1rem, 5vw, 3rem) 80px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: -60px; right: -60px;
      width: 500px; height: 500px;
      background: radial-gradient(circle, rgba(200,115,42,0.12) 0%, transparent 70%);
      pointer-events: none;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: 0; left: 0; right: 0;
      height: 4px;
      background: linear-gradient(90deg, transparent, var(--copper), transparent);
    }

    /* Pipe decorations */
    .pipe-deco {
      position: absolute;
      right: clamp(20px, 6vw, 80px);
      top: 50%;
      transform: translateY(-50%);
      opacity: 0.06;
      font-size: 180px;
      color: var(--copper);
      font-family: var(--font-head);
      font-weight: 800;
      letter-spacing: -0.05em;
      pointer-events: none;
      user-select: none;
    }

    .hero-inner {
      max-width: 780px;
      position: relative;
    }

    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: rgba(200,115,42,0.15);
      border: 1px solid rgba(200,115,42,0.3);
      border-radius: 100px;
      padding: 6px 16px;
      margin-bottom: 24px;
      font-family: var(--font-head);
      font-size: 0.8rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--copper-glow);
    }

    .hero-badge::before {
      content: '';
      width: 6px; height: 6px;
      background: var(--copper-glow);
      border-radius: 50%;
      animation: pulse 2s ease-in-out infinite;
    }

    @keyframes pulse {
      0%, 100% { opacity: 1; transform: scale(1); }
      50% { opacity: 0.5; transform: scale(0.8); }
    }

    h1 {
      font-family: var(--font-head);
      font-weight: 800;
      font-size: clamp(2.4rem, 6vw, 4.2rem);
      line-height: 1.05;
      color: var(--white);
      text-transform: uppercase;
      letter-spacing: 0.02em;
      margin-bottom: 20px;
    }

    h1 em {
      font-style: normal;
      color: var(--copper-glow);
    }

    .hero-sub {
      font-size: clamp(1rem, 2vw, 1.15rem);
      color: var(--gray-light);
      max-width: 580px;
      line-height: 1.7;
      margin-bottom: 36px;
    }

    .hero-ctas {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      align-items: center;
    }

    .btn-primary {
      background: var(--copper);
      color: var(--white);
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 1.1rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      padding: 16px 36px;
      border-radius: 4px;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: background 0.2s, transform 0.15s, box-shadow 0.2s;
      box-shadow: 0 4px 20px rgba(200,115,42,0.3);
    }
    .btn-primary:hover {
      background: var(--copper-light);
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(200,115,42,0.4);
    }

    .btn-secondary {
      background: transparent;
      color: var(--gray-light);
      font-family: var(--font-head);
      font-weight: 600;
      font-size: 1rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      padding: 16px 24px;
      border: 1px solid rgba(255,255,255,0.15);
      border-radius: 4px;
      transition: all 0.2s;
    }
    .btn-secondary:hover { border-color: var(--copper); color: var(--copper-glow); }

    .hero-trust {
      display: flex;
      align-items: center;
      gap: 20px;
      margin-top: 48px;
      padding-top: 32px;
      border-top: 1px solid rgba(255,255,255,0.08);
      flex-wrap: wrap;
    }

    .trust-item {
      display: flex;
      align-items: center;
      gap: 8px;
      color: var(--gray);
      font-size: 0.85rem;
    }

    .trust-item strong {
      color: var(--gray-light);
      font-family: var(--font-head);
      font-weight: 600;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      font-size: 0.8rem;
    }

    .trust-dot {
      width: 4px; height: 4px;
      background: var(--copper);
      border-radius: 50%;
    }

    /* ── SOCIAL PROOF ── */
    .proof-bar {
      background: var(--copper);
      padding: 20px clamp(1rem, 4vw, 3rem);
      display: flex;
      align-items: center;
      justify-content: center;
      gap: clamp(12px, 3vw, 40px);
      flex-wrap: wrap;
    }

    .proof-rating {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .stars {
      display: flex;
      gap: 2px;
    }

    .star { color: var(--star); font-size: 1.1rem; }

    .rating-num {
      font-family: var(--font-head);
      font-weight: 800;
      font-size: 1.5rem;
      color: var(--white);
      letter-spacing: 0.02em;
    }

    .rating-count {
      color: rgba(255,255,255,0.8);
      font-size: 0.9rem;
    }

    .proof-divider {
      width: 1px;
      height: 32px;
      background: rgba(255,255,255,0.3);
    }

    .proof-text {
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 1rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--white);
    }

    /* ── SECTION SHARED ── */
    section {
      padding: clamp(60px, 8vw, 100px) clamp(1rem, 5vw, 3rem);
    }

    .section-label {
      font-family: var(--font-head);
      font-weight: 600;
      font-size: 0.75rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--copper);
      margin-bottom: 12px;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .section-label::before {
      content: '';
      display: block;
      width: 28px;
      height: 2px;
      background: var(--copper);
    }

    h2 {
      font-family: var(--font-head);
      font-weight: 800;
      font-size: clamp(1.8rem, 4vw, 2.8rem);
      text-transform: uppercase;
      letter-spacing: 0.02em;
      line-height: 1.1;
      margin-bottom: 16px;
    }

    .section-sub {
      font-size: 1rem;
      color: #5a6a7a;
      line-height: 1.7;
      max-width: 560px;
      margin-bottom: 48px;
    }

    /* ── SERVICES ── */
    .services { background: var(--navy); }
    .services h2 { color: var(--white); }
    .services .section-sub { color: var(--gray); }

    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 2px;
      border: 2px solid rgba(200,115,42,0.2);
      border-radius: 8px;
      overflow: hidden;
    }

    .service-card {
      background: var(--navy-light);
      padding: 32px 28px;
      transition: background 0.2s;
      position: relative;
    }

    .service-card::before {
      content: '';
      position: absolute;
      top: 0; left: 0;
      width: 3px; height: 0;
      background: var(--copper);
      transition: height 0.3s ease;
    }

    .service-card:hover { background: var(--navy-mid); }
    .service-card:hover::before { height: 100%; }

    .service-icon {
      font-size: 1.8rem;
      margin-bottom: 16px;
      display: block;
    }

    .service-card h3 {
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 1.1rem;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      color: var(--white);
      margin-bottom: 10px;
    }

    .service-card p {
      font-size: 0.9rem;
      color: var(--gray);
      line-height: 1.6;
    }

    /* ── ABOUT ── */
    .about { background: var(--cream); }

    .about-inner {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: clamp(32px, 6vw, 80px);
      align-items: center;
      max-width: 1100px;
      margin: 0 auto;
    }

    .about-visual {
      background: var(--navy);
      border-radius: 8px;
      padding: 48px 40px;
      position: relative;
      overflow: hidden;
    }

    .about-visual::before {
      content: '15+';
      position: absolute;
      top: -20px; right: -10px;
      font-family: var(--font-head);
      font-weight: 800;
      font-size: 9rem;
      color: rgba(200,115,42,0.08);
      line-height: 1;
      pointer-events: none;
    }

    .stat-block {
      position: relative;
      padding: 24px 0;
      border-bottom: 1px solid rgba(255,255,255,0.07);
    }
    .stat-block:last-child { border-bottom: none; padding-bottom: 0; }
    .stat-block:first-child { padding-top: 0; }

    .stat-num {
      font-family: var(--font-head);
      font-weight: 800;
      font-size: 2.8rem;
      color: var(--copper-glow);
      line-height: 1;
      margin-bottom: 4px;
    }

    .stat-label {
      font-family: var(--font-head);
      font-weight: 600;
      font-size: 0.8rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--gray);
    }

    .about-content h2 { color: var(--text-dark); }

    .about-body {
      font-size: 1rem;
      line-height: 1.8;
      color: #4a5a6a;
      margin-bottom: 24px;
    }

    .license-block {
      display: flex;
      flex-direction: column;
      gap: 8px;
      padding: 20px;
      background: var(--navy);
      border-radius: 6px;
      border-left: 3px solid var(--copper);
      margin-top: 28px;
    }

    .license-item {
      font-family: var(--font-head);
      font-size: 0.85rem;
      letter-spacing: 0.06em;
      color: var(--gray-light);
    }

    .license-item strong {
      color: var(--copper-glow);
    }

    /* ── REVIEWS ── */
    .reviews { background: var(--cream-dark); }
    .reviews h2 { color: var(--text-dark); }

    .reviews-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      margin-top: 0;
    }

    .review-card {
      background: var(--white);
      border-radius: 8px;
      padding: 28px;
      box-shadow: 0 2px 16px rgba(13,27,42,0.06);
      border-bottom: 3px solid var(--copper);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .review-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 32px rgba(13,27,42,0.1);
    }

    .review-stars { margin-bottom: 16px; }
    .review-stars .star { font-size: 0.9rem; }

    .review-text {
      font-size: 0.95rem;
      line-height: 1.7;
      color: #3a4a5a;
      font-style: italic;
      margin-bottom: 20px;
    }

    .reviewer {
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 0.85rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--navy);
    }

    /* ── HOURS + LOCATION ── */
    .location { background: var(--navy); }
    .location h2 { color: var(--white); }
    .location .section-sub { color: var(--gray); }

    .location-inner {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: clamp(32px, 6vw, 80px);
      max-width: 1000px;
    }

    .hours-block {
      display: flex;
      flex-direction: column;
      gap: 0;
    }

    .hours-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 14px 0;
      border-bottom: 1px solid rgba(255,255,255,0.07);
      font-size: 0.95rem;
    }

    .hours-row:last-child { border-bottom: none; }

    .day {
      font-family: var(--font-head);
      font-weight: 600;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      font-size: 0.85rem;
      color: var(--gray-light);
    }

    .time {
      color: var(--copper-glow);
      font-family: var(--font-head);
      font-weight: 600;
      font-size: 0.85rem;
    }

    .contact-block {
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

    .contact-item {
      display: flex;
      gap: 14px;
      align-items: flex-start;
    }

    .contact-icon {
      width: 40px;
      height: 40px;
      background: rgba(200,115,42,0.15);
      border: 1px solid rgba(200,115,42,0.3);
      border-radius: 6px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.1rem;
      flex-shrink: 0;
    }

    .contact-info strong {
      display: block;
      font-family: var(--font-head);
      font-weight: 600;
      font-size: 0.75rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--gray);
      margin-bottom: 4px;
    }

    .contact-info a, .contact-info span {
      color: var(--white);
      text-decoration: none;
      font-size: 1rem;
      transition: color 0.2s;
    }

    .contact-info a:hover { color: var(--copper-glow); }

    /* ── FINAL CTA ── */
    .final-cta {
      background: var(--copper);
      text-align: center;
      padding: clamp(60px, 8vw, 100px) clamp(1rem, 5vw, 3rem);
      position: relative;
      overflow: hidden;
    }

    .final-cta::before {
      content: '';
      position: absolute;
      top: -100px; left: 50%;
      transform: translateX(-50%);
      width: 600px; height: 300px;
      background: radial-gradient(ellipse, rgba(255,255,255,0.1) 0%, transparent 70%);
      pointer-events: none;
    }

    .final-cta h2 {
      color: var(--white);
      font-size: clamp(2rem, 5vw, 3.5rem);
      margin-bottom: 12px;
      position: relative;
    }

    .final-cta p {
      color: rgba(255,255,255,0.85);
      font-size: 1.05rem;
      margin-bottom: 36px;
      position: relative;
    }

    .btn-white {
      background: var(--white);
      color: var(--copper);
      font-family: var(--font-head);
      font-weight: 800;
      font-size: 1.2rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      padding: 18px 44px;
      border-radius: 4px;
      display: inline-block;
      transition: transform 0.2s, box-shadow 0.2s;
      box-shadow: 0 4px 24px rgba(0,0,0,0.15);
      position: relative;
    }
    .btn-white:hover { transform: translateY(-2px); box-shadow: 0 8px 36px rgba(0,0,0,0.2); }

    /* ── FOOTER ── */
    footer {
      background: #080f17;
      padding: 32px clamp(1rem, 4vw, 3rem);
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 16px;
    }

    .footer-left {
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 1rem;
      color: var(--white);
      text-transform: uppercase;
      letter-spacing: 0.06em;
    }

    .footer-left span {
      display: block;
      font-size: 0.75rem;
      font-weight: 400;
      color: var(--gray);
      letter-spacing: 0.04em;
      margin-top: 2px;
      text-transform: none;
    }

    .footer-right {
      font-size: 0.8rem;
      color: var(--gray);
      text-align: right;
    }

    /* ── MOBILE ── */
    @media (max-width: 700px) {
      .header-cta .btn-call { display: none; }

      .about-inner,
      .location-inner { grid-template-columns: 1fr; }

      .about-visual { padding: 32px 24px; }
      .about-visual::before { font-size: 6rem; }

      .proof-divider { display: none; }

      footer { flex-direction: column; text-align: center; }
      .footer-right { text-align: center; }

      .hero-ctas .btn-secondary { display: none; }
      .btn-primary { width: 100%; justify-content: center; }
    }

    /* ── BOOKING ── */
    .booking { background: var(--cream); }
    .booking h2 { color: var(--text-dark); }

    .calendly-wrapper {
      max-width: 900px;
    }

    .calendly-placeholder {
      background: var(--navy);
      border-radius: 8px;
      padding: 60px 40px;
      text-align: center;
      border: 2px dashed rgba(200,115,42,0.35);
    }

    .calendly-icon { font-size: 2.5rem; margin-bottom: 16px; }

    .calendly-msg {
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 1.1rem;
      letter-spacing: 0.04em;
      text-transform: uppercase;
      color: var(--white);
      margin-bottom: 8px;
    }

    .calendly-sub {
      color: var(--gray);
      font-size: 0.9rem;
      margin-bottom: 28px;
      line-height: 1.6;
    }

    .calendly-input-row {
      display: flex;
      gap: 10px;
      max-width: 520px;
      margin: 0 auto;
      flex-wrap: wrap;
    }

    .calendly-input-row input {
      flex: 1;
      padding: 12px 16px;
      border-radius: 4px;
      border: 1px solid rgba(200,115,42,0.4);
      background: rgba(255,255,255,0.06);
      color: var(--white);
      font-family: var(--font-body);
      font-size: 0.9rem;
      outline: none;
      min-width: 200px;
    }

    .calendly-input-row input::placeholder { color: var(--gray); }
    .calendly-input-row input:focus { border-color: var(--copper); }

    .calendly-input-row button {
      background: var(--copper);
      color: var(--white);
      border: none;
      padding: 12px 24px;
      border-radius: 4px;
      font-family: var(--font-head);
      font-weight: 700;
      font-size: 0.9rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      cursor: pointer;
      transition: background 0.2s;
      white-space: nowrap;
    }
    .calendly-input-row button:hover { background: var(--copper-light); }

    /* ── SCROLL ANIMATIONS ── */
    .fade-up {
      opacity: 0;
      transform: translateY(24px);
      transition: opacity 0.6s ease, transform 0.6s ease;
    }
    .fade-up.visible { opacity: 1; transform: translateY(0); }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <div class="logo">
      <div class="logo-icon">🔧</div>
      <div class="logo-text">
        Ed's Plumbing
        <span>Walla Walla, WA</span>
      </div>
    </div>
    <div class="header-cta">
      <a href="tel:+15095407108" class="phone-link">📞 (509) 540-7108</a>
      <a href="#book" class="btn-call" style="background:transparent; border:1px solid rgba(200,115,42,0.5); color:var(--copper-glow);">Book Online</a>
      <a href="tel:+15095407108" class="btn-call">Call Now</a>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="pipe-deco">|||</div>
    <div class="hero-inner">
      <div class="hero-badge">Now accepting new clients — Free quotes</div>
      <h1>Walla Walla's Trusted <em>Plumber</em> — Done Right, Every Time</h1>
      <p class="hero-sub">
        Edgar Gonzalez has been solving plumbing problems for homeowners and businesses across Walla Walla for over 15 years. New construction, full remodels, or a quick repair — call or text for a free quote today.
      </p>
      <div class="hero-ctas">
        <a href="tel:+15095407108" class="btn-primary">📞 Call or Text Now</a>
        <a href="#services" class="btn-secondary">View Services</a>
      </div>
      <div class="hero-trust">
        <div class="trust-item">
          <strong>⭐ 4.9 Stars</strong>
          <span>— 39 Google Reviews</span>
        </div>
        <div class="trust-dot"></div>
        <div class="trust-item">
          <strong>Licensed & Bonded</strong>
          <span>— WA State Certified</span>
        </div>
        <div class="trust-dot"></div>
        <div class="trust-item">
          <strong>15+ Years</strong>
          <span>— Commercial & Residential</span>
        </div>
      </div>
    </div>
  </section>

  <!-- SOCIAL PROOF BAR -->
  <div class="proof-bar">
    <div class="proof-rating">
      <div class="stars">
        <span class="star">★</span>
        <span class="star">★</span>
        <span class="star">★</span>
        <span class="star">★</span>
        <span class="star">★</span>
      </div>
      <span class="rating-num">4.9</span>
      <span class="rating-count">on Google</span>
    </div>
    <div class="proof-divider"></div>
    <div class="proof-text">39 Five-Star Reviews</div>
    <div class="proof-divider"></div>
    <div class="proof-text">Free Quotes · Call or Text</div>
  </div>

  <!-- SERVICES -->
  <section class="services" id="services">
    <div class="section-label">What We Do</div>
    <h2>Full-Service Plumbing<br>for Home & Business</h2>
    <p class="section-sub">
      From ground-up builds to emergency repairs, Ed handles it all. Residential or commercial — no job is too big or too small.
    </p>
    <div class="services-grid fade-up">
      <div class="service-card">
        <span class="service-icon">🏠</span>
        <h3>Residential Plumbing</h3>
        <p>Repairs, installations, and upgrades for your home. Sinks, toilets, water heaters, and everything in between.</p>
      </div>
      <div class="service-card">
        <span class="service-icon">🏢</span>
        <h3>Commercial Plumbing</h3>
        <p>Reliable commercial work for businesses, restaurants, and multi-unit properties throughout Walla Walla.</p>
      </div>
      <div class="service-card">
        <span class="service-icon">🔨</span>
        <h3>New Construction</h3>
        <p>Full plumbing rough-in and finish work for new builds. On-schedule, code-compliant, and built to last.</p>
      </div>
      <div class="service-card">
        <span class="service-icon">🛁</span>
        <h3>Remodels</h3>
        <p>Kitchen and bathroom remodels done right. New layouts, fixture upgrades, and full replumbing.</p>
      </div>
      <div class="service-card">
        <span class="service-icon">🔧</span>
        <h3>Repairs</h3>
        <p>Leaks, clogs, burst pipes, water heater issues — fast diagnosis and lasting fixes.</p>
      </div>
      <div class="service-card">
        <span class="service-icon">📋</span>
        <h3>Free Estimates</h3>
        <p>Not sure what you need? Call or text and Ed will walk you through your options — no pressure, no obligation.</p>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section class="about" id="about">
    <div class="about-inner">
      <div class="about-visual fade-up">
        <div class="stat-block">
          <div class="stat-num">15+</div>
          <div class="stat-label">Years of Experience</div>
        </div>
        <div class="stat-block">
          <div class="stat-num">4.9★</div>
          <div class="stat-label">Average Google Rating</div>
        </div>
        <div class="stat-block">
          <div class="stat-num">2-in-1</div>
          <div class="stat-label">Residential & Commercial</div>
        </div>
        <div class="license-block">
          <div class="license-item">Bond: <strong>#PJ7538</strong></div>
          <div class="license-item">License: <strong>#EDSPLPL804N4</strong></div>
          <div class="license-item" style="color: var(--gray); font-size: 0.75rem;">Washington State Licensed & Bonded</div>
        </div>
      </div>
      <div class="about-content fade-up">
        <div class="section-label">About Ed</div>
        <h2>Local Plumber,<br>Real Experience</h2>
        <p class="about-body">
          My name is Edgar Gonzalez and I've been serving the Walla Walla community for over 15 years. I specialize in both residential and commercial plumbing — from new construction builds to full remodels and everyday repairs.
        </p>
        <p class="about-body">
          When you call Ed's Plumbing, you're talking directly to me. No dispatcher, no middleman — just a licensed professional who shows up, does the work, and stands behind it.
        </p>
        <a href="tel:+15095407108" class="btn-primary" style="display:inline-flex;">
          📞 Get a Free Quote
        </a>
      </div>
    </div>
  </section>

  <!-- REVIEWS -->
  <section class="reviews" id="reviews">
    <div class="section-label">What Clients Say</div>
    <h2>39 Five-Star Reviews<br>and Counting</h2>
    <p class="section-sub">Don't take our word for it — here's what Walla Walla homeowners and businesses say about Ed's work.</p>
    <div class="reviews-grid fade-up">
      <div class="review-card">
        <div class="review-stars">
          <span class="star">★</span><span class="star">★</span><span class="star">★</span><span class="star">★</span><span class="star">★</span>
        </div>
        <p class="review-text">"Ed did an excellent job on my plumbing project. From start to finish, he was professional, clean, and transparent about the work that needed to be done. He took the time to explain options and costs, and the final result was perfect. I would absolutely use him again and recommend him to anyone needing a dependable plumber."</p>
        <div class="reviewer">— Google Reviewer</div>
      </div>
      <div class="review-card">
        <div class="review-stars">
          <span class="star">★</span><span class="star">★</span><span class="star">★</span><span class="star">★</span><span class="star">★</span>
        </div>
        <p class="review-text">"I requested help with a water filter system and Ed came out and was able to improvise so I could use the system. 6 months later I forgot which was the main valve — a quick phone call to Ed, who remembered and helped me by phone. That is TOP notch customer service. So appreciative of Ed for his expertise and genuine caring for his customers."</p>
        <div class="reviewer">— Google Reviewer</div>
      </div>
      <div class="review-card">
        <div class="review-stars">
          <span class="star">★</span><span class="star">★</span><span class="star">★</span><span class="star">★</span><span class="star">★</span>
        </div>
        <p class="review-text">"We were introduced to Ed when I had a water heater leak. Since then we've called him several more times for a variety of plumbing issues — he has officially become 'our plumber' and earned a permanent spot in my important contacts. If you're looking for a plumber who is knowledgeable, honest, prompt, and reasonably priced, Ed is your guy."</p>
        <div class="reviewer">— Google Reviewer</div>
      </div>
    </div>
    <p style="text-align:center; margin-top: 28px; color: #6a7a8a; font-size: 0.9rem;">
      Read all 39 reviews on <a href="https://maps.google.com" target="_blank" style="color: var(--copper); text-decoration: none; font-weight: 600;">Google Maps →</a>
    </p>
  </section>

  <!-- HOURS + CONTACT -->
  <section class="location" id="contact">
    <div class="section-label">Hours & Contact</div>
    <h2>Ready When You Need Us</h2>
    <p class="section-sub">Call or text anytime. Ed responds fast and offers free quotes on all jobs.</p>
    <div class="location-inner fade-up">
      <div class="hours-block">
        <div class="hours-row"><span class="day">Monday</span><span class="time">6 AM – 6 PM</span></div>
        <div class="hours-row"><span class="day">Tuesday</span><span class="time">6 AM – 6 PM</span></div>
        <div class="hours-row"><span class="day">Wednesday</span><span class="time">6 AM – 6 PM</span></div>
        <div class="hours-row"><span class="day">Thursday</span><span class="time">6 AM – 6 PM</span></div>
        <div class="hours-row"><span class="day">Friday</span><span class="time">6 AM – 6 PM</span></div>
        <div class="hours-row"><span class="day">Saturday</span><span class="time">Call for availability</span></div>
        <div class="hours-row"><span class="day">Sunday</span><span class="time">Call for availability</span></div>
      </div>
      <div class="contact-block">
        <div class="contact-item">
          <div class="contact-icon">📞</div>
          <div class="contact-info">
            <strong>Phone / Text</strong>
            <a href="tel:+15095407108">(509) 540-7108</a>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">📍</div>
          <div class="contact-info">
            <strong>Service Area</strong>
            <span>Walla Walla, WA & surrounding areas</span>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">💬</div>
          <div class="contact-info">
            <strong>Free Quotes</strong>
            <span>Call or text for a no-obligation estimate</span>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">✅</div>
          <div class="contact-info">
            <strong>Licensed & Bonded</strong>
            <span>WA State — Bond #PJ7538</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- BOOK ONLINE -->
  <section class="booking" id="book">
    <div class="section-label">Schedule Online</div>
    <h2>Book a Free Consultation</h2>
    <p class="section-sub">Pick a time that works for you and Ed will reach out to confirm. Fast, easy, no phone tag.</p>
    <div class="calendly-wrapper fade-up">
      <div class="calendly-placeholder" id="calendly-placeholder">
        <div class="calendly-icon">📅</div>
        <p class="calendly-msg">Calendly booking will appear here.</p>
        <p class="calendly-sub">Paste your Calendly link below to activate online scheduling.</p>
        <div class="calendly-input-row">
          <input type="text" id="calendly-url" placeholder="https://calendly.com/your-link" />
          <button onclick="loadCalendly()">Load Calendar</button>
        </div>
      </div>
      <div id="calendly-embed" style="display:none; min-height:650px; border-radius:8px; overflow:hidden;"></div>
    </div>
  </section>

  <!-- FINAL CTA -->
  <section class="final-cta">
    <h2>Need a Plumber in Walla Walla?</h2>
    <p>Call or text Edgar directly. Free quote, fast response, quality work — guaranteed.</p>
    <a href="tel:+15095407108" class="btn-white">📞 (509) 540-7108</a>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="footer-left">
      Ed's Plumbing
      <span>Walla Walla, WA · Licensed & Bonded</span>
    </div>
    <div class="footer-right">
      Bond #PJ7538 · License #EDSPLPL804N4<br>
      © 2025 Ed's Plumbing. All rights reserved.
    </div>
  </footer>

  <script>
    // Scroll fade-in
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(e => {
        if (e.isIntersecting) {
          e.target.classList.add('visible');
          observer.unobserve(e.target);
        }
      });
    }, { threshold: 0.12 });

    document.querySelectorAll('.fade-up').forEach(el => observer.observe(el));

    // Calendly loader
    function loadCalendly() {
      const input = document.getElementById('calendly-url').value.trim();
      if (!input) { alert('Please paste your Calendly link first.'); return; }
      const url = input.startsWith('http') ? input : 'https://' + input;

      // Load Calendly widget script
      const script = document.createElement('script');
      script.src = 'https://assets.calendly.com/assets/external/widget.js';
      document.head.appendChild(script);

      // Load Calendly CSS
      const link = document.createElement('link');
      link.rel = 'stylesheet';
      link.href = 'https://assets.calendly.com/assets/external/widget.css';
      document.head.appendChild(link);

      // Show embed, hide placeholder
      document.getElementById('calendly-placeholder').style.display = 'none';
      const embed = document.getElementById('calendly-embed');
      embed.style.display = 'block';
      embed.innerHTML = `<div class="calendly-inline-widget" data-url="${url}?hide_gdpr_banner=1&primary_color=c8732a" style="min-width:320px;height:650px;"></div>`;

      script.onload = function() {
        if (window.Calendly) Calendly.initInlineWidgets();
      };
    }

    // Auto-load if URL param provided: eds-plumbing.html?calendly=https://calendly.com/...
    const params = new URLSearchParams(window.location.search);
    if (params.get('calendly')) {
      document.getElementById('calendly-url').value = params.get('calendly');
      loadCalendly();
    }
  </script>

</body>
</html>
