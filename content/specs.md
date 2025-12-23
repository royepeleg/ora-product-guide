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
      border-radius: 50px;
    }

    h1.guide-title {
      font-family: 'Archivo Black', sans-serif;
      font-size: clamp(2rem, 5vw, 3.5rem);
      text-transform: uppercase;
      margin: 0 0 10px 0;
      text-align: center;
      line-height: 1;
      color: var(--text-main);
    }

    .subtitle {
      text-align: center;
      color: var(--text-muted);
      font-size: 2rem;
      margin-bottom: 40px;
    }

    .specs-card {
      background: var(--card-bg);
      border-radius: 24px;
      padding: 20px;
      border: 1px solid #333;
      max-width: 900px;
      margin: 0 auto;
      overflow-x: auto; /* מאפשר גלילה בטלפונים אם הטבלה רחבה מדי */
    }

    .specs-table {
      width: 100%;
      border-collapse: collapse;
      text-align: left;
      min-width: 500px;
    }

    .specs-table th {
      color: var(--accent);
      font-family: 'Archivo Black', sans-serif;
      text-transform: uppercase;
      padding: 15px;
      border-bottom: 2px solid #333;
      font-size: 1.1rem;
    }

    .specs-table td {
      padding: 15px;
      border-bottom: 1px solid #222;
      vertical-align: middle;
    }

    .specs-table tr:hover {
      background: rgba(255, 255, 255, 0.02);
    }

    .feature-name {
      font-weight: 800;
      color: var(--text-main);
      width: 30%;
    }

    .ora-value {
      color: var(--accent);
      font-weight: 700;
      width: 35%;
    }

    .standard-value {
      color: var(--text-muted);
      width: 35%;
    }

    .highlight-cell {
      background: rgba(200, 255, 47, 0.05);
    }

  </style>

  <h1 class="guide-title">Technical Specifications</h1>
  <p class="subtitle">Side-by-side comparison: ORA 1 vs. Standard Lighting Kits</p>

  <div class="specs-card">
    <table class="specs-table">
      <thead>
        <tr>
          <th>Specification</th>
          <th>ORA 1</th>
          <th>Standard Kit (TINI2)</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="feature-name">Weight</td>
          <td class="ora-value">60g</td>
          <td class="standard-value">55.48g</td>
        </tr>
        <tr>
          <td class="feature-name">Lighting Intensity</td>
          <td class="ora-value highlight-cell">500 lm</td>
          <td class="standard-value highlight-cell">200 lm</td>
        </tr>
        <tr>
          <td class="feature-name">Working Power</td>
          <td class="ora-value">5W</td>
          <td class="standard-value">—</td>
        </tr>
        <tr>
          <td class="feature-name">Energy Source</td>
          <td class="ora-value highlight-cell">Drone Battery</td>
          <td class="standard-value highlight-cell">Dedicated Internal Battery</td>
        </tr>
        <tr>
          <td class="feature-name">Charging</td>
          <td class="ora-value">No charging required</td>
          <td class="standard-value">Manual charge per unit</td>
        </tr>
        <tr>
          <td class="feature-name">Operation</td>
          <td class="ora-value highlight-cell">Remote (Controller)</td>
          <td class="standard-value highlight-cell">Manual Switch</td>
        </tr>
      </tbody>
    </table>
  </div>

  <div style="text-align: center; margin-top: 40px;">
    <p style="color: var(--text-muted);">Ready to start? Visit our 
      <a href="/installation-en/" style="color: var(--accent); text-decoration: underline; font-weight: 700;">Installation Guide</a>
    </p>
  </div>

</div>
