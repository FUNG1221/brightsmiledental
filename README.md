<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Liberty Legal Group | New York Law Firm</title>

  <meta name="description" content="Liberty Legal Group provides trusted legal representation in New York for personal injury, family law, criminal defense, immigration, business law, and estate planning." />
  <meta name="keywords" content="New York law firm, personal injury lawyer, family law attorney, criminal defense lawyer, immigration lawyer, business attorney, estate planning lawyer" />

  <meta property="og:title" content="Liberty Legal Group | Trusted Legal Representation" />
  <meta property="og:description" content="Premium legal services in New York. Free consultation available." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?auto=format&fit=crop&w=1600&q=80" />

  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;600;700&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />

  <style>
    :root {
      --navy: #071b3a;
      --navy-light: #0c2d5b;
      --gold: #c8a24a;
      --gold-light: #e2c46f;
      --white: #ffffff;
      --gray: #f4f6f8;
      --text: #1d2939;
      --muted: #667085;
      --dark: #050d1c;
      --shadow: 0 18px 45px rgba(7, 27, 58, 0.15);
      --radius: 18px;
      --transition: all 0.35s ease;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: "Inter", sans-serif;
      color: var(--text);
      background: var(--white);
      line-height: 1.7;
      overflow-x: hidden;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    img {
      max-width: 100%;
      display: block;
    }

    .container {
      width: min(1180px, 92%);
      margin: auto;
    }

    .section {
      padding: 100px 0;
    }

    .section-light {
      background: var(--gray);
    }

    .section-title {
      text-align: center;
      margin-bottom: 60px;
    }

    .section-title span {
      color: var(--gold);
      font-weight: 700;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      font-size: 14px;
    }

    .section-title h2 {
      font-family: "Cinzel", serif;
      color: var(--navy);
      font-size: clamp(32px, 4vw, 48px);
      margin-top: 10px;
      line-height: 1.2;
    }

    .section-title p {
      max-width: 720px;
      margin: 16px auto 0;
      color: var(--muted);
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      padding: 15px 26px;
      border-radius: 999px;
      font-weight: 700;
      transition: var(--transition);
      cursor: pointer;
      border: none;
    }

    .btn-gold {
      background: linear-gradient(135deg, var(--gold), var(--gold-light));
      color: var(--navy);
      box-shadow: 0 12px 30px rgba(200, 162, 74, 0.35);
    }

    .btn-gold:hover {
      transform: translateY(-3px);
      box-shadow: 0 18px 40px rgba(200, 162, 74, 0.45);
    }

    .btn-outline {
      border: 2px solid rgba(255,255,255,0.75);
      color: var(--white);
    }

    .btn-outline:hover {
      background: var(--white);
      color: var(--navy);
      transform: translateY(-3px);
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 999;
      background: rgba(7, 27, 58, 0.92);
      backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(255,255,255,0.1);
    }

    .navbar {
      height: 82px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 12px;
      color: var(--white);
      font-family: "Cinzel", serif;
      font-size: 23px;
      font-weight: 700;
    }

    .logo i {
      color: var(--gold);
    }

    .nav-links {
      display: flex;
      list-style: none;
      gap: 26px;
      align-items: center;
    }

    .nav-links a {
      color: rgba(255,255,255,0.92);
      font-size: 15px;
      font-weight: 600;
      transition: var(--transition);
    }

    .nav-links a:hover {
      color: var(--gold);
    }

    .menu-toggle {
      display: none;
      color: var(--white);
      font-size: 26px;
      cursor: pointer;
    }

    .hero {
      min-height: 100vh;
      background:
        linear-gradient(115deg, rgba(7,27,58,0.94), rgba(7,27,58,0.6)),
        url("https://images.unsplash.com/photo-1589829545856-d10d557cf95f?auto=format&fit=crop&w=1800&q=80") center/cover no-repeat;
      color: var(--white);
      display: flex;
      align-items: center;
      padding-top: 90px;
      position: relative;
    }

    .hero-content {
      max-width: 780px;
      animation: fadeUp 1s ease forwards;
    }

    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      background: rgba(255,255,255,0.12);
      border: 1px solid rgba(255,255,255,0.22);
      padding: 10px 18px;
      border-radius: 999px;
      color: var(--gold-light);
      font-weight: 700;
      margin-bottom: 24px;
    }

    .hero h1 {
      font-family: "Cinzel", serif;
      font-size: clamp(42px, 7vw, 78px);
      line-height: 1.05;
      margin-bottom: 24px;
    }

    .hero p {
      font-size: 19px;
      max-width: 680px;
      color: rgba(255,255,255,0.88);
      margin-bottom: 34px;
    }

    .hero-actions {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
    }

    .hero-stats {
      margin-top: 55px;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
      max-width: 720px;
    }

    .hero-stat {
      background: rgba(255,255,255,0.11);
      border: 1px solid rgba(255,255,255,0.16);
      padding: 24px;
      border-radius: var(--radius);
      backdrop-filter: blur(10px);
    }

    .hero-stat strong {
      display: block;
      color: var(--gold-light);
      font-size: 32px;
      font-family: "Cinzel", serif;
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 55px;
      align-items: center;
    }

    .about-img {
      position: relative;
    }

    .about-img img {
      border-radius: 24px;
      box-shadow: var(--shadow);
    }

    .about-card {
      position: absolute;
      bottom: -30px;
      right: -25px;
      background: var(--navy);
      color: var(--white);
      padding: 28px;
      border-radius: 20px;
      max-width: 260px;
      box-shadow: var(--shadow);
    }

    .about-card i {
      color: var(--gold);
      font-size: 34px;
      margin-bottom: 14px;
    }

    .about-text h2 {
      font-family: "Cinzel", serif;
      color: var(--navy);
      font-size: clamp(32px, 4vw, 48px);
      line-height: 1.2;
      margin-bottom: 22px;
    }

    .about-text p {
      color: var(--muted);
      margin-bottom: 18px;
    }

    .check-list {
      list-style: none;
      margin: 25px 0;
    }

    .check-list li {
      margin-bottom: 12px;
      font-weight: 600;
    }

    .check-list i {
      color: var(--gold);
      margin-right: 10px;
    }

    .practice-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 28px;
    }

    .practice-card,
    .attorney-card,
    .result-card,
    .testimonial-card,
    .choose-card {
      background: var(--white);
      border-radius: var(--radius);
      padding: 34px;
      box-shadow: var(--shadow);
      transition: var(--transition);
      border: 1px solid rgba(7,27,58,0.08);
    }

    .practice-card:hover,
    .attorney-card:hover,
    .result-card:hover,
    .testimonial-card:hover,
    .choose-card:hover {
      transform: translateY(-10px);
    }

    .icon-box {
      width: 66px;
      height: 66px;
      border-radius: 18px;
      background: rgba(200,162,74,0.14);
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--gold);
      font-size: 28px;
      margin-bottom: 22px;
    }

    .practice-card h3,
    .choose-card h3,
    .result-card h3 {
      color: var(--navy);
      font-size: 22px;
      margin-bottom: 12px;
    }

    .practice-card p,
    .choose-card p,
    .result-card p {
      color: var(--muted);
      margin-bottom: 20px;
    }

    .learn-link {
      color: var(--navy);
      font-weight: 800;
      display: inline-flex;
      gap: 8px;
      align-items: center;
    }

    .choose-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 22px;
    }

    .choose-card {
      text-align: center;
      padding: 28px 20px;
    }

    .choose-card .number {
      font-family: "Cinzel", serif;
      color: var(--gold);
      font-size: 36px;
      font-weight: 700;
      margin-bottom: 8px;
    }

    .attorney-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 30px;
    }

    .attorney-card {
      padding: 0;
      overflow: hidden;
    }

    .attorney-card img {
      height: 340px;
      width: 100%;
      object-fit: cover;
    }

    .attorney-info {
      padding: 30px;
    }

    .attorney-info h3 {
      color: var(--navy);
      font-size: 24px;
      margin-bottom: 5px;
    }

    .position {
      color: var(--gold);
      font-weight: 800;
      margin-bottom: 15px;
    }

    .attorney-meta {
      color: var(--muted);
      font-size: 14px;
      margin-bottom: 12px;
    }

    .results-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 24px;
    }

    .result-amount {
      font-family: "Cinzel", serif;
      color: var(--gold);
      font-size: 34px;
      font-weight: 700;
      margin-bottom: 10px;
    }

    .testimonial-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 26px;
    }

    .stars {
      color: var(--gold);
      margin-bottom: 16px;
      letter-spacing: 2px;
    }

    .testimonial-card p {
      color: var(--muted);
      margin-bottom: 22px;
      font-style: italic;
    }

    .client {
      color: var(--navy);
      font-weight: 800;
    }

    .faq-wrap {
      max-width: 920px;
      margin: auto;
    }

    .faq-item {
      background: var(--white);
      margin-bottom: 16px;
      border-radius: 16px;
      box-shadow: var(--shadow);
      overflow: hidden;
    }

    .faq-question {
      padding: 22px 26px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      cursor: pointer;
      font-weight: 800;
      color: var(--navy);
    }

    .faq-answer {
      max-height: 0;
      overflow: hidden;
      transition: var(--transition);
      color: var(--muted);
      padding: 0 26px;
    }

    .faq-item.active .faq-answer {
      max-height: 180px;
      padding: 0 26px 24px;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 38px;
    }

    .contact-info,
    .contact-form {
      background: var(--white);
      border-radius: 24px;
      padding: 38px;
      box-shadow: var(--shadow);
    }

    .contact-info h3,
    .contact-form h3 {
      color: var(--navy);
      font-size: 28px;
      margin-bottom: 24px;
      font-family: "Cinzel", serif;
    }

    .contact-row {
      display: flex;
      gap: 16px;
      margin-bottom: 22px;
      color: var(--muted);
    }

    .contact-row i {
      color: var(--gold);
      font-size: 22px;
      width: 26px;
      margin-top: 4px;
    }

    form input,
    form select,
    form textarea {
      width: 100%;
      padding: 15px 16px;
      margin-bottom: 16px;
      border-radius: 12px;
      border: 1px solid #d0d5dd;
      font-family: inherit;
      outline: none;
      transition: var(--transition);
    }

    form input:focus,
    form select:focus,
    form textarea:focus {
      border-color: var(--gold);
      box-shadow: 0 0 0 4px rgba(200,162,74,0.14);
    }

    textarea {
      min-height: 130px;
      resize: vertical;
    }

    .map {
      margin-top: 35px;
      border-radius: 24px;
      overflow: hidden;
      box-shadow: var(--shadow);
    }

    .map iframe {
      width: 100%;
      height: 360px;
      border: 0;
    }

    footer {
      background: var(--dark);
      color: rgba(255,255,255,0.82);
      padding: 70px 0 25px;
    }

    .footer-grid {
      display: grid;
      grid-template-columns: 1.4fr 1fr 1fr 1.2fr;
      gap: 35px;
      margin-bottom: 45px;
    }

    footer h3,
    footer h4 {
      color: var(--white);
      margin-bottom: 20px;
    }

    footer h3 {
      font-family: "Cinzel", serif;
      font-size: 25px;
    }

    footer ul {
      list-style: none;
    }

    footer li {
      margin-bottom: 10px;
    }

    footer a:hover {
      color: var(--gold);
    }

    .socials {
      display: flex;
      gap: 12px;
      margin-top: 18px;
    }

    .socials a {
      width: 42px;
      height: 42px;
      background: rgba(255,255,255,0.08);
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      transition: var(--transition);
    }

    .socials a:hover {
      background: var(--gold);
      color: var(--navy);
      transform: translateY(-4px);
    }

    .copyright {
      border-top: 1px solid rgba(255,255,255,0.12);
      padding-top: 24px;
      text-align: center;
      color: rgba(255,255,255,0.58);
    }

    .sticky-call,
    .sticky-consult,
    .back-top {
      position: fixed;
      z-index: 998;
      border-radius: 999px;
      box-shadow: var(--shadow);
    }

    .sticky-call {
      left: 22px;
      bottom: 22px;
      width: 58px;
      height: 58px;
      background: var(--gold);
      color: var(--navy);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 24px;
      animation: pulse 1.8s infinite;
    }

    .sticky-consult {
      right: 22px;
      bottom: 22px;
      background: var(--navy);
      color: var(--white);
      padding: 15px 22px;
      font-weight: 800;
    }

    .back-top {
      right: 22px;
      bottom: 88px;
      width: 46px;
      height: 46px;
      background: var(--white);
      color: var(--navy);
      display: none;
      align-items: center;
      justify-content: center;
    }

    .back-top.show {
      display: flex;
    }

    .reveal {
      opacity: 0;
      transform: translateY(35px);
      transition: 0.8s ease;
    }

    .reveal.active {
      opacity: 1;
      transform: translateY(0);
    }

    @keyframes fadeUp {
      from {
        opacity: 0;
        transform: translateY(35px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes pulse {
      0% {
        box-shadow: 0 0 0 0 rgba(200,162,74,0.6);
      }
      70% {
        box-shadow: 0 0 0 18px rgba(200,162,74,0);
      }
      100% {
        box-shadow: 0 0 0 0 rgba(200,162,74,0);
      }
    }

    @media (max-width: 1024px) {
      .practice-grid,
      .testimonial-grid,
      .attorney-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .choose-grid,
      .results-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .footer-grid,
      .about-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }

      .about-card {
        right: 20px;
      }
    }

    @media (max-width: 768px) {
      .menu-toggle {
        display: block;
      }

      .nav-links {
        position: absolute;
        top: 82px;
        left: 0;
        width: 100%;
        background: var(--navy);
        flex-direction: column;
        padding: 25px;
        display: none;
      }

      .nav-links.active {
        display: flex;
      }

      .hero-stats,
      .practice-grid,
      .testimonial-grid,
      .attorney-grid,
      .choose-grid,
      .results-grid {
        grid-template-columns: 1fr;
      }

      .section {
        padding: 75px 0;
      }

      .sticky-consult {
        display: none;
      }
    }
  </style>

  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "LegalService",
    "name": "Liberty Legal Group",
    "image": "https://images.unsplash.com/photo-1589829545856-d10d557cf95f",
    "address": {
      "@type": "PostalAddress",
      "streetAddress": "350 Fifth Avenue, Suite 4200",
      "addressLocality": "New York",
      "addressRegion": "NY",
      "postalCode": "10118",
      "addressCountry": "US"
    },
    "telephone": "+1-212-555-0198",
    "email": "info@libertylegalgroup.com",
    "areaServed": "New York, USA",
    "priceRange": "$$"
  }
  </script>
</head>

<body>
  <header>
    <div class="container navbar">
      <a href="#" class="logo"><i class="fa-solid fa-scale-balanced"></i> Liberty Legal Group</a>
      <div class="menu-toggle"><i class="fa-solid fa-bars"></i></div>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#practice">Practice Areas</a></li>
        <li><a href="#attorneys">Attorneys</a></li>
        <li><a href="#results">Results</a></li>
        <li><a href="#faq">FAQ</a></li>
        <li><a href="#contact" class="btn btn-gold">Free Consultation</a></li>
      </ul>
    </div>
  </header>

  <section class="hero">
    <div class="container">
      <div class="hero-content">
        <div class="hero-badge"><i class="fa-solid fa-award"></i> New York Legal Excellence</div>
        <h1>Trusted Legal Representation When You Need It Most</h1>
        <p>Liberty Legal Group provides strategic, compassionate, and results-driven legal counsel for individuals, families, and businesses across New York.</p>
        <div class="hero-actions">
          <a href="#contact" class="btn btn-gold">Free Consultation <i class="fa-solid fa-arrow-right"></i></a>
          <a href="tel:+12125550198" class="btn btn-outline"><i class="fa-solid fa-phone"></i> Call Now</a>
        </div>

        <div class="hero-stats">
          <div class="hero-stat"><strong class="counter" data-target="20">0</strong><span>Years Experience</span></div>
          <div class="hero-stat"><strong class="counter" data-target="5000">0</strong><span>Clients Served</span></div>
          <div class="hero-stat"><strong class="counter" data-target="98">0</strong><span>Client Satisfaction</span></div>
        </div>
      </div>
    </div>
  </section>

  <section id="about" class="section">
    <div class="container about-grid reveal">
      <div class="about-img">
        <img src="https://images.unsplash.com/photo-1450101499163-c8848c66ca85?auto=format&fit=crop&w=1000&q=80" alt="Law firm office">
        <div class="about-card">
          <i class="fa-solid fa-gavel"></i>
          <h3>Premium Legal Counsel</h3>
          <p>Built on integrity, strategy, and client-first representation.</p>
        </div>
      </div>

      <div class="about-text">
        <h2>Experienced Attorneys. Personal Attention. Powerful Results.</h2>
        <p>Founded in New York, Liberty Legal Group has built a reputation for delivering professional, reliable, and personalized legal representation. Our firm combines deep legal knowledge with a modern client-focused approach.</p>
        <p>Our mission is simple: protect our clients, guide them with clarity, and fight for the best possible outcome in every matter.</p>

        <ul class="check-list">
          <li><i class="fa-solid fa-check"></i> Client-focused legal strategies</li>
          <li><i class="fa-solid fa-check"></i> Transparent communication</li>
          <li><i class="fa-solid fa-check"></i> Experienced trial and negotiation team</li>
          <li><i class="fa-solid fa-check"></i> Trusted by individuals, families, and businesses</li>
        </ul>

        <a href="#contact" class="btn btn-gold">Schedule a Consultation</a>
      </div>
    </div>
  </section>

  <section id="practice" class="section section-light">
    <div class="container">
      <div class="section-title reveal">
        <span>Practice Areas</span>
        <h2>Comprehensive Legal Services</h2>
        <p>Our attorneys handle a wide range of legal matters with professionalism, discretion, and strategic focus.</p>
      </div>

      <div class="practice-grid">
        <div class="practice-card reveal">
          <div class="icon-box"><i class="fa-solid fa-car-burst"></i></div>
          <h3>Personal Injury</h3>
          <p>Representation for accident victims seeking fair compensation for injuries, medical bills, and damages.</p>
          <a href="#contact" class="learn-link">Learn More <i class="fa-solid fa-arrow-right"></i></a>
        </div>

        <div class="practice-card reveal">
          <div class="icon-box"><i class="fa-solid fa-people-roof"></i></div>
          <h3>Family Law</h3>
          <p>Guidance for divorce, custody, support, and sensitive family matters with care and discretion.</p>
          <a href="#contact" class="learn-link">Learn More <i class="fa-solid fa-arrow-right"></i></a>
        </div>

        <div class="practice-card reveal">
          <div class="icon-box"><i class="fa-solid fa-shield-halved"></i></div>
          <h3>Criminal Defense</h3>
          <p>Strong defense strategies for clients facing criminal charges, investigations, or legal accusations.</p>
          <a href="#contact" class="learn-link">Learn More <i class="fa-solid fa-arrow-right"></i></a>
        </div>

        <div class="practice-card reveal">
          <div class="icon-box"><i class="fa-solid fa-passport"></i></div>
          <h3>Immigration Law</h3>
          <p>Legal help for visas, green cards, citizenship, family petitions, and immigration challenges.</p>
          <a href="#contact" class="learn-link">Learn More <i class="fa-solid fa-arrow-right"></i></a>
        </div>

        <div class="practice-card reveal">
          <div class="icon-box"><i class="fa-solid fa-briefcase"></i></div>
          <h3>Business Law</h3>
          <p>Legal support for contracts, disputes, business formation, compliance, and commercial litigation.</p>
          <a href="#contact" class="learn-link">Learn More <i class="fa-solid fa-arrow-right"></i></a>
        </div>

        <div class="practice-card reveal">
          <div class="icon-box"><i class="fa-solid fa-file-signature"></i></div>
          <h3>Estate Planning</h3>
          <p>Protect your family and assets with wills, trusts, probate guidance, and estate planning solutions.</p>
          <a href="#contact" class="learn-link">Learn More <i class="fa-solid fa-arrow-right"></i></a>
        </div>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="section-title reveal">
        <span>Why Choose Us</span>
        <h2>Legal Support You Can Trust</h2>
      </div>

      <div class="choose-grid">
        <div class="choose-card reveal"><div class="number">20+</div><h3>Years Experience</h3><p>Decades of legal insight.</p></div>
        <div class="choose-card reveal"><div class="number">5000+</div><h3>Clients Served</h3><p>Trusted by thousands.</p></div>
        <div class="choose-card reveal"><div class="number">Free</div><h3>Consultation</h3><p>Start with clarity.</p></div>
        <div class="choose-card reveal"><div class="number">24/7</div><h3>Support</h3><p>Here when needed.</p></div>
        <div class="choose-card reveal"><div class="number">Proven</div><h3>Results</h3><p>Focused on outcomes.</p></div>
      </div>
    </div>
  </section>

  <section id="attorneys" class="section section-light">
    <div class="container">
      <div class="section-title reveal">
        <span>Meet Our Attorneys</span>
        <h2>Experienced Legal Professionals</h2>
      </div>

      <div class="attorney-grid">
        <div class="attorney-card reveal">
          <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?auto=format&fit=crop&w=900&q=80" alt="Attorney Jonathan Miller">
          <div class="attorney-info">
            <h3>Jonathan Miller</h3>
            <div class="position">Managing Partner</div>
            <div class="attorney-meta"><strong>Experience:</strong> 22 years</div>
            <div class="attorney-meta"><strong>Education:</strong> Columbia Law School</div>
            <p>Jonathan leads the firm with extensive litigation experience and a strong record of protecting client interests in complex legal matters.</p>
          </div>
        </div>

        <div class="attorney-card reveal">
          <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&w=900&q=80" alt="Attorney Sarah Bennett">
          <div class="attorney-info">
            <h3>Sarah Bennett</h3>
            <div class="position">Senior Family Law Attorney</div>
            <div class="attorney-meta"><strong>Experience:</strong> 15 years</div>
            <div class="attorney-meta"><strong>Education:</strong> New York University School of Law</div>
            <p>Sarah is known for her compassionate approach and strong advocacy in divorce, custody, and family-related legal matters.</p>
          </div>
        </div>

        <div class="attorney-card reveal">
          <img src="https://images.unsplash.com/photo-1556157382-97eda2f9e2bf?auto=format&fit=crop&w=900&q=80" alt="Attorney Michael Carter">
          <div class="attorney-info">
            <h3>Michael Carter</h3>
            <div class="position">Criminal Defense Attorney</div>
            <div class="attorney-meta"><strong>Experience:</strong> 18 years</div>
            <div class="attorney-meta"><strong>Education:</strong> Fordham University School of Law</div>
            <p>Michael brings courtroom strength, strategic defense planning, and dedicated representation to clients facing criminal charges.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="results" class="section">
    <div class="container">
      <div class="section-title reveal">
        <span>Case Results</span>
        <h2>Professional Sample Results</h2>
        <p>Past results do not guarantee future outcomes. Each case is unique and depends on its specific facts.</p>
      </div>

      <div class="results-grid">
        <div class="result-card reveal">
          <div class="result-amount">$1.8M</div>
          <h3>Personal Injury Settlement</h3>
          <p>Successful settlement for a client injured in a serious vehicle accident.</p>
        </div>
        <div class="result-card reveal">
          <div class="result-amount">$750K</div>
          <h3>Business Litigation</h3>
          <p>Resolved a complex contract dispute for a growing New York business.</p>
        </div>
        <div class="result-card reveal">
          <div class="result-amount">Won</div>
          <h3>Family Law Case</h3>
          <p>Helped a parent secure a favorable custody arrangement.</p>
        </div>
        <div class="result-card reveal">
          <div class="result-amount">Approved</div>
          <h3>Immigration Approval</h3>
          <p>Assisted a family with a successful permanent residency application.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="section section-light">
    <div class="container">
      <div class="section-title reveal">
        <span>Testimonials</span>
        <h2>What Clients Say</h2>
      </div>

      <div class="testimonial-grid">
        <div class="testimonial-card reveal"><div class="stars">★★★★★</div><p>"The team was professional, responsive, and truly cared about my case."</p><div class="client">Emily Roberts</div></div>
        <div class="testimonial-card reveal"><div class="stars">★★★★★</div><p>"They explained everything clearly and helped me feel confident from day one."</p><div class="client">David Thompson</div></div>
        <div class="testimonial-card reveal"><div class="stars">★★★★★</div><p>"Excellent communication and outstanding legal guidance throughout the process."</p><div class="client">Michelle Carter</div></div>
        <div class="testimonial-card reveal"><div class="stars">★★★★★</div><p>"A reliable law firm with attorneys who genuinely fight for their clients."</p><div class="client">Anthony Williams</div></div>
        <div class="testimonial-card reveal"><div class="stars">★★★★★</div><p>"My consultation was helpful, honest, and gave me a clear path forward."</p><div class="client">Jessica Morgan</div></div>
        <div class="testimonial-card reveal"><div class="stars">★★★★★</div><p>"Professional, respectful, and highly knowledgeable. I highly recommend them."</p><div class="client">Robert Anderson</div></div>
      </div>
    </div>
  </section>

  <section id="faq" class="section">
    <div class="container">
      <div class="section-title reveal">
        <span>FAQ</span>
        <h2>Frequently Asked Questions</h2>
      </div>

      <div class="faq-wrap reveal">
        <div class="faq-item"><div class="faq-question">Do you offer free consultation? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">Yes. We offer a free initial consultation to understand your situation and explain your legal options.</div></div>
        <div class="faq-item"><div class="faq-question">How much does a lawyer cost? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">Costs depend on the type and complexity of the case. We explain fees clearly before representation begins.</div></div>
        <div class="faq-item"><div class="faq-question">How long does a lawsuit take? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">Timelines vary based on the facts, court schedule, negotiation progress, and complexity of the matter.</div></div>
        <div class="faq-item"><div class="faq-question">What should I bring to my first meeting? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">Bring relevant documents, contracts, court papers, photos, messages, police reports, or medical records.</div></div>
        <div class="faq-item"><div class="faq-question">Do you handle emergency legal matters? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">Yes. Our team provides responsive support for urgent legal situations whenever possible.</div></div>
        <div class="faq-item"><div class="faq-question">Can you represent clients outside New York? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">We primarily serve New York clients and can discuss whether your matter falls within our service area.</div></div>
        <div class="faq-item"><div class="faq-question">Will I work directly with an attorney? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">Yes. Our attorneys and legal team work closely with clients throughout the legal process.</div></div>
        <div class="faq-item"><div class="faq-question">How do I schedule a consultation? <i class="fa-solid fa-plus"></i></div><div class="faq-answer">You can call us, email us, or submit the contact form on this website.</div></div>
      </div>
    </div>
  </section>

  <section id="contact" class="section section-light">
    <div class="container">
      <div class="section-title reveal">
        <span>Contact Us</span>
        <h2>Schedule Your Free Consultation</h2>
      </div>

      <div class="contact-grid">
        <div class="contact-info reveal">
          <h3>Get In Touch</h3>
          <div class="contact-row"><i class="fa-solid fa-phone"></i><div><strong>Phone</strong><br>+1 (212) 555-0198</div></div>
          <div class="contact-row"><i class="fa-solid fa-envelope"></i><div><strong>Email</strong><br>info@libertylegalgroup.com</div></div>
          <div class="contact-row"><i class="fa-solid fa-location-dot"></i><div><strong>Office Address</strong><br>350 Fifth Avenue, Suite 4200<br>New York, NY 10118</div></div>
          <div class="contact-row"><i class="fa-solid fa-clock"></i><div><strong>Business Hours</strong><br>Monday - Friday: 8:00 AM - 6:00 PM<br>Saturday: By Appointment<br>Emergency Support: 24/7</div></div>
        </div>

        <div class="contact-form reveal">
          <h3>Request Consultation</h3>
          <form>
            <input type="text" placeholder="Full Name" required>
            <input type="email" placeholder="Email Address" required>
            <input type="tel" placeholder="Phone Number" required>
            <select required>
              <option value="">Select Practice Area</option>
              <option>Personal Injury</option>
              <option>Family Law</option>
              <option>Criminal Defense</option>
              <option>Immigration Law</option>
              <option>Business Law</option>
              <option>Estate Planning</option>
            </select>
            <textarea placeholder="Briefly describe your legal matter" required></textarea>
            <button type="submit" class="btn btn-gold">Submit Request <i class="fa-solid fa-paper-plane"></i></button>
          </form>
        </div>
      </div>

      <div class="map reveal">
        <iframe src="https://www.google.com/maps?q=350%20Fifth%20Avenue%20New%20York%20NY&output=embed" loading="lazy"></iframe>
      </div>
    </div>
  </section>

  <footer>
    <div class="container footer-grid">
      <div>
        <h3>Liberty Legal Group</h3>
        <p>Trusted legal representation for individuals, families, and businesses in New York.</p>
        <div class="socials">
          <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
          <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
          <a href="#"><i class="fa-brands fa-x-twitter"></i></a>
          <a href="#"><i class="fa-brands fa-instagram"></i></a>
        </div>
      </div>

      <div>
        <h4>Quick Links</h4>
        <ul>
          <li><a href="#about">About Us</a></li>
          <li><a href="#practice">Practice Areas</a></li>
          <li><a href="#attorneys">Attorneys</a></li>
          <li><a href="#results">Case Results</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>

      <div>
        <h4>Practice Areas</h4>
        <ul>
          <li>Personal Injury</li>
          <li>Family Law</li>
          <li>Criminal Defense</li>
          <li>Immigration Law</li>
          <li>Business Law</li>
          <li>Estate Planning</li>
        </ul>
      </div>

      <div>
        <h4>Contact Information</h4>
        <p>350 Fifth Avenue, Suite 4200<br>New York, NY 10118</p>
        <p>+1 (212) 555-0198</p>
        <p>info@libertylegalgroup.com</p>
      </div>
    </div>

    <div class="container copyright">
      <p>© 2026 Liberty Legal Group. All Rights Reserved. Attorney Advertising. Prior results do not guarantee a similar outcome.</p>
    </div>
  </footer>

  <a href="tel:+12125550198" class="sticky-call"><i class="fa-solid fa-phone"></i></a>
  <a href="#contact" class="sticky-consult">Free Consultation</a>
  <a href="#" class="back-top"><i class="fa-solid fa-arrow-up"></i></a>

  <script>
    const menuToggle = document.querySelector(".menu-toggle");
    const navLinks = document.querySelector(".nav-links");

    menuToggle.addEventListener("click", () => {
      navLinks.classList.toggle("active");
    });

    document.querySelectorAll(".nav-links a").forEach(link => {
      link.addEventListener("click", () => {
        navLinks.classList.remove("active");
      });
    });

    const revealElements = document.querySelectorAll(".reveal");

    function revealOnScroll() {
      revealElements.forEach(element => {
        const windowHeight = window.innerHeight;
        const elementTop = element.getBoundingClientRect().top;
        if (elementTop < windowHeight - 90) {
          element.classList.add("active");
        }
      });
    }

    window.addEventListener("scroll", revealOnScroll);
    revealOnScroll();

    const faqItems = document.querySelectorAll(".faq-item");

    faqItems.forEach(item => {
      item.querySelector(".faq-question").addEventListener("click", () => {
        item.classList.toggle("active");
        const icon = item.querySelector("i");
        icon.classList.toggle("fa-plus");
        icon.classList.toggle("fa-minus");
      });
    });

    const counters = document.querySelectorAll(".counter");
    let counterStarted = false;

    function startCounters() {
      if (counterStarted) return;

      const statsTop = document.querySelector(".hero-stats").getBoundingClientRect().top;
      if (statsTop < window.innerHeight) {
        counterStarted = true;

        counters.forEach(counter => {
          const target = +counter.dataset.target;
          let current = 0;
          const increment = target / 90;

          const updateCounter = () => {
            current += increment;
            if (current < target) {
              counter.textContent = Math.ceil(current);
              requestAnimationFrame(updateCounter);
            } else {
              counter.textContent = target + (target === 98 ? "%" : "+");
            }
          };

          updateCounter();
        });
      }
    }

    window.addEventListener("scroll", startCounters);
    startCounters();

    const backTop = document.querySelector(".back-top");

    window.addEventListener("scroll", () => {
      if (window.scrollY > 600) {
        backTop.classList.add("show");
      } else {
        backTop.classList.remove("show");
      }
    });

    document.querySelector("form").addEventListener("submit", function(e) {
      e.preventDefault();
      alert("Thank you. Your consultation request has been received.");
      this.reset();
    });
  </script>
</body>
</html>
