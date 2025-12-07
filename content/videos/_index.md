---
title: "Videos"
---

# Product Videos

Click on a tutorial to watch:

<ul>
  <li><a href="#" onclick="showVideo('intro')">📘 Tutorial Video</a></li>
  <li><a href="#" onclick="showVideo('cleaning')">🧼 Cleaning Instructions</a></li>
  <li><a href="#" onclick="showVideo('calibration')">🎯 Calibration Guide</a></li>
</ul>

<hr>

<div id="videoPlayer" style="margin-top:20px; display:none;">
  <video id="mainVideo" width="100%" controls>
    <source id="videoSource" src="" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

<script>
function showVideo(name) {
  const sources = {
    "intro": "/videos/v1.mp4",
    "cleaning": "/videos/cleaning.mp4",
    "calibration": "/videos/calibration.mp4"
  };

  document.getElementById('videoSource').src = sources[name];
  document.getElementById('mainVideo').load();

  document.getElementById('videoPlayer').style.display = 'block';
}
</script>
