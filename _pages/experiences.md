---
layout: archive
title: "My Experiences"
permalink: /experiences/
author_profile: true
---

<!-- Back to home link -->
<div style="max-width:1100px; margin:20px auto;">
  <a href="/" style="font-size:17px; text-decoration:none; color:#4a78ff; font-weight:600;">
    ← Back to Homepage
  </a>
</div>

<style>
/* ===========================
   Modern Intro Styling
   =========================== */
.experiences-intro {
  max-width: 900px;
  margin: 0 auto 50px auto;
  padding: 35px 38px;
  border-radius: 22px;
  background: linear-gradient(135deg, rgba(76,115,255,0.12), rgba(255,255,255,0.65));
  backdrop-filter: blur(10px);
  border: 1px solid rgba(160,175,255,0.3);
  box-shadow: 0 10px 36px rgba(0,0,0,0.08);
  text-align: center;
  font-family: "Inter", sans-serif;
  color: #1d2b3a;
  font-size: 20px;
  line-height: 1.75;
}

/* DARKER TITLE */
.experiences-intro h2 {
  margin-top: 0;
  margin-bottom: 18px;
  font-size: 32px;
  font-weight: 800;
  color: #0f1c2b; /* Solid darker navy */
}

/* ===========================
   Experience Card
   =========================== */
.experience-card {
  max-width: 1100px;
  margin: 45px auto;
  padding: 38px 40px;
  border-radius: 26px;
  background: rgba(255,255,255,0.78);
  backdrop-filter: blur(14px);
  border: 1px solid rgba(210,210,210,0.45);
  box-shadow: 
      0 12px 40px rgba(0,0,0,0.08),
      0 2px 6px rgba(0,0,0,0.05);
  font-family: "Inter", sans-serif;
  transition: transform .25s ease, box-shadow .25s ease;
}

/* STRONGER, CLEANER CARD TITLE (OLD STYLE) */
.experience-title {
  text-align: center;
  font-size: 28px;   /* slightly smaller, sharper */
  font-weight: 700;  /* stronger classic look */
  margin-bottom: 22px;
  color: #16222e;
  letter-spacing: 0.1px;
}

/* ===========================
   Media row (3 items)
   =========================== */
.media-row {
  display: flex;
  justify-content: center;
  gap: 25px;
  flex-wrap: nowrap;
  padding-bottom: 10px;
}

.media-row img,
.media-row iframe {
  width: 32%;
  height: 260px;
  object-fit: cover;
  border-radius: 18px;
  border: 1px solid rgba(200,200,200,0.45);
  background: #fff;
  box-shadow: 0 8px 18px rgba(0,0,0,0.12);
  transition: transform .25s ease, box-shadow .25s ease;
}

.media-row img:hover,
.media-row iframe:hover {
  transform: scale(1.015);
  box-shadow: 0 12px 28px rgba(0,0,0,0.18);
}

/* Text */
.experience-text {
  font-size: 18px;
  line-height: 1.75;
  color: #2c2f36;
  text-align: left;
  max-width: 950px;
  margin: 20px auto 0 auto;
  padding: 0 5px;
}
</style>

<!-- ======================= -->
<!-- Intro Section           -->
<!-- ======================= -->
<div class="experiences-intro">
  <h2>My Experiences</h2>
  Here I share highlights from conferences, workshops, academic events,  
  and meaningful moments in my research journey.  
  These experiences help me learn, grow, and stay connected with the AI community. ✨
</div>

<!-- ======================= -->
<!-- CVPR 2025 EXPERIENCE    -->
<!-- ======================= -->
<div class="experience-card">

  <div class="experience-title">CVPR 2025 Experience</div>

  <div class="media-row">
    <img src="/images/cvpr2025.jpg" alt="CVPR 2025 Image 1">
    <img src="/images/cvpr2025-image.jpg" alt="CVPR 2025 Image 2">
    <iframe 
      src="https://drive.google.com/file/d/1FRzcL42qNmYI19X1_Nt-EjK5U6g7QZHX/preview"
      allow="autoplay">
    </iframe>
  </div>

  <div class="experience-text">
    I attended <b>CVPR 2025</b> — an incredible opportunity to meet world-class researchers, 
    explore breakthrough work in 3D Computer Vision, Gaussian Splatting, foundation models,  
    and learn about the newest progress across the vision community.
    <br><br>
    It was inspiring to attend workshops, connect with companies, gain insights from top labs,  
    and talk with experts shaping the future of AI.  
    I came back with new ideas, motivation, and a deeper understanding of current research trends.
  </div>

</div>
