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
      padding: 40px 20px;
      line-height: 1.5;
      max-width: 100%;
      border-radius:50px;
    }


    h1.guide-title {
      font-family: 'Archivo Black', sans-serif;
      font-size: clamp(2.5rem, 5vw, 4rem);
      text-transform: uppercase;
      margin: 0 0 20px 0;
      text-align: center;
      line-height: 1;
      color:var(--text-main);
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
      text-decoration: none;
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

    /* כרטיסיות שלבים */
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

    /* רשת תמונות לשלב 1 */
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
      min-height: 50px; /* גובה אחיד לטקסט */
    }

    .check-item img {
      width: 100%;
      height: 200px; /* גובה אחיד לתמונות */
      object-fit: cover;
      border-radius: 12px;
      border: 1px solid #444;
      transition: transform 0.3s ease;
    }

    .check-item img:hover {
      transform: scale(1.03);
      border-color: var(--accent);
    }

    /* רשימות */
    .step-card ul {
      list-style-type: none;
      padding: 0;
    }

.step-card ul li { position: relative; padding-left: 20px; margin-bottom: 10px; color: var(--text-muted); }

.step-card ul li::before { content: "•"; color: var(--accent); font-weight: bold; position: absolute; left: 0; }

    /* Important Note Section */
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

    /* רספונסיביות */
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

  <h1 class="guide-title">Operating Guide</h1>
  
  <div class="lang-btn-container">
    <a href="/user-guide-he/" class="lang-btn">עבור לעברית</a>
  </div>

  <div class="video-wrapper">
    <video id="mainVideo" controls>
      <source id="videoSource" src="/videos/guide.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div class="step-card">
    <div class="step-header">Step 1 – Pre-Flight Checks</div>
    <div class="checklist-grid">
      <div class="check-item">
        <p>Check the rear unit connection to the drone</p>
        <img src="/images/rearcon2.jpg" alt="Rear Unit Connection" loading="lazy" />
      </div>
      <div class="check-item">
        <p>Check the battery connection to the rear unit</p>
        <img src="/images/btrccon.jpg" alt="Battery Connection" loading="lazy" />
      </div>
      <div class="check-item">
        <p>Check that the front unit is seated properly and has no play</p>
        <img src="/images/frontunit.jpg" alt="Front Unit" loading="lazy" />
      </div>
      <div class="check-item">
        <p>Check the black cable connection to the bottom of the front light</p>
        <img src="/images/frontcable.jpg" alt="Cable Connection" loading="lazy" />
      </div>
      <div class="check-item" style="grid-column: 1 / -1;">
        <p>Check the memory-card door on the drone</p>
        <div style="display:flex; gap:20px;">
            <img src="/images/sddoor1.jpg" alt="SD Door 1" style="width:50%; height:auto; border-radius:12px;" loading="lazy" />
            <img src="/images/sddoor2.jpg" alt="SD Door 2" style="width:50%; height:auto; border-radius:12px;" loading="lazy" />
        </div>      
        <ul style="margin-top:15px;">
          <li>Gently ensure the door is fully closed and the propeller can rotate freely</li>
          <li>Ensure the flexible cable exits the door straight without bending</li>
        </ul>
      </div>
      <div class="check-item">
        <p>Check the memory card connection to the rear unit<br><span style="font-size:1.5rem; color:#888;">Make sure the connector is fully inserted so it does not enter the propeller area during flight</span></p>
        <img src="/images/sdconnection.jpg" alt="SD Connection" loading="lazy" />
      </div>
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">Step 2 – Power On</div>
    <ul>
      <li><strong style="color:white;">Turn on</strong> the drone</li>
      <li><strong style="color:white;">Turn on</strong> the controller</li>
      <li><strong style="color:white;">Turn on</strong> the goggles</li>
      <li>Wait for the full startup sequence until the drone video feed appears on the screen</li>
    </ul>
  </div>

  <div class="step-card">
    <div class="step-header">Step 3 – System Operation</div>
    <div style="display: flex; flex-direction: column; gap: 20px; align-items: center; text-align: center;">
      <p style="font-size: 1.7rem;">Press the <strong style="color:var(--accent);">photo button</strong> on the controller — after ~5 seconds the lights will turn on</p>      
      <img src="/images/photobtn.jpg" alt="Photo Button" style="max-width: 350px; border-radius: 12px; border: 1px solid #444;" />
      <div style="text-align: left; background: rgba(255,255,255,0.05); padding: 20px; border-radius: 10px; width: 100%;">
        <p style="margin-bottom: 10px;"><strong>Operational Tips:</strong></p>
        <ul>
          <li>Turn the system off and on twice to verify proper operation.</li>
          <li>You may turn the drone off and on during flight.</li>
          <li>Be sure to wait for the flashlight to turn on before pressing again to turn it off - and vice versa.</li>
        </ul>
      </div>
    </div>

  </div>

  <div class="step-card important-note">
    <div class="step-header" style="border-bottom-color: var(--accent);">Important Note</div>
    <div style="text-align: center;">
      <p style="font-size: 1.7rem;">The drone should show <strong>"SD Slow"</strong>, this is the desired state:</p>
      <img src="/images/cdslowapp.png" alt="SD Slow Warning" />
      <p style="font-size: 1.7rem; margin-top: 30px;">If it does not appear, set up a photo on the memory card as shown below:</p>
      <img src="/images/sdmode.jpg" alt="SD Mode Setup" />
    </div>
  </div>

</div>
