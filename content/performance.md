+++
title = ""
+++

<div class="performance-page">
  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    @import url("https://fonts.googleapis.com/css2?family=Archivo+Black&family=Inter:wght@400;700;900&family=Assistant:wght@400;700&display=swap");
    :root {
      --accent: #c8ff2f; /* הצהוב הזרחני שלך */
      --dark: #080808;
      --card-bg: #141414;
      --text-main: #ffffff;
      --text-muted: #888888;
      --competitor-color: #4a4a4a; /* אפור עבור המתחרה */
    }
    .performance-page {
      background: var(--dark);
      color: var(--text-main);
      font-family: 'Assistant', 'Inter', sans-serif;
      padding: 40px 20px;
      max-width: 100%;
      overflow-x: hidden;
      direction: ltr; 
      border-radius: 50px;
    }
    h1, h2, h3 {
      font-family: 'Archivo Black', sans-serif;
      text-transform: uppercase;
      margin: 0;
      color:white
    }
    /* --- SECTION 1: HEAD TO HEAD --- */
    .comparison-header {
      text-align: center;
      margin-bottom: 60px;
    }
    .comparison-header h1 {
      font-size: clamp(2.5rem, 5vw, 4rem);
      margin-bottom: 10px;
    }
    .products-grid {
      display: grid;
      grid-template-columns: 1fr 80px 1fr; /* מוצר - VS - מוצר */
      gap: 20px;
      max-width: 1000px;
      margin: 0 auto 60px;
      align-items: center;
    }
    .product-card {
      background: var(--card-bg);
      padding: 30px;
      border-radius: 20px;
      text-align: center;
      border: 1px solid #333;
      position: relative;
    }
    .product-card.our-product {
      border: 2px solid var(--accent);
      box-shadow: 0 0 30px rgba(200, 255, 47, 0.1);
    }
    .product-img-placeholder {
      width: 100%;
          max-height: 340px;
      background: #222; /* כאן תיכנס התמונה שלך */
      border-radius: 10px;
      margin-bottom: 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      object-fit: contain;
    }
    .product-title {
      font-size: 1.8rem;
      font-weight: 900;
      margin-bottom: 5px;
    }
    .our-product .product-title { color: var(--accent); }
    .competitor .product-title { color: #fff; }
    .vs-badge {
      background: #fff;
      color: #000;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Archivo Black';
      font-size: 1.5rem;
      z-index: 2;
    }
    /* --- SECTION 2: FLIGHT TIME CHART --- */
    .stats-section {
      max-width: 900px;
      margin: 0 auto 80px;
    }
    .section-title {
      font-size: 2rem;
      margin-bottom: 30px;
      border-left: 5px solid var(--accent);
      padding-left: 15px;
    }
    .chart-container {
      background: var(--card-bg);
      padding: 30px;
      border-radius: 20px;
    }
    .bar-group {
      margin-bottom: 25px;
    }
    .bar-label {
      display: flex;
      justify-content: space-between;
      margin-bottom: 8px;
      font-weight: 700;
    }
    .progress-bg {
      background: #333;
      height: 24px;
      border-radius: 12px;
      overflow: hidden;
      position: relative;
    }
    .progress-fill {
      height: 100%;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: flex-end;
      padding-right: 10px;
      font-size: 1.4rem;
      font-weight: bold;
      color: #000;
    }
    /* צבעים לגרף */
    .fill-base { background: #fff; width: 100%; } /* רחפן נקי */
    .fill-ora { background: var(--accent); width: 92%; } /* המוצר שלך */
    .fill-comp { background: var(--competitor-color); color: #fff; width: 85%; } /* מתחרה */
    /* --- SECTION 3: WEIGHT & SPECS --- */
    .specs-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
      max-width: 1000px;
      margin: 0 auto 80px;
    }
    .spec-box {
      background: var(--card-bg);
      padding: 30px;
      border-radius: 20px;
      text-align: center;
    }
    .big-number {
      font-size: 3.5rem;
      font-family: 'Archivo Black';
      line-height: 1;
      margin: 10px 0;
    }
    .ora-num { color: var(--accent); }
    .comp-num { color: #888; font-size: 2.5rem; }
    /* --- SECTION 4: VIDEO COMPARISON --- */
    .video-comparison {
      max-width: 1200px;
      margin: 0 auto 80px;
    }
    .video-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
    }
    .video-wrapper {
      position: relative;
      padding-bottom: 56.25%; /* 16:9 Aspect Ratio */
      height: 0;
      background: #000;
      border-radius: 10px;
      overflow: hidden;
    }
    .video-wrapper iframe, .video-wrapper video {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
    }
    .video-label {
      text-align: center;
      padding: 10px;
      font-weight: bold;
      background: #222;
      margin-bottom: 10px;
      border-radius: 8px;
    }
    /* --- FEATURE LIST (TABLE REPLACEMENT) --- */
    .feature-list {
      max-width: 800px;
      margin: 0 auto;
    }
    .feature-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 0;
      border-bottom: 1px solid #333;
    }
    .feature-item:last-child { border-bottom: none; }
    .feature-name {
      font-size: 2.1rem;
      color: #aaa;
    }
    .feature-val-ora {
      font-weight: bold;
      color: var(--accent);
      text-align: right;
      font-size: 2.2rem;
    }
    .feature-val-comp {
      font-size: 1.9rem;
      color: #666;
      text-align: right;
      text-decoration: line-through;
      margin-top: 5px;
    }
    /* MOBILE RESPONSIVE */
    @media (max-width: 768px) {
      .products-grid {
        grid-template-columns: 1fr;
        gap: 40px;
      }
      .vs-badge {
        margin: -30px auto; /* ממקם את ה-VS באמצע בין הכרטיסים */
      }
      .video-grid {
        grid-template-columns: 1fr;
      }
      .feature-item {
        flex-direction: column;
        align-items: flex-start;
        gap: 10px;
      }
      .feature-val-ora, .feature-val-comp {
        text-align: left;
      }
    }

  </style>

  <div class="comparison-header">
    <h1>Performance</h1>
    <p style="color: #888; font-size: 2.2rem;">ORA 1 vs. Standard (TINI2)</p>
  </div>

  <div class="products-grid">
    <div class="product-card our-product">
      <div class="product-title">ORA 1</div>
      <img src="/images/noback.png" alt="ORA 1" class="product-img-placeholder" style="object-fit: cover;">
      <p>Professional Drone Lighting</p>
    </div>
    <div class="vs-badge">VS</div>
    <div class="product-card competitor">
      <div class="product-title">TINI 2</div>
      <img src="/images/tini2white.png" alt="TINI 2" class="product-img-placeholder" style="object-fit: cover; filter: grayscale(100%);">
      <p>Standard Flashlight Kit</p>
    </div>

  </div>

  <div class="stats-section">
    <h2 class="section-title">Flight Time Impact</h2>
    <div class="chart-container">
      <div class="bar-group">
        <div class="bar-label">
          <span>Drone Only (No Payload)</span>
          <span>28 Min</span> </div>
        <div class="progress-bg">
          <div class="progress-fill fill-base">100%</div>
        </div>
      </div>
      <div class="bar-group">
        <div class="bar-label">
          <span style="color: var(--accent);">With ORA 1</span>
          <span style="color: var(--accent);">26 Min</span> </div>
        <div class="progress-bg">
          <div class="progress-fill fill-ora">92%</div>
        </div>
      </div>
      <div class="bar-group">
        <div class="bar-label">
          <span>With TINI 2 Kit</span>
          <span>24 Min</span> </div>
        <div class="progress-bg">
          <div class="progress-fill fill-comp">85%</div>
        </div>
      </div>
      <p style="margin-top: 20px; font-size: 1.9rem; color: #666;">
        * Flight times are estimated based on hover conditions with DJI Mavic 3.
      </p>
    </div>
  </div>
  <div class="specs-grid">
    <div class="spec-box">
      <h3>Total Weight</h3>
      <div style="display: flex; justify-content: center; align-items: baseline; gap: 20px; margin-top: 20px;">
        <div>
          <div class="big-number ora-num">60g</div>
          <div style="color:var(--accent)">ORA 1</div>
        </div>
        <div style="border-right: 1px solid #333; height: 50px;"></div>
        <div>
          <div class="big-number comp-num">55g</div>
          <div style="color:#666">TINI 2</div>
        </div>
      </div>
      <p style="color: #888; margin-top: 15px;">
        Although slightly heavier, ORA 1 includes an integrated power management system, eliminating external batteries.
      </p>
    </div>
    <div class="spec-box">
      <h3>Brightness (Lumens)</h3>
      <div class="big-number ora-num" style="margin-top: 20px;">500 lm</div>
      <p style="color: #fff; margin-bottom: 5px;">vs 200 lm (Competitor)</p>
      <div class="progress-bg" style="margin-top: 15px;">
        <div class="progress-fill fill-ora" style="width: 100%;">2.5x Brighter</div>
      </div>
    </div>

  </div>

  <div class="video-comparison">
    <h2 class="section-title">Night Visibility Test</h2>
    <div class="video-grid">
      <div>
        <div class="video-label" style="color: var(--accent);">ORA 1 (500 Lumens)</div>
        <div class="video-wrapper">
          <iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID_HERE" frameborder="0" allowfullscreen></iframe>
        </div>
      </div>
      <div>
        <div class="video-label" style="color: #888;">Standard Kit (200 Lumens)</div>
        <div class="video-wrapper">
           <iframe src="https://www.youtube.com/embed/COMPETITOR_VIDEO_ID" frameborder="0" allowfullscreen></iframe>
        </div>
      </div>
    </div>
  </div>

  <div class="feature-list">
    <h3 style="text-align: center; margin-bottom: 30px; font-size: 2.5rem;">Detailed Specifications</h3>
    <div class="feature-item">
      <div class="feature-name">Lighting Intensity</div>
      <div>
        <div class="feature-val-ora">500 Lumens</div>
        <div class="feature-val-comp">200 Lumens</div>
      </div>
    </div>
    <div class="feature-item">
      <div class="feature-name">Operation Method</div>
      <div>
        <div class="feature-val-ora">Remote Control (Drone Controller)</div>
        <div class="feature-val-comp">Manual Switch Only</div>
      </div>
    </div>
    <div class="feature-item">
      <div class="feature-name">Power Source</div>
      <div>
        <div class="feature-val-ora">Direct Drone Power</div>
        <div class="feature-val-comp">Separate Battery Required</div>
      </div>
    </div>
    <div class="feature-item">
      <div class="feature-name">Charging</div>
      <div>
        <div class="feature-val-ora">No Charging Needed</div>
        <div class="feature-val-comp">Requires Frequent Charging</div>
      </div>
    </div>

  </div>

</div>
