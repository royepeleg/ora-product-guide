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

  <h1 class="guide-title">Installation Guide</h1>
  
  <div class="lang-btn-container">
    <a href="/installation-he/" class="lang-btn">עבור לעברית</a>
  </div>

  <div class="video-wrapper">
    <video id="mainVideo" controls>
      <source id="videoSource" src="/videos/instull.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div class="step-card">
    <div class="step-header">Step 1 – Insert the Memory Card</div>
    <div class="check-item">
      <p>Insert the memory card into the slot located inside the left-rear propeller guard, on the drone-side inner wall.</p>
      <div class="image-grid">
        <img src="/images/cdslot1.JPG" alt="CD Slot 1" loading="lazy" />
        <img src="/images/cddoor2.JPG" alt="CD Door 2" loading="lazy" />
      </div>
      <p style="font-size: 1.4rem; color: var(--text-muted); margin-top: 20px;">
        Insert the card gently with the label facing downward. Guide the flexible cable upward toward the top of the drone. Close the card cover gently and ensure the propeller rotates freely.
      </p>
      <img src="/images/cddoor1.JPG" class="single-img" alt="CD Door Closed" loading="lazy" />
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">Step 2 – Secure the Memory Cable</div>
    <div class="check-item">
      <p>Secure the connector of the memory card cable to the drone body using the clip, ensuring it does not interfere with the propeller.</p>
      <div class="image-grid">
        <img src="/images/cdconclips1.JPG" alt="Cable Clips" loading="lazy" />
        <img src="/images/cdcon1.JPG" alt="Cable Secure" loading="lazy" />
      </div>
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">Step 3 – Connect the Rear Unit</div>
    <div class="check-item">
      <p>Connect the rear module to the battery interface on the drone's body. It is recommended to perform the first installation without the battery.</p>
      <p style="color: var(--accent); font-weight: 800;">Important: Insert it straight to avoid bending the pins.</p>
      <img src="/images/rearbefor.JPG" class="single-img" alt="Rear Unit Install" loading="lazy" />
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">Step 4 – Connect the Front Cable</div>
    <div class="check-item">
      <p>Connect the black Type-C cable to the front light module of the kit.</p>
      <div class="image-grid">
        <img src="/images/rearafter2.JPG" alt="Rear View" loading="lazy" />
        <img src="/images/frontcable.jpg" alt="Front Cable Connection" loading="lazy" />
      </div>
      <p style="margin-top:20px;">Then snap the front clip into place as shown.</p>
      <div class="image-grid">
        <img src="/images/frontclips.JPG" alt="Front Clip" loading="lazy" />
        <img src="/images/front.JPG" alt="Front Unit" loading="lazy" />
      </div>
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">Step 5 – Connect the Memory Cable</div>
    <div class="check-item">
      <p>Connect the memory card cable to the matching connector coming from the drone.</p>
      <img src="/images/sdconnection.jpg" class="single-img" alt="SD Connection" loading="lazy" />
    </div>
  </div>

  <div class="step-card">
    <div class="step-header">Step 6 – Install the Battery</div>
    <div class="check-item">
      <p>Insert the battery into its slot and connect it to the kit.</p>
      <div class="image-grid">
        <img src="/images/btrcon.jpg" alt="Battery Connection 1" loading="lazy" />
        <img src="/images/btrcon2.jpg" alt="Battery Connection 2" loading="lazy" />
      </div>
      <div style="margin-top: 30px; padding: 20px; background: rgba(200, 255, 47, 0.1); border-radius: 15px; border-right: 4px solid var(--accent);">
        <p style="font-size: 1.5rem; margin: 0;">
          After completing the installation, follow the testing and activation steps described in the 
          <a href="/user-guide-en/" style="color: var(--accent); font-weight: 700; text-decoration: underline;">User Guide</a>.
        </p>
      </div>
    </div>
  </div>

</div>
