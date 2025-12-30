+++
title = ""
+++

<div class="guide-page" dir="rtl">
  
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
      padding: 40px 20px;
      line-height: 1.5;
      max-width: 100%;
      border-radius: 50px;
      text-align: right;
    }

    h1.guide-title {
      font-family: 'Archivo Black', sans-serif;
      font-size: clamp(2.5rem, 5vw, 4rem);
      text-transform: uppercase;
      margin: 0 0 20px 0;
      text-align: center;
      line-height: 1;
      color: var(--text-main);
    }

    .step-header {
      color: var(--accent);
      font-family: 'Archivo Black', sans-serif;
      font-size: 1.8rem;
      margin-bottom: 20px;
      text-transform: uppercase;
      border-bottom: 2px solid #333;
      padding-bottom: 10px;
    }

    .lang-btn-container {
      text-align: center;
      margin-bottom: 40px;
    }

    .lang-btn {
      display: inline-block;
      padding: 10px 30px;
      border-radius: 999px;
      background: rgba(255, 255, 255, 0.1);
      color: var(--accent);
      text-decoration: none;
      font-weight: 700;
      border: 1px solid var(--accent);
      transition: all 0.3s ease;
    }

    .lang-btn:hover {
      background: var(--accent);
      text-decoration: none;
      color: #000;
      box-shadow: 0 0 20px rgba(200, 255, 47, 0.4);
    }

    .video-wrapper {
      max-width: 500px;
      margin: 0 auto 60px;
      border-radius: 20px;
      overflow: hidden;
      border: 2px solid #333;
      box-shadow: 0 20px 50px rgba(0,0,0,0.5);
    }

    video {
      display: block;
      width: 100%;
      height: auto;
    }

    .step-card {
      background: var(--card-bg);
      border-radius: 20px;
      padding: 30px;
      margin-bottom: 40px;
      border: 1px solid #333;
      max-width: 900px;
      margin-left: auto;
      margin-right: auto;
    }

    .check-item {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .check-item p {
      font-weight: 600;
      font-size: 1.7rem;
      margin: 0;
    }

    .image-grid {
      display: flex;
      gap: 20px;
      margin-top: 10px;
    }

    .image-grid img {
      width: 50%;
      height: auto;
      object-fit: cover;
      border-radius: 12px;
      border: 1px solid #444;
      transition: transform 0.3s ease;
    }

    .image-grid img:hover {
      transform: scale(1.03);
      border-color: var(--accent);
    }

    .single-img {
       width: 100%;
       max-width: 450px;
       border-radius: 12px;
       border: 1px solid #444;
       margin-top: 10px;
    }

    @media (max-width: 768px) {
      .image-grid {
        flex-direction: column;
      }
      .image-grid img {
        width: 100%;
      }
    }

  </style>

  <h1 class="guide-title">מדריך התקנה</h1>
  
  <div class="lang-btn-container">
    <a href="/installation-en/" class="lang-btn">Switch to English</a>
  </div>

  <div class="video-wrapper">
    <video id="mainVideo" controls>
      <source id="videoSource" src="/videos/instull.mp4" type="video/mp4">
      הדפדפן שלך אינו תומך בנגן הוידאו.
    </video>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 1 – הכנסת כרטיס הזיכרון</div>
    <div class="check-item">
      <p>הכנס את כרטיס הזיכרון אל החריץ בגוף הרחפן שנמצא בתוך המגן של הפרופ האחורי שמאלי, בדופן הקרובה לגוף הרחפן.</p>
      <div class="image-grid">
        <img src="/images/cdslot1.JPG" alt="חריץ כרטיס זיכרון" loading="lazy" />
        <img src="/images/cddoor2.JPG" alt="דלת כרטיס זיכרון" loading="lazy" />
      </div>
      <p style="font-size: 1.4rem; color: var(--text-muted); margin-top: 20px;">
        את הכרטיס יש להכניס בזהירות כשהכיתוב כלפי מטה. את הכבל הגמיש יש להשחיל לכיוון החלק העליון של הרחפן, ולאחר מכן לסגור בעדינות את המכסה ולוודא שהפרופ מסתובב חופשי.
      </p>
      <img src="/images/cddoor1.JPG" class="single-img" alt="מכסה סגור" loading="lazy" />
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 2 – קיבוע מחבר כרטיס הזיכרון</div>
    <div class="check-item">
      <p>את המחבר שמחובר לכבל של כרטיס הזיכרון יש לקבע לגוף הרחפן בעזרת הקליפס, ולוודא שהוא אינו מפריע לפרופ.</p>
      <div class="image-grid">
        <img src="/images/cdconclips1.JPG" alt="קליפסים למחבר" loading="lazy" />
        <img src="/images/cdcon1.JPG" alt="מחבר מקובע" loading="lazy" />
      </div>
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 3 – חיבור היחידה האחורית</div>
    <div class="check-item">
      <p>יש לחבר את החלק האחורי למקום שאליו מתחברת סוללת הרחפן בגוף הרחפן. מומלץ לבצע את החיבור הראשון ללא הסוללה.</p>
      <p style="color: var(--accent); font-weight: 800;">שים לב! יש להכניס בצורה ישרה כדי לא לעקם את הפינים.</p>
      <img src="/images/rearbefor.JPG" class="single-img" alt="התקנת יחידה אחורית" loading="lazy" />
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 4 – חיבור הכבל הקדמי</div>
    <div class="check-item">
      <p>חבר את הכבל השחור עם מחבר ה-Type-C לפנס הקדמי של הערכה.</p>
      <div class="image-grid">
        <img src="/images/rearafter2.JPG" alt="מבט אחורי" loading="lazy" />
        <img src="/images/frontcable.jpg" alt="חיבור כבל קדמי" loading="lazy" />
      </div>
      <p style="margin-top:20px;">ואז חבר את הקליפס הקדמי למקומו כפי שמוצג בתמונה.</p>
      <div class="image-grid">
        <img src="/images/frontclips.JPG" alt="קליפס קדמי" loading="lazy" />
        <img src="/images/front.JPG" alt="יחידה קדמית" loading="lazy" />
      </div>
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 5 – חיבור מחבר הזיכרון</div>
    <div class="check-item">
      <p>חבר את המחבר של כרטיס הזיכרון אל הכבל שיוצא מהרחפן.</p>
      <img src="/images/sdconnection.jpg" class="single-img" alt="חיבור כרטיס זיכרון" loading="lazy" />
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 6 – חיבור הסוללה</div>
    <div class="check-item">
      <p>חבר את הסוללה למקומה ואת המחבר שלה למקומו בגוף הערכה.</p>
      <div class="image-grid">
        <img src="/images/btrcon.JPG" alt="חיבור סוללה 1" loading="lazy"/>
        <img src="/images/btrcon2.JPG" alt="חיבור סוללה 2" loading="lazy"/>
      </div>
      <div style="margin-top: 30px; padding: 20px; background: rgba(200, 255, 47, 0.1); border-radius: 15px; border-right: 4px solid var(--accent);">
        <p style="font-size: 1.5rem; margin: 0;">
          לאחר סיום ההתקנה יש לבצע את הבדיקות וההפעלה כפי שמתואר ב
          <a href="/user-guide-he/" style="color: var(--accent); font-weight: 700; text-decoration: underline;">מדריך ההפעלה</a>.
        </p>
      </div>
    </div>
  </div>

</div>
