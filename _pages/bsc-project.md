---
layout: archive
title: "Behavior Analysis of Car Drivers Based on Computer Vision"
permalink: /driver-behavior/
author_profile: true
---

<div class="project-page">

<style>
.project-page {
  background: #f6f7f9;
  padding-bottom: 40px;
}

/* Intro */
.project-intro {
  display: grid;
  grid-template-columns: 1fr 1.3fr;
  gap: 24px;
  align-items: center;
  background: #ffffff;
  padding: 24px 28px;
  margin: 0 auto 32px auto;
  max-width: 1050px;
  border-radius: 16px;
  box-shadow: 0 6px 20px rgba(0,0,0,0.08);
}
.project-intro img {
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.18);
}
.project-intro-text {
  font-size: 17px;
  line-height: 1.6;
}

/* Section title */
.project-section-title {
  text-align: center;
  font-size: 28px;
  font-weight: 700;
  margin: 28px 0 18px 0;
}

/* Two-column grids */
.project-grid-2 {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 32px;
  max-width: 1050px;
  margin: 0 auto 32px auto;
}

/* Video boxes */
.project-video-box {
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.20);
  background: #000;
}
.project-video-box iframe {
  width: 100%;
  height: 250px;
}

/* Captions */
.project-caption-title {
  text-align: center;
  font-size: 19px;
  font-weight: 700;
  margin-top: 10px;
}
.project-caption-text {
  text-align: center;
  font-size: 15px;
  margin: 0 auto;
  max-width: 90%;
}

/* Architecture image */
.project-arch-img {
  display: block;
  margin: 14px auto 28px auto;
  max-width: 650px;
  width: 60%;
  border-radius: 12px;
  box-shadow: 0 4px 14px rgba(0,0,0,0.15);
}

/* Divider */
.project-divider {
  height: 1px;
  width: 75%;
  background: #cccccc;
  margin: 32px auto;
}
</style>

<div class="project-section-title">
🚗 Behavior Analysis of Car Drivers Based on Computer Vision
</div>

<div class="project-intro">
  <img src="/images/Intro.jpg" alt="Driver project intro">
  <div class="project-intro-text">
    This project develops an advanced driver assistance system (ADAS) using computer vision.  
    By combining <b>YOLOv8</b> 🧠, <b>Optical Flow</b> 🔄, and <b>SSD</b> face detection 👤, the system
    detects objects outside the vehicle while analyzing the driver’s head pose inside the car.
    <br><br>
    A built-in <b>Voice Assistant</b> 🔊 informs the driver about potential dangers and traffic
    conditions to improve overall road safety.
  </div>
</div>

<div class="project-divider"></div>

<div class="project-section-title">🧩 System Components</div>

<div class="project-grid-2">

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1A2q3yyOWNahFMdCXNqwSgLiplSm0I8R8/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Head Direction Detection 👁️</div>
    <div class="project-caption-text">
      Uses SSD-based face detection to estimate the driver’s head orientation.
    </div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/10NZdcjuLJwZpQkWyuejilv89bkpzwO8w/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Object Detection & Tracking 📦➡️</div>
    <div class="project-caption-text">
      YOLOv8 detects external objects while Optical Flow tracks their motion.
    </div>
  </div>

</div>

<div class="project-divider"></div>

<div class="project-section-title">🎥 Examples of the Running System</div>

<div class="project-grid-2">

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1OBGQBOWgTtPI4M-Lg9MHks1ceZ5gpF04/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Wake Up! 😴➡️⚠️</div>
    <div class="project-caption-text">Detects driver drowsiness and alerts them to stay safe.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1SKdeQcPozlHjiXv1Xai9ZFWGEwpoZ0t2/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Traffic Light 🚦</div>
    <div class="project-caption-text">Identifies upcoming traffic lights and informs the driver.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/175rLPKxnW_U6EwKj4D845NgkOWCcjafd/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Pedestrian 🚶‍♂️</div>
    <div class="project-caption-text">Detects nearby pedestrians for safer navigation.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1Xo7zvCDjAGA3eRQL3tgdRpmuObn_qE4a/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Look Left 👈</div>
    <div class="project-caption-text">Warns when hazards approach from the left side.</div>
  </div>

</div>

<div class="project-divider"></div>

<div class="project-section-title">🛠️ System Architecture</div>
<img src="/images/Architecture.jpg" class="project-arch-img" alt="System architecture diagram">

</div> <!-- END .project-page -->
