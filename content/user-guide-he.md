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

    .lang-btn:active {
      text-decoration: none;
      transform: translateY(1px) scale(0.98);
      box-shadow: 0 2px 10px rgba(200, 255, 47, 0.4);
      transition: all 0.1s;
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

    .checklist-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .check-item {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .check-item p {
      font-weight: 600;
      font-size: 1.7rem;
      margin: 0;
      min-height: 50px;
    }

    .check-item img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 12px;
      border: 1px solid #444;
      transition: transform 0.3s ease;
    }

    .check-item img:hover {
      transform: scale(1.03);
      border-color: var(--accent);
    }

    ul {
      list-style-type: none;
      padding: 0;
    }

    ul li {
      position: relative;
      padding-right: 25px;
      margin-bottom: 10px;
      color: var(--text-muted);
    }

    ul li::before {
      content: "•";
      color: var(--accent);
      font-weight: bold;
      position: absolute;
      right: 0;
    }

    .important-note {
      border: 2px solid var(--accent);
      background: rgba(200, 255, 47, 0.05);
    }

    .important-note img {
      width: 100%;
      max-width: 600px;
      border-radius: 10px;
      margin-top: 15px;
      border: 1px solid #444;
    }

    @media (max-width: 768px) {
      .checklist-grid {
        grid-template-columns: 1fr;
      }
      .check-item img {
        height: auto;
        max-height: 300px;
      }
      .check-item p {
        min-height: auto;
      }
    }

  </style>

  <h1 class="guide-title">מדריך הפעלה</h1>
  
  <div class="lang-btn-container">
    <a href="/user-guide-en/" class="lang-btn">Switch to English</a>
  </div>

  <div class="video-wrapper">
    <video id="mainVideo" controls>
      <source id="videoSource" src="/videos/guide.mp4" type="video/mp4">
      הדפדפן שלך אינו תומך בנגן הוידאו.
    </video>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 1 – בדיקות מקדימות</div>
    <div class="checklist-grid">
      <div class="check-item">
        <p>בדוק חיבור היחידה האחורית לרחפן</p>
        <img src="/images/rearcon2.jpg" alt="חיבור יחידה אחורית" loading="lazy" />
      </div>
      <div class="check-item">
        <p>בדוק חיבור הסוללה ליחידה האחורית</p>
        <img src="/images/btrccon.jpg" alt="חיבור סוללה" loading="lazy" />
      </div>
      <div class="check-item">
        <p>בדוק שהיחידה הקדמית יושבת היטב ואין חופשים</p>
        <img src="/images/frontunit.jpg" alt="יחידה קדמית" loading="lazy" />
      </div>
      <div class="check-item">
        <p>בדוק את חיבור הכבל השחור לתחתית הפנס הקדמי</p>
        <img src="/images/frontcable.jpg" alt="חיבור כבל" loading="lazy" />
      </div>
      <div class="check-item" style="grid-column: 1 / -1;">
        <p>בדוק את תריס כרטיס הזיכרון ברחפן</p>
        <div style="display:flex; gap:20px;">
            <img src="/images/sddoor1.jpg" alt="תריס SD 1" style="width:50%; height:auto; border-radius:12px;" loading="lazy" />
            <img src="/images/sddoor2.jpg" alt="תריס SD 2" style="width:50%; height:auto; border-radius:12px;" loading="lazy" />
        </div>      
        <ul style="margin-top:15px;">
          <li>ודא בעדינות שהוא סגור עד הסוף והפרופלור יכול להסתובב בחופשיות</li>
          <li>ודא שהכבל הגמיש יוצא בצורה ישרה מהתריס ללא כיפוף</li>
        </ul>
      </div>
      <div class="check-item">
        <p>בדוק את חיבור כרטיס הזיכרון ליחידה האחורית<br><span style="font-size:1.5rem; color:#888;">שים לב שהקונקטור מחובר היטב כדי שלא יפגע מהפרופלור בזמן טיסה</span></p>
        <img src="/images/sdconnection.jpg" alt="חיבור כרטיס זיכרון" loading="lazy" />
      </div>
    </div>

  </div>

  <div class="step-card">
    <div class="step-header">שלב 2 – הדלקה</div>
    <ul>
      <li><strong style="color:white;">הפעל</strong> את הרחפן</li>
      <li><strong style="color:white;">הפעל</strong> את השלט</li>
      <li><strong style="color:white;">הפעל</strong> את המשקף</li>
      <li>המתן לסיום ההדלקה עד שמופיע שידור מהרחפן על המסך</li>
    </ul>
  </div>

  <div class="step-card">
    <div class="step-header">שלב 3 – הפעלה ובדיקת מערכת</div>
    <div style="display: flex; flex-direction: column; gap: 20px; align-items: center; text-align: center;">
      <p style="font-size: 1.7rem;">לחץ על <strong style="color:var(--accent);">כפתור הצילום</strong> בשלט — לאחר כ־5 שניות הפנסים יידלקו</p>      
      <img src="/images/photobtn.jpg" alt="כפתור צילום" style="max-width: 350px; border-radius: 12px; border: 1px solid #444;" />
      <div style="text-align: right; background: rgba(255,255,255,0.05); padding: 20px; border-radius: 10px; width: 100%;">
        <p style="margin-bottom: 10px;"><strong>טיפים לתפעול:</strong></p>
        <ul>
          <li>בצע הדלקה וכיבוי פעמיים כדי לוודא שהמערכת פועלת כראוי.</li>
          <li>ניתן לכבות ולהדליק את הרחפן גם במהלך הטיסה.</li>
          <li>יש להמתין להדלקה מלאה של הפנס לפני לחיצה נוספת לכיבוי — ולהיפך.</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="step-card important-note">
    <div class="step-header" style="border-bottom-color: var(--accent);">הערה חשובה</div>
    <div style="text-align: center;">
      <p style="font-size: 1.7rem;">הרחפן אמור להראות <strong>"SD Slow"</strong>, זהו המצב הרצוי:</p>
      <img src="/images/cdslowapp.PNG" alt="אזהרת SD Slow" />
      <p style="font-size: 1.7rem; margin-top: 30px;">אם זה לא מופיע, בצע הגדרת צילום על כרטיס הזיכרון כפי שמוצג בתמונה:</p>
      <img src="/images/sdmode.jpg" alt="הגדרת מצב SD" />
    </div>
  </div>

</div>
