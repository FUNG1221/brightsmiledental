[index.html](https://github.com/user-attachments/files/29328678/index.html)
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
      --navy-darker: #040f24;
      --gold: #c8a24a;
      --gold-light: #e2c46f;
      --gold-dark: #8b6f47;
      --white: #ffffff;
      --gray: #f4f6f8;
      --gray-light: #fafbfc;
      --text: #1d2939;
      --text-light: #344054;
      --muted: #667085;
      --dark: #050d1c;
      --shadow: 0 18px 45px rgba(7, 27, 58, 0.15);
      --shadow-lg: 0 30px 60px rgba(7, 27, 58, 0.25);
      --shadow-sm: 0 8px 20px rgba(7, 27, 58, 0.08);
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
      background: linear-gradient(135deg, var(--gray-light) 0%, var(--gray) 100%);
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
      font-weight: 700;
    }

    .section-title p {
      max-width: 720px;
      margin: 16px auto 0;
      color: var(--muted);
      font-size: 16px;
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
      font-size: 15px;
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

    .btn-secondary {
      background: var(--navy);
      color: var(--white);
      box-shadow: 0 12px 30px rgba(7, 27, 58, 0.25);
    }

    .btn-secondary:hover {
      transform: translateY(-3px);
      box-shadow: 0 18px 40px rgba(7, 27, 58, 0.35);
      background: var(--navy-light);
    }

    /* Loading Animation */
    .loader-wrapper {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(135deg, var(--navy-darker) 0%, var(--navy) 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 9999;
      opacity: 1;
      transition: opacity 0.8s ease;
    }

    .loader-wrapper.hidden {
      opacity: 0;
      pointer-events: none;
    }

    .loader-content {
      text-align: center;
    }

    .loader-logo {
      color: var(--gold);
      font-size: 48px;
      margin-bottom: 24px;
      animation: logoFloat 1s ease-in-out infinite;
    }

    .loader-text {
      color: var(--white);
      font-family: "Cinzel", serif;
      font-size: 22px;
      margin-bottom: 32px;
      letter-spacing: 2px;
    }

    .loader-spinner {
      width: 50px;
      height: 50px;
      border: 3px solid rgba(200, 162, 74, 0.3);
      border-top-color: var(--gold);
      border-radius: 50%;
      animation: spin 1s linear infinite;
      margin: 0 auto;
    }

    @keyframes logoFloat {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    @keyframes spin {
      to { transform: rotate(360deg); }
    }

    /* Emergency Banner */
    .emergency-banner {
      background: linear-gradient(135deg, #dc2626 0%, #b91c1c 100%);
      color: var(--white);
      padding: 16px 0;
      position: sticky;
      top: 0;
      z-index: 998;
      box-shadow: 0 4px 15px rgba(220, 38, 38, 0.3);
    }

    .emergency-banner-content {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      font-weight: 600;
      font-size: 15px;
    }

    .emergency-banner i {
      font-size: 18px;
      animation: pulse-emergency 1.5s ease-in-out infinite;
    }

    @keyframes pulse-emergency {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.6; }
    }

    header {
      position: fixed;
      top: 48px;
      width: 100%;
      z-index: 997;
      background: rgba(7, 27, 58, 0.95);
      backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(200, 162, 74, 0.2);
      box-shadow: var(--shadow-sm);
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
      letter-spacing: 0.5px;
    }

    .logo i {
      color: var(--gold);
      font-size: 26px;
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
      position: relative;
    }

    .nav-links a::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 2px;
      background: var(--gold);
      transition: var(--transition);
    }

    .nav-links a:hover::after {
      width: 100%;
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
        linear-gradient(115deg, rgba(7,27,58,0.96), rgba(7,27,58,0.65)),
        url("https://images.unsplash.com/photo-1589829545856-d10d557cf95f?auto=format&fit=crop&w=1800&q=80") center/cover no-repeat;
      color: var(--white);
      display: flex;
      align-items: center;
      padding-top: 90px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: radial-gradient(circle at 20% 50%, rgba(200, 162, 74, 0.08) 0%, transparent 50%);
      pointer-events: none;
    }

    .hero-content {
      max-width: 780px;
      animation: fadeUp 1s ease forwards;
      position: relative;
      z-index: 1;
    }

    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      background: rgba(200, 162, 74, 0.15);
      border: 1px solid rgba(200, 162, 74, 0.4);
      padding: 12px 20px;
      border-radius: 999px;
      color: var(--gold-light);
      font-weight: 700;
      margin-bottom: 24px;
      font-size: 14px;
    }

    .hero h1 {
      font-family: "Cinzel", serif;
      font-size: clamp(42px, 7vw, 78px);
      line-height: 1.05;
      margin-bottom: 24px;
      font-weight: 700;
      letter-spacing: -0.5px;
    }

    .hero p {
      font-size: 19px;
      max-width: 680px;
      color: rgba(255,255,255,0.88);
      margin-bottom: 34px;
      line-height: 1.6;
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
      background: rgba(255,255,255,0.08);
      border: 1px solid rgba(200, 162, 74, 0.25);
      padding: 24px;
      border-radius: var(--radius);
      backdrop-filter: blur(20px);
      transition: var(--transition);
    }

    .hero-stat:hover {
      background: rgba(255,255,255,0.12);
      border-color: rgba(200, 162, 74, 0.4);
    }

    .hero-stat strong {
      display: block;
      color: var(--gold-light);
      font-size: 32px;
      font-family: "Cinzel", serif;
      margin-bottom: 4px;
    }

    .hero-stat span {
      font-size: 14px;
      color: rgba(255, 255, 255, 0.7);
      font-weight: 600;
    }

    /* Trust Badges */
    .trust-badges {
      margin-top: 50px;
      display: flex;
      gap: 24px;
      flex-wrap: wrap;
      align-items: center;
    }

    .trust-badge {
      display: flex;
      align-items: center;
      gap: 10px;
      background: rgba(255,255,255,0.08);
      border: 1px solid rgba(200, 162, 74, 0.25);
      padding: 12px 18px;
      border-radius: 12px;
      font-size: 13px;
      color: rgba(255, 255, 255, 0.8);
    }

    .trust-badge i {
      color: var(--gold);
      font-size: 16px;
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
      box-shadow: var(--shadow-lg);
      border: 1px solid rgba(200, 162, 74, 0.15);
    }

    .about-card {
      position: absolute;
      bottom: -30px;
      right: -25px;
      background: linear-gradient(135deg, var(--navy) 0%, var(--navy-light) 100%);
      color: var(--white);
      padding: 28px;
      border-radius: 20px;
      max-width: 260px;
      box-shadow: var(--shadow-lg);
      border: 1px solid rgba(200, 162, 74, 0.2);
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
      font-weight: 700;
    }

    .about-text p {
      color: var(--muted);
      margin-bottom: 18px;
      line-height: 1.8;
    }

    .check-list {
      list-style: none;
      margin: 25px 0;
    }

    .check-list li {
      margin-bottom: 12px;
      font-weight: 600;
      color: var(--text-light);
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .check-list i {
      color: var(--gold);
      font-size: 18px;
      flex-shrink: 0;
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
      box-shadow: var(--shadow-lg);
      border-color: rgba(200, 162, 74, 0.2);
    }

    .icon-box {
      width: 66px;
      height: 66px;
      border-radius: 18px;
      background: linear-gradient(135deg, rgba(200,162,74,0.2), rgba(200,162,74,0.08));
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
      font-weight: 700;
    }

    .practice-card p,
    .choose-card p,
    .result-card p {
      color: var(--muted);
      margin-bottom: 20px;
      line-height: 1.6;
    }

    .learn-link {
      color: var(--navy);
      font-weight: 800;
      display: inline-flex;
      gap: 8px;
      align-items: center;
      transition: var(--transition);
    }

    .learn-link:hover {
      color: var(--gold);
      gap: 12px;
    }

    .choose-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 22px;
    }

    .choose-card {
      text-align: center;
      padding: 28px 20px;
      background: linear-gradient(135deg, var(--white) 0%, var(--gray-light) 100%);
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
      cursor: pointer;
      position: relative;
    }

    .attorney-card img {
      height: 340px;
      width: 100%;
      object-fit: cover;
      transition: var(--transition);
    }

    .attorney-card:hover img {
      transform: scale(1.05);
    }

    .attorney-overlay {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      background: linear-gradient(to top, rgba(7,27,58,0.95), transparent);
      padding: 30px;
      color: var(--white);
      height: 50%;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      transition: var(--transition);
    }

    .attorney-info {
      padding: 30px;
      background: var(--white);
    }

    .attorney-info h3 {
      color: var(--navy);
      font-size: 24px;
      margin-bottom: 5px;
      font-weight: 700;
    }

    .position {
      color: var(--gold);
      font-weight: 800;
      margin-bottom: 15px;
      font-size: 14px;
    }

    .attorney-meta {
      color: var(--muted);
      font-size: 14px;
      margin-bottom: 12px;
    }

    .attorney-card .view-btn {
      color: var(--gold);
      font-weight: 800;
      font-size: 13px;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      margin-top: 12px;
      transition: var(--transition);
    }

    .attorney-card .view-btn:hover {
      gap: 10px;
      color: var(--gold-light);
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
      font-size: 16px;
    }

    .testimonial-card p {
      color: var(--muted);
      margin-bottom: 22px;
      font-style: italic;
      line-height: 1.7;
    }

    .client {
      color: var(--navy);
      font-weight: 800;
      font-size: 15px;
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
      border: 1px solid rgba(7,27,58,0.08);
      transition: var(--transition);
    }

    .faq-item:hover {
      box-shadow: var(--shadow-lg);
      border-color: rgba(200, 162, 74, 0.2);
    }

    .faq-question {
      padding: 22px 26px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      cursor: pointer;
      font-weight: 800;
      color: var(--navy);
      transition: var(--transition);
    }

    .faq-question:hover {
      color: var(--gold);
    }

    .faq-answer {
      max-height: 0;
      overflow: hidden;
      transition: var(--transition);
      color: var(--muted);
      padding: 0 26px;
      line-height: 1.7;
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
      border: 1px solid rgba(7,27,58,0.08);
    }

    .contact-info h3,
    .contact-form h3 {
      color: var(--navy);
      font-size: 28px;
      margin-bottom: 24px;
      font-family: "Cinzel", serif;
      font-weight: 700;
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
      flex-shrink: 0;
    }

    .contact-row div {
      flex: 1;
    }

    .contact-row strong {
      color: var(--text);
      font-weight: 700;
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
      font-size: 15px;
    }

    form input:focus,
    form select:focus,
    form textarea:focus {
      border-color: var(--gold);
      box-shadow: 0 0 0 4px rgba(200,162,74,0.14);
      background: rgba(200,162,74,0.02);
    }

    form input::placeholder,
    form select::placeholder,
    form textarea::placeholder {
      color: #999;
    }

    .form-group {
      position: relative;
    }

    .error-message {
      color: #dc2626;
      font-size: 13px;
      margin-top: -12px;
      margin-bottom: 12px;
      display: none;
      font-weight: 600;
    }

    .form-group.error input,
    .form-group.error select,
    .form-group.error textarea {
      border-color: #dc2626;
      background: rgba(220, 38, 38, 0.03);
    }

    .form-group.error .error-message {
      display: block;
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

    /* Success Message */
    .success-message {
      position: fixed;
      top: 130px;
      right: 20px;
      background: linear-gradient(135deg, #10b981 0%, #059669 100%);
      color: var(--white);
      padding: 18px 24px;
      border-radius: 12px;
      box-shadow: var(--shadow-lg);
      display: none;
      align-items: center;
      gap: 12px;
      z-index: 10000;
      animation: slideIn 0.4s ease;
      border: 1px solid rgba(16, 185, 129, 0.3);
    }

    .success-message.show {
      display: flex;
    }

    .success-message i {
      font-size: 20px;
    }

    .success-message-text {
      flex: 1;
      font-weight: 600;
    }

    .success-message-close {
      cursor: pointer;
      font-size: 18px;
      opacity: 0.8;
      transition: var(--transition);
    }

    .success-message-close:hover {
      opacity: 1;
    }

    @keyframes slideIn {
      from {
        transform: translateX(400px);
        opacity: 0;
      }
      to {
        transform: translateX(0);
        opacity: 1;
      }
    }

    /* Modal */
    .modal {
      display: none;
      position: fixed;
      z-index: 10001;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.6);
      backdrop-filter: blur(4px);
      overflow-y: auto;
      animation: fadeIn 0.3s ease;
    }

    .modal.show {
      display: flex;
      align-items: center;
      justify-content: center;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    .modal-content {
      background: var(--white);
      border-radius: 24px;
      max-width: 700px;
      width: 90%;
      box-shadow: var(--shadow-lg);
      overflow: hidden;
      animation: slideUp 0.3s ease;
      max-height: 90vh;
      overflow-y: auto;
    }

    @keyframes slideUp {
      from {
        transform: translateY(50px);
        opacity: 0;
      }
      to {
        transform: translateY(0);
        opacity: 1;
      }
    }

    .modal-header {
      position: relative;
      height: 320px;
      overflow: hidden;
    }

    .modal-header img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .modal-close {
      position: absolute;
      top: 20px;
      right: 20px;
      width: 40px;
      height: 40px;
      background: var(--white);
      border: none;
      border-radius: 50%;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--navy);
      font-size: 20px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
      transition: var(--transition);
    }

    .modal-close:hover {
      background: var(--gold);
      color: var(--white);
    }

    .modal-body {
      padding: 40px;
    }

    .modal-body h2 {
      font-family: "Cinzel", serif;
      color: var(--navy);
      font-size: 32px;
      margin-bottom: 8px;
      font-weight: 700;
    }

    .modal-position {
      color: var(--gold);
      font-weight: 800;
      margin-bottom: 20px;
      font-size: 15px;
    }

    .modal-meta {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      margin-bottom: 28px;
      padding-bottom: 28px;
      border-bottom: 1px solid rgba(7,27,58,0.08);
    }

    .modal-meta-item {
      display: flex;
      flex-direction: column;
    }

    .modal-meta-item label {
      color: var(--muted);
      font-size: 13px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.5px;
      margin-bottom: 6px;
    }

    .modal-meta-item value {
      color: var(--text);
      font-size: 16px;
      font-weight: 700;
    }

    .modal-body p {
      color: var(--muted);
      line-height: 1.8;
      margin-bottom: 16px;
    }

    .modal-body ul {
      list-style: none;
      margin-bottom: 28px;
    }

    .modal-body ul li {
      color: var(--muted);
      margin-bottom: 12px;
      padding-left: 24px;
      position: relative;
      line-height: 1.6;
    }

    .modal-body ul li::before {
      content: '✓';
      position: absolute;
      left: 0;
      color: var(--gold);
      font-weight: 800;
    }

    .modal-actions {
      display: flex;
      gap: 12px;
      margin-top: 28px;
    }

    .modal-actions .btn {
      flex: 1;
    }

    footer {
      background: linear-gradient(135deg, var(--dark) 0%, var(--navy-darker) 100%);
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
      font-weight: 700;
    }

    footer h3 {
      font-family: "Cinzel", serif;
      font-size: 25px;
      letter-spacing: 0.5px;
    }

    footer ul {
      list-style: none;
    }

    footer li {
      margin-bottom: 10px;
      transition: var(--transition);
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
      background: rgba(200, 162, 74, 0.15);
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      transition: var(--transition);
      color: var(--gold);
      border: 1px solid rgba(200, 162, 74, 0.3);
    }

    .socials a:hover {
      background: var(--gold);
      color: var(--white);
      transform: translateY(-4px);
    }

    .copyright {
      border-top: 1px solid rgba(255,255,255,0.12);
      padding-top: 24px;
      text-align: center;
      color: rgba(255,255,255,0.58);
      font-size: 14px;
    }

    .sticky-call,
    .sticky-consult,
    .back-top {
      position: fixed;
      z-index: 996;
      border-radius: 999px;
      box-shadow: var(--shadow-lg);
    }

    .sticky-call {
      left: 22px;
      bottom: 22px;
      width: 58px;
      height: 58px;
      background: linear-gradient(135deg, var(--gold), var(--gold-light));
      color: var(--navy);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 24px;
      animation: pulse 1.8s infinite;
      border: 2px solid var(--white);
    }

    .sticky-consult {
      right: 22px;
      bottom: 22px;
      background: linear-gradient(135deg, var(--navy), var(--navy-light));
      color: var(--white);
      padding: 15px 22px;
      font-weight: 800;
      font-size: 14px;
      border: 1px solid rgba(200, 162, 74, 0.3);
      transition: var(--transition);
    }

    .sticky-consult:hover {
      transform: translateY(-3px);
      box-shadow: 0 20px 40px rgba(7, 27, 58, 0.35);
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
      border: 2px solid var(--gold);
      transition: var(--transition);
    }

    .back-top:hover {
      background: var(--gold);
      color: var(--white);
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
        bottom: -20px;
      }

      header {
        top: 48px;
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
        padding: 60px 0;
      }

      .sticky-consult {
        display: none;
      }

      .trust-badges {
        gap: 12px;
      }

      .trust-badge {
        padding: 10px 14px;
        font-size: 12px;
      }

      .hero-stats {
        gap: 16px;
        max-width: 100%;
      }

      .hero-stat {
        padding: 16px;
      }

      .hero-stat strong {
        font-size: 24px;
      }

      .modal-content {
        width: 95%;
        max-height: 85vh;
      }

      .modal-body {
        padding: 24px;
      }

      .modal-body h2 {
        font-size: 24px;
      }

      .contact-row {
        gap: 12px;
      }

      .contact-row i {
        font-size: 18px;
      }

      .footer-grid {
        gap: 25px;
      }
    }

    @media (max-width: 480px) {
      .hero-actions {
        flex-direction: column;
        gap: 12px;
      }

      .hero-actions .btn {
        width: 100%;
      }

      .btn {
        padding: 13px 20px;
        font-size: 14px;
      }

      .hero p {
        font-size: 16px;
      }

      .about-card {
        position: static;
        margin-top: 30px;
        max-width: 100%;
      }

      .hero-stat {
        padding: 12px;
      }

      .hero-stat strong {
        font-size: 20px;
      }

      .icon-box {
        width: 56px;
        height: 56px;
        font-size: 24px;
      }

      .practice-card,
      .attorney-card,
      .result-card,
      .testimonial-card,
      .choose-card,
      .contact-info,
      .contact-form {
        padding: 20px;
      }

      .modal-header {
        height: 240px;
      }

      .emergency-banner-content {
        font-size: 13px;
        gap: 10px;
      }

      .success-message {
        right: 10px;
        left: 10px;
        width: auto;
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
  <!-- Loading Animation -->
  <div class="loader-wrapper" id="loaderWrapper">
    <div class="loader-content">
      <div class="loader-logo"><i class="fa-solid fa-scale-balanced"></i></div>
      <div class="loader-text">Liberty Legal Group</div>
      <div class="loader-spinner"></div>
    </div>
  </div>

  <!-- Emergency Banner -->
  <div class="emergency-banner">
    <div class="container">
      <div class="emergency-banner-content">
        <i class="fa-solid fa-phone"></i>
        <span>Emergency Legal Matter? Call us 24/7 at <strong>+1 (212) 555-0198</strong></span>
      </div>
    </div>
  </div>

  <!-- Success Message -->
  <div class="success-message" id="successMessage">
    <i class="fa-solid fa-check-circle"></i>
    <div class="success-message-text" id="successText">Consultation request submitted successfully!</div>
    <span class="success-message-close" onclick="closeSuccessMessage()">×</span>
  </div>

  <!-- Attorney Modal -->
  <div class="modal" id="attorneyModal">
    <div class="modal-content">
      <div class="modal-header">
        <img id="modalImage" src="" alt="Attorney">
        <button class="modal-close" onclick="closeModal()"><i class="fa-solid fa-times"></i></button>
      </div>
      <div class="modal-body">
        <h2 id="modalName"></h2>
        <div class="modal-position" id="modalPosition"></div>
        
        <div class="modal-meta">
          <div class="modal-meta-item">
            <label>Experience</label>
            <value id="modalExperience"></value>
          </div>
          <div class="modal-meta-item">
            <label>Education</label>
            <value id="modalEducation"></value>
          </div>
        </div>

        <div id="modalDescription"></div>

        <ul id="modalSpecialties">
          <li>Client-focused representation</li>
          <li>Strategic case planning</li>
          <li>Proven track record</li>
        </ul>

        <div class="modal-actions">
          <a href="#contact" class="btn btn-gold" onclick="closeModal()">Schedule Consultation</a>
          <a href="tel:+12125550198" class="btn btn-secondary" onclick="closeModal()">Call Now</a>
        </div>
      </div>
    </div>
  </div>

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

        <div class="trust-badges">
          <div class="trust-badge"><i class="fa-solid fa-shield-check"></i> ABA Certified</div>
          <div class="trust-badge"><i class="fa-solid fa-star"></i> 4.9/5 Rating</div>
          <div class="trust-badge"><i class="fa-solid fa-medal"></i> Award Winning</div>
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
        <div class="attorney-card reveal" onclick="openModal(attorneyData[0])">
          <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?auto=format&fit=crop&w=900&q=80" alt="Attorney Jonathan Miller">
          <div class="attorney-info">
            <h3>Jonathan Miller</h3>
            <div class="position">Managing Partner</div>
            <div class="attorney-meta"><strong>Experience:</strong> 22 years</div>
            <div class="attorney-meta"><strong>Education:</strong> Columbia Law School</div>
            <p style="margin-bottom: 0;">Jonathan leads the firm with extensive litigation experience and a strong record of protecting client interests in complex legal matters.</p>
            <div class="attorney-card view-btn"><i class="fa-solid fa-arrow-right"></i> View Profile</div>
          </div>
        </div>

        <div class="attorney-card reveal" onclick="openModal(attorneyData[1])">
          <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&w=900&q=80" alt="Attorney Sarah Bennett">
          <div class="attorney-info">
            <h3>Sarah Bennett</h3>
            <div class="position">Senior Family Law Attorney</div>
            <div class="attorney-meta"><strong>Experience:</strong> 15 years</div>
            <div class="attorney-meta"><strong>Education:</strong> New York University School of Law</div>
            <p style="margin-bottom: 0;">Sarah is known for her compassionate approach and strong advocacy in divorce, custody, and family-related legal matters.</p>
            <div class="attorney-card view-btn"><i class="fa-solid fa-arrow-right"></i> View Profile</div>
          </div>
        </div>

        <div class="attorney-card reveal" onclick="openModal(attorneyData[2])">
          <img src="https://images.unsplash.com/photo-1556157382-97eda2f9e2bf?auto=format&fit=crop&w=900&q=80" alt="Attorney Michael Carter">
          <div class="attorney-info">
            <h3>Michael Carter</h3>
            <div class="position">Criminal Defense Attorney</div>
            <div class="attorney-meta"><strong>Experience:</strong> 18 years</div>
            <div class="attorney-meta"><strong>Education:</strong> Fordham University School of Law</div>
            <p style="margin-bottom: 0;">Michael brings courtroom strength, strategic defense planning, and dedicated representation to clients facing criminal charges.</p>
            <div class="attorney-card view-btn"><i class="fa-solid fa-arrow-right"></i> View Profile</div>
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
          <form id="contactForm">
            <div class="form-group">
              <input type="text" id="fullName" placeholder="Full Name" required>
              <div class="error-message">Please enter your full name</div>
            </div>
            
            <div class="form-group">
              <input type="email" id="email" placeholder="Email Address" required>
              <div class="error-message">Please enter a valid email address</div>
            </div>
            
            <div class="form-group">
              <input type="tel" id="phone" placeholder="Phone Number" required>
              <div class="error-message">Please enter a valid phone number</div>
            </div>
            
            <div class="form-group">
              <select id="practiceArea" required>
                <option value="">Select Practice Area</option>
                <option>Personal Injury</option>
                <option>Family Law</option>
                <option>Criminal Defense</option>
                <option>Immigration Law</option>
                <option>Business Law</option>
                <option>Estate Planning</option>
              </select>
              <div class="error-message">Please select a practice area</div>
            </div>
            
            <div class="form-group">
              <textarea id="message" placeholder="Briefly describe your legal matter" required></textarea>
              <div class="error-message">Please describe your legal matter</div>
            </div>
            
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
    // Attorney Data
    const attorneyData = [
      {
        name: "Jonathan Miller",
        position: "Managing Partner",
        experience: "22 years",
        education: "Columbia Law School",
        image: "https://images.unsplash.com/photo-1560250097-0b93528c311a?auto=format&fit=crop&w=900&q=80",
        description: "Jonathan leads the firm with extensive litigation experience and a strong record of protecting client interests in complex legal matters. He specializes in high-stakes commercial litigation and has successfully handled cases across multiple practice areas.",
        specialties: [
          "Commercial Litigation",
          "Complex Business Disputes",
          "Legal Strategy & Consultation",
          "Trial Representation",
          "Client Advocacy"
        ]
      },
      {
        name: "Sarah Bennett",
        position: "Senior Family Law Attorney",
        experience: "15 years",
        education: "New York University School of Law",
        image: "https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&w=900&q=80",
        description: "Sarah is known for her compassionate approach and strong advocacy in divorce, custody, and family-related legal matters. With over 15 years of experience, she helps families navigate complex situations with care and expertise.",
        specialties: [
          "Divorce & Separation",
          "Child Custody Cases",
          "Family Law Mediation",
          "Spousal Support",
          "Family Planning"
        ]
      },
      {
        name: "Michael Carter",
        position: "Criminal Defense Attorney",
        experience: "18 years",
        education: "Fordham University School of Law",
        image: "https://images.unsplash.com/photo-1556157382-97eda2f9e2bf?auto=format&fit=crop&w=900&q=80",
        description: "Michael brings courtroom strength, strategic defense planning, and dedicated representation to clients facing criminal charges. He has an impressive track record of achieving favorable outcomes in both state and federal cases.",
        specialties: [
          "Criminal Defense",
          "DUI/DWI Cases",
          "White Collar Crime",
          "Felony Defense",
          "Appeals & Post-Conviction"
        ]
      }
    ];

    // Loading Animation
    window.addEventListener('load', function() {
      setTimeout(function() {
        document.getElementById('loaderWrapper').classList.add('hidden');
      }, 1200);
    });

    // Menu Toggle
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

    // Reveal on Scroll
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

    // FAQ Accordion
    const faqItems = document.querySelectorAll(".faq-item");

    faqItems.forEach(item => {
      item.querySelector(".faq-question").addEventListener("click", () => {
        item.classList.toggle("active");
        const icon = item.querySelector("i");
        icon.classList.toggle("fa-plus");
        icon.classList.toggle("fa-minus");
      });
    });

    // Counter Animation
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

    // Back to Top Button
    const backTop = document.querySelector(".back-top");

    window.addEventListener("scroll", () => {
      if (window.scrollY > 600) {
        backTop.classList.add("show");
      } else {
        backTop.classList.remove("show");
      }
    });

    backTop.addEventListener("click", (e) => {
      e.preventDefault();
      window.scrollTo({ top: 0, behavior: "smooth" });
    });

    // Attorney Modal
    function openModal(attorney) {
      const modal = document.getElementById('attorneyModal');
      document.getElementById('modalImage').src = attorney.image;
      document.getElementById('modalName').textContent = attorney.name;
      document.getElementById('modalPosition').textContent = attorney.position;
      document.getElementById('modalExperience').textContent = attorney.experience;
      document.getElementById('modalEducation').textContent = attorney.education;
      document.getElementById('modalDescription').innerHTML = '<p>' + attorney.description + '</p>';
      
      const specialtiesList = document.getElementById('modalSpecialties');
      specialtiesList.innerHTML = '';
      attorney.specialties.forEach(specialty => {
        const li = document.createElement('li');
        li.textContent = specialty;
        specialtiesList.appendChild(li);
      });
      
      modal.classList.add('show');
      document.body.style.overflow = 'hidden';
    }

    function closeModal() {
      const modal = document.getElementById('attorneyModal');
      modal.classList.remove('show');
      document.body.style.overflow = 'auto';
    }

    window.addEventListener('click', function(event) {
      const modal = document.getElementById('attorneyModal');
      if (event.target === modal) {
        closeModal();
      }
    });

    // Form Validation
    const form = document.getElementById('contactForm');
    const formInputs = {
      fullName: document.getElementById('fullName'),
      email: document.getElementById('email'),
      phone: document.getElementById('phone'),
      practiceArea: document.getElementById('practiceArea'),
      message: document.getElementById('message')
    };

    function validateEmail(email) {
      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      return emailRegex.test(email);
    }

    function validatePhone(phone) {
      const phoneRegex = /^[\d\s\-\+\(\)]+$/;
      return phoneRegex.test(phone) && phone.replace(/\D/g, '').length >= 10;
    }

    function showError(fieldName) {
      const input = formInputs[fieldName];
      const formGroup = input.closest('.form-group');
      formGroup.classList.add('error');
    }

    function clearError(fieldName) {
      const input = formInputs[fieldName];
      const formGroup = input.closest('.form-group');
      formGroup.classList.remove('error');
    }

    Object.keys(formInputs).forEach(fieldName => {
      formInputs[fieldName].addEventListener('focus', () => {
        clearError(fieldName);
      });
    });

    form.addEventListener("submit", function(e) {
      e.preventDefault();
      let isValid = true;

      // Validate Full Name
      if (!formInputs.fullName.value.trim()) {
        showError('fullName');
        isValid = false;
      }

      // Validate Email
      if (!validateEmail(formInputs.email.value)) {
        showError('email');
        isValid = false;
      }

      // Validate Phone
      if (!validatePhone(formInputs.phone.value)) {
        showError('phone');
        isValid = false;
      }

      // Validate Practice Area
      if (!formInputs.practiceArea.value) {
        showError('practiceArea');
        isValid = false;
      }

      // Validate Message
      if (!formInputs.message.value.trim()) {
        showError('message');
        isValid = false;
      }

      if (isValid) {
        // Show success message
        showSuccessMessage("Thank you! Your consultation request has been received. We will contact you within 24 hours.");
        form.reset();
        
        // Optional: Clear any error states
        Object.keys(formInputs).forEach(fieldName => {
          clearError(fieldName);
        });
      }
    });

    function showSuccessMessage(message) {
      const successMessage = document.getElementById('successMessage');
      document.getElementById('successText').textContent = message;
      successMessage.classList.add('show');
      
      setTimeout(() => {
        successMessage.classList.remove('show');
      }, 5000);
    }

    function closeSuccessMessage() {
      const successMessage = document.getElementById('successMessage');
      successMessage.classList.remove('show');
    }
  </script>
</body>
</html>
