---
layout: default
title: "Behavior Analysis of Car Drivers Based on Computer Vision"
permalink: /driver-behavior/
author_profile: true
---

<span class='anchor' id='driver-behavior'></span>

<div class="project-page">

<div class="project-section-title">
Behavior Analysis of Car Drivers Based on Computer Vision
</div>

<div class="project-intro">
  <img src="/images/Intro.jpg" alt="Driver project intro">
<div class="project-intro-text">
  This project builds an integrated advanced driver assistance system (ADAS) powered by computer vision. 
  It combines <b>YOLOv8</b> for exterior object detection, <b>Optical Flow</b> for motion tracking, 
  and an <b>SSD-based</b> face detector for monitoring the driver’s head pose inside the vehicle.
  <br><br>
  A built-in <b>Voice Assistant</b> provides real-time alerts about hazards, surrounding traffic, 
  and driver inattention, enhancing overall road safety.
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
    <div class="project-caption-title">Wake Up! 😴➡️⚠️</div>
    <div class="project-caption-text">Detects drowsiness and alerts the driver.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1SKdeQcPozlHjiXv1Xai9ZFWGEwpoZ0t2/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Traffic Light 🚦</div>
    <div class="project-caption-text">Identifies traffic lights ahead and warns the driver.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/175rLPKxnW_U6EwKj4D845NgkOWCcjafd/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Pedestrian 🚶‍♂️</div>
    <div class="project-caption-text">Detects nearby pedestrians for safer driving.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1Xo7zvCDjAGA3eRQL3tgdRpmuObn_qE4a/preview" allow="autoplay"></iframe>
    </div>
    <div class="project-caption-title">Look Left 👈</div>
    <div class="project-caption-text">Warns about hazards approaching from the left side.</div>
  </div>

</div>

<div class="project-divider"></div>

<div class="project-section-title">System Architecture</div>
<img src="/images/Architecture.jpg" class="project-arch-img" alt="System architecture diagram">

</div> <!-- END project-page -->
