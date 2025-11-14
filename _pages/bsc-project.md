---
layout: page
title: "Behavior Analysis of Car Drivers Using Computer Vision"
permalink: /driver-behavior/
---

# Behavior Analysis of Car Drivers Based on Computer Vision

<!-- Intro Image -->
<div style="text-align:center; margin-bottom:30px;">
  <img src="/images/Intro.jpg" style="max-width:60%; border-radius:10px;" alt="Driver Behavior Intro Image">
</div>

## Introduction

The project focuses on developing an advanced driver assistance system (ADAS) using computer vision.  
By combining **YOLOv8**, **Optical Flow**, and **SSD face detection**, the system detects objects outside the vehicle while analyzing the driver’s head pose inside the vehicle.  

To further improve safety, a **Voice Assistant** continuously informs the driver about dangers and traffic conditions.

---

# System Components
<div align="center"><i>(videos are clickable)</i></div>

<style>
.video-grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 25px;
  margin-top: 20px;
  margin-bottom: 40px;
  justify-items: center;
}
.video-box iframe {
  width: 100%;
  max-width: 420px;
  height: 240px;
  border-radius: 10px;
}
.section-text {
  max-width: 420px;
}
</style>

<div class="video-grid-2">

<!-- Head Pose -->
<div>
  <div class="video-box">
    <iframe src="https://drive.google.com/file/d/1A2q3yyOWNahFMdCXNqwSgLiplSm0I8R8/preview" allow="autoplay"></iframe>
  </div>
  <h3>Head Direction Detection</h3>
  <p class="section-text">
    This part of the system uses the SSD algorithm to detect the driver's face and estimate their head direction accurately.
  </p>
</div>

<!-- Object Detection -->
<div>
  <div class="video-box">
    <iframe src="https://drive.google.com/file/d/10NZdcjuLJwZpQkWyuejilv89bkpzwO8w/preview" allow="autoplay"></iframe>
  </div>
  <h3>Object Detection and Tracking</h3>
  <p class="section-text">
    YOLOv8 detects objects outside the vehicle and Optical Flow tracks them. The system identifies pedestrians, cars, bicycles, and more.
  </p>
</div>

</div>

---

# Examples of the Running System

<style>
.video-grid-2x2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 25px;
  justify-items: center;
  margin-bottom: 40px;
}
</style>

<div class="video-grid-2x2">

<!-- Wake Up -->
<div>
  <div class="video-box">
    <iframe src="https://drive.google.com/file/d/1OBGQBOWgTtPI4M-Lg9MHks1ceZ5gpF04/preview" allow="autoplay"></iframe>
  </div>
  <h3>Wake Up!</h3>
  <p>The system detects driver drowsiness and issues alerts.</p>
</div>

<!-- Traffic Light -->
<div>
  <div class="video-box">
    <iframe src="https://drive.google.com/file/d/1SKdeQcPozlHjiXv1Xai9ZFWGEwpoZ0t2/preview" allow="autoplay"></iframe>
  </div>
  <h3>Traffic Light</h3>
  <p>The system detects traffic lights ahead and warns the driver.</p>
</div>

<!-- Pedestrian -->
<div>
  <div class="video-box">
    <iframe src="https://drive.google.com/file/d/175rLPKxnW_U6EwKj4D845NgkOWCcjafd/preview" allow="autoplay"></iframe>
  </div>
  <h3>Pedestrian</h3>
  <p>The system identifies pedestrians in front of the car.</p>
</div>

<!-- Look Left -->
<div>
  <div class="video-box">
    <iframe src="https://drive.google.com/file/d/1Xo7zvCDjAGA3eRQL3tgdRpmuObn_qE4a/preview" allow="autoplay"></iframe>
  </div>
  <h3>Look Left</h3>
  <p>A car enters from the left while the driver looks right, and the system warns of danger.</p>
</div>

</div>

---

# System Architecture

<div style="text-align:center;">
  <img src="/images/Architecture.jpg" style="max-width:70%; border-radius:10px;">
</div>

<br>
<p style="max-width:700px; margin:auto;">
The system integrates two subsystems—driver head pose estimation and external object detection—to generate a fused safety decision for real-time driving assistance.
</p>

---
