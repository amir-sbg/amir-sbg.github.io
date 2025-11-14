---
layout: archive
title: "Behavior Analysis of Car Drivers Based on Computer Vision"
permalink: /driver-behavior/
author_profile: true
---

<!--

<style>
/* ===========================
   Global Page Styling
   =========================== */
.project-page {
  background: linear-gradient(180deg, #f4f5f7 0%, #eef0f3 100%);
  padding-bottom: 50px;
  font-family: "Inter", sans-serif;
}

/* ===========================
   Section Title
   =========================== */
.project-section-title {
  text-align: center;
  font-size: 34px;
  font-weight: 800;
  margin: 40px 0 25px 0;
  color: #1f2d3d;
  letter-spacing: 0.3px;
  text-transform: none;
  position: relative;
}

/* Stylish underline */
.project-section-title::after {
  content: "";
  display: block;
  width: 70px;
  height: 4px;
  background: #3c7dff;
  margin: 12px auto 0 auto;
  border-radius: 3px;
}

/* ===========================
   Intro Section
   =========================== */
.project-intro {
  display: grid;
  grid-template-columns: 1fr 1.2fr;
  gap: 30px;
  align-items: center;
  background: white;
  padding: 28px 32px;
  margin: 0 auto 45px auto;
  max-width: 1100px;
  border-radius: 18px;
  box-shadow: 0 8px 24px rgba(0,0,0,0.09);
}

.project-intro img {
  width: 100%;
  border-radius: 14px;
  box-shadow: 0 4px 14px rgba(0,0,0,0.18);
}

.project-intro-text {
  font-size: 18px;
  line-height: 1.7;
  color: #333;
}

/* ===========================
   Grid (2 columns)
   =========================== */
.project-grid-2 {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 35px;
  max-width: 1100px;
  margin: 8px auto 45px auto;
}

/* ===========================
   Video Boxes
   =========================== */
.project-video-box {
  border-radius: 14px;
  overflow: hidden;
  background: #000;
  box-shadow: 0 6px 16px rgba(0,0,0,0.25);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

/* Hover zoom effect */
.project-video-box:hover {
  transform: translateY(-6px);
  box-shadow: 0 12px 26px rgba(0,0,0,0.28);
}

.project-video-box iframe {
  width: 100%;
  height: 260px;
}

/* ===========================
   Captions
   =========================== */
.project-caption-title {
  text-align: center;
  font-size: 20px;
  font-weight: 700;
  margin-top: 12px;
  color: #1e3a5f;
}

.project-caption-text {
  text-align: center;
  font-size: 15.5px;
  max-width: 90%;
  margin: 4px auto 0 auto;
  color: #555;
}

/* ===========================
   Architecture Image
   =========================== */
.project-arch-img {
  display: block;
  margin: 18px auto 35px auto;
  max-width: 700px;
  width: 65%;
  border-radius: 14px;
  box-shadow: 0 6px 20px rgba(0,0,0,0.18);
  transition: transform .3s ease;
}

/* Slight hover pop */
.project-arch-img:hover {
  transform: scale(1.02);
}

/* ===========================
   Divider
   =========================== */
.project-divider {
  height: 1px;
  width: 70%;
  background: #d0d4d9;
  margin: 38px auto;
}
</style>




<div class="project-page">

<div class="project-section-title">
Behavior Analysis of Car Drivers Based on Computer Vision
</div>

<div class="project-intro">
  <img src="/images/Intro.jpg" alt="Driver project intro">
  <div class="project-intro-text">
    The project develops an advanced driver assistance system (ADAS) using computer vision.
    By combining <b>YOLOv8</b>, <b>Optical Flow</b>, and <b>SSD</b> face detection, the system
    detects objects outside the vehicle while analyzing the driver’s head pose inside the car.
    <br><br>
    A <b>Voice Assistant</b> module informs the driver about potential dangers and traffic
    conditions to improve overall road safety.
  </div>
</div>

<div class="project-divider"></div>

<div class="project-section-title">System Components</div>

<div class="project-grid-2">

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1A2q3yyOWNahFMdCXNqwSgLiplSm0I8R8/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Head Direction Detection</div>
    <div class="project-caption-text">
      Uses SSD-based face detection to estimate the driver’s head direction.
    </div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/10NZdcjuLJwZpQkWyuejilv89bkpzwO8w/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Object Detection and Tracking</div>
    <div class="project-caption-text">
      YOLOv8 detects external objects while Optical Flow tracks their motion over time.
    </div>
  </div>

</div>

<div class="project-divider"></div>

<div class="project-section-title">Examples of the Running System</div>

<div class="project-grid-2">

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1OBGQBOWgTtPI4M-Lg9MHks1ceZ5gpF04/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Wake Up!</div>
    <div class="project-caption-text">Detects drowsiness and alerts the driver.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1SKdeQcPozlHjiXv1Xai9ZFWGEwpoZ0t2/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Traffic Light</div>
    <div class="project-caption-text">Identifies traffic lights ahead and warns the driver.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/175rLPKxnW_U6EwKj4D845NgkOWCcjafd/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Pedestrian</div>
    <div class="project-caption-text">Detects nearby pedestrians for safer driving.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1Xo7zvCDjAGA3eRQL3tgdRpmuObn_qE4a/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Look Left</div>
    <div class="project-caption-text">Warns about hazards approaching from the left side.</div>
  </div>

</div>

<div class="project-divider"></div>

-->

<div class="project-section-title">System Architecture</div>
<img src="/images/Architecture.jpg" class="project-arch-img" alt="System architecture diagram">

</div> <!-- END project-page -->
