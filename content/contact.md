+++
title = ""
+++

<div class="guide-page">
  
  <style>
    @import url("https://fonts.googleapis.com/css2?family=Archivo+Black&family=Inter:wght@400;700;900&family=Assistant:wght@400;600;800&display=swap");

    :root {
      --accent: #c8ff2f;
      --dark: #080808;
      --card-bg: #141414;
      --text-main: #ffffff;
      --text-muted: #cccccc;
    }

    .guide-page {
      background: var(--dark);
      color: var(--text-main);
      font-family: 'Assistant', 'Inter', sans-serif;
      padding: 40px 15px;
      line-height: 1.4;
      max-width: 100%;
      border-radius: 40px;
      text-align: center;
      overflow-x: hidden; /* מונע גלילה לצדדים במובייל */
    }

    h1.guide-title {
      font-family: 'Archivo Black', sans-serif;
      font-size: clamp(2.5rem, 8vw, 4rem);
      color:var(--text-main)
      text-transform: uppercase;
      margin-bottom: 20px;
      line-height: 1;
    }

    .contact-container {
      max-width: 900px;
      margin: 0 auto;
    }

    /* פונט גדול לתיאור עם התאמה למובייל */
    .contact-description p {
      font-size: clamp(1.5rem, 4vw, 2.5rem);
      font-weight: 600;
      margin-bottom: 20px;
      word-wrap: break-word;
    }

    .contact-card {
      background: var(--card-bg);
      border-radius: 24px;
      padding: clamp(20px, 5vw, 40px);
      border: 1px solid #333;
      margin: 30px auto;
      display: block;
      width: 100%;
      max-width: 600px;
      text-align: left;
      box-sizing: border-box;
    }

    .contact-item {
      margin-bottom: 25px;
      /* גודל לינקים מותאם */
      font-size: clamp(1.2rem, 3.5vw, 2.2rem);
      word-break: break-all; /* מונע מהמייל הארוך לצאת מהמסך במובייל */
    }

    .contact-item label {
      display: block;
      color: var(--accent);
      font-weight: 800;
      text-transform: uppercase;
      font-size: clamp(1.1rem, 3vw, 1.9rem);
      margin-bottom: 8px;
    }

    .contact-item a {
      color: var(--text-main);
      text-decoration: none;
      font-weight: 700;
    }

    /* כפתור גוגל פורמס - גמיש למובייל */
    .form-btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      background: var(--accent);
      color: #000;
      padding: 15px 30px;
      border-radius: 999px;
      font-weight: 900;
      /* גודל פונט בכפתור משתנה */
      font-size: clamp(1.3rem, 4vw, 2.3rem);
      text-decoration: none;
      transition: all 0.3s ease;
      box-shadow: 0 10px 30px rgba(200, 255, 47, 0.2);
      max-width: 100%;
      box-sizing: border-box;
    }

    .form-btn:hover {
      transform: translateY(-3px);
      box-shadow: 0 15px 40px rgba(200, 255, 47, 0.4);
    }

    .or-divider {
      font-size: clamp(1.5rem, 4vw, 2rem);
      margin: 30px 0;
      color: #444;
      font-weight: 800;
    }

    [dir="rtl"] .contact-card {
      text-align: right;
    }

    /* תיקונים ספציפיים למסכים קטנים מאוד */
    @media (max-width: 480px) {
      .guide-page {
        padding: 30px 10px;
        border-radius: 20px;
      }
      .contact-item {
        margin-bottom: 15px;
      }
    }

  </style>

  <div class="contact-container">
    <h1 class="guide-title">Get in Touch</h1>
    <div class="contact-description">
      <p>For questions, technical support, or reservations, please reach out to us.</p>
      <p dir="rtl">לשאלות, תמיכה טכנית והזמנות - אנא צרו קשר איתנו.</p>
    </div>
    <a href="YOUR_GOOGLE_FORM_URL_HERE" target="_blank" class="form-btn">
      📩 Open Support Form / פתח טופס
    </a>
    <div class="or-divider">OR / או</div>
    <div class="contact-card">
      <div class="contact-item">
        <label>Email / אימייל</label>
        <a href="mailto:contact.ora001@gmail.com">contact.ora001@gmail.com</a>
      </div>
      <div class="contact-item">
        <label>Website / אתר</label>
        <a href="https://ora-guide.pages.dev">ora-guide.pages.dev</a>
      </div>
    </div>
  </div>

</div>

<!-- +++
title = ""
+++

<div class="guide-page">

  <style>
    @import url("https://fonts.googleapis.com/css2?family=Archivo+Black&family=Inter:wght@400;700;900&family=Assistant:wght@400;600;800&display=swap");

    :root {
      --accent: #c8ff2f;
      --dark: #080808;
      --card-bg: #141414;
      --text-main: #ffffff;
      --text-muted: #cccccc;
    }

    .guide-page {
      background: var(--dark);
      color: var(--text-main);
      font-family: 'Assistant', 'Inter', sans-serif;
      padding: 60px 20px;
      line-height: 1.5;
      max-width: 100%;
      border-radius: 50px;
      text-align: center;
    }

    h1.guide-title {
      font-family: 'Archivo Black', sans-serif;
      font-size: clamp(3.5rem, 5vw, 4rem);
      text-transform: uppercase;
      margin-bottom: 20px;
      color: var(--text-main);
    }

    .contact-container {
      max-width: 800px;
      margin: 0 auto;
    }
    .contact-container p{

font-size:2.5rem; }

    .contact-description {
      font-size: 1.4rem;
      color: var(--text-muted);
      margin-bottom: 40px;
    }

    .contact-card {
      background: var(--card-bg);
      border-radius: 24px;
      padding: 40px;
      border: 1px solid #333;
      margin-bottom: 40px;
      display: inline-block;
      width: 100%;
      max-width: 500px;
      text-align: left;
    }

    .contact-item {
      margin-bottom: 20px;
      font-size: 2.2rem;
    }

    .contact-item label {
      display: block;
      color: var(--accent);
      font-weight: 700;
      text-transform: uppercase;
      font-size: 1.9rem;
      margin-bottom: 5px;
    }

    .contact-item a {
      color: var(--text-main);
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }

    .contact-item a:hover {
      color: var(--accent);
    }

    /* Google Forms Button */
    .form-btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      background: var(--accent);
      color: #000;
      padding: 18px 40px;
      border-radius: 999px;
      font-weight: 800;
      font-size: 2.3rem;
      text-decoration: none;
      transition: all 0.3s ease;
      box-shadow: 0 10px 30px rgba(200, 255, 47, 0.2);
      margin-top: 20px;
    }

    .form-btn:hover {
      transform: translateY(-3px);
      box-shadow: 0 15px 40px rgba(200, 255, 47, 0.4);
      background: #d4ff5e;
    }

    .form-btn:active {
      transform: translateY(1px);
    }

    [dir="rtl"] .contact-card {
      text-align: right;
    }

  </style>

  <div class="contact-container" style="font-size:2.5">
    <h1 class="guide-title">Get in Touch</h1>
    <div class="contact-description">
      <p style="font-size:2.5">For questions, technical support, or reservations, please reach out to us.</p>
      <p dir="rtl">לשאלות, תמיכה טכנית והזמנות - אנא צרו קשר איתנו.</p>
    </div>
    <a href="YOUR_GOOGLE_FORM_URL_HERE" target="_blank" class="form-btn">
      📩 Open Support Form / פתח טופס פנייה
    </a>
    <div style="font-size:2rem margin: 40px 0; color: #333;">OR / או</div>
    <div class="contact-card">
      <div class="contact-item">
        <label>Email / אימייל</label>
        <a href="mailto:contact.ora001@gmail.com">contact.ora001@gmail.com</a>
      </div>
      <div class="contact-item">
        <label>Website / אתר</label>
        <a href="https://ora-guide.pages.dev">ora-guide.pages.dev</a>
      </div>
    </div>

  </div>

</div> -->
