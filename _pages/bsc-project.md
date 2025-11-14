---
layout: page
title: "Behavior Analysis of Car Drivers Using Computer Vision"
permalink: /driver-behavior/
---

# Behavior Analysis of Car Drivers Based on Computer Vision

<div align="center">
  <img src="/images/Intro.jpg" width="85%" alt="Driver behavior project intro image">
</div>

## Introduction

The project focuses on developing an advanced driver assistance system (ADAS) using computer vision.  
By combining **YOLOv8**, **Optical Flow**, and **SSD face detection**, the system detects objects outside the vehicle while analyzing the driver’s head pose inside the vehicle in real-time.  

To further improve safety, a **Voice Assistant** continuously informs the driver about dangers and traffic situations, helping reduce accidents and enhance overall driving awareness.

---

# System Components
<div align="center"><i>(videos are playable)</i></div>

<style>
.project-grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  margin-bottom: 40px;
}
.project-video {
  width: 100%;
  border-radius: 8px;
  overflow: hidden;
}
.project-text {
  font-size: 16px;
}
</style>

<div class="project-grid-2">

<!-- Head Pose -->
<div>
  <video class="project-video" controls>
    <source src="https://drive.google.com/uc?export=download&id=1A2q3yyOWNahFMdCXNqwSgLiplSm0I8R8" type="video/mp4">
  </video>
  <h3>Head Direction Detection</h3>
  <p class="project-text">
    This part of the system uses the Single Shot Detector (SSD) algorithm to detect the driver’s face and estimate their head direction with high accuracy.
  </p>
</div>

<!-- Object Detection -->
<div>
  <video class="project-video" controls>
    <source src="https://drive.google.com/uc?export=download&id=10NZdcjuLJwZpQkWyuejilv89bkpzwO8w" type="video/mp4">
  </video>
  <h3>Object Detection and Tracking</h3>
  <p class="project-text">
    YOLOv8 detects objects outside the car, and Optical Flow tracks them.  
    The system recognizes pedestrians, vehicles, traffic lights, bicycles, and more.
  </p>
</div>

</div>

---

# Examples of the Running System

<style>
.project-grid-2x2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  margin-bottom: 40px;
}
.project-item {
  margin-bottom: 30px;
}
</style>

<div class="project-grid-2x2">

<!-- Wake up -->
<div class="project-item">
  <video class="project-video" controls>
    <source src="https://drive.google.com/uc?export=download&id=1OBGQBOWgTtPI4M-Lg9MHks1ceZ5gpF04" type="video/mp4">
  </video>
  <h3>Wake Up!</h3>
  <p>The system detects drowsiness and alerts the driver to prevent accidents.</p>
</div>

<!-- Traffic Light -->
<div class="project-item">
  <video class="project-video" controls>
    <source src="https://drive.google.com/uc?export=download&id=1SKdeQcPozlHjiXv1Xai9ZFWGEwpoZ0t2" type="video/mp4">
  </video>
  <h3>Traffic Light</h3>
  <p>The system detects traffic lights ahead and informs the driver.</p>
</div>

<!-- Pedestrian -->
<div class="project-item">
  <video class="project-video" controls>
    <source src="https://drive.google.com/uc?export=download&id=175rLPKxnW_U6EwKj4D845NgkOWCcjafd" type="video/mp4">
  </video>
  <h3>Pedestrian</h3>
  <p>The system identifies pedestrians in front of the car and alerts the driver.</p>
</div>

<!-- Look Left -->
<div class="project-item">
  <video class="project-video" controls>
    <source src="https://drive.google.com/uc?export=download&id=1Xo7zvCDjAGA3eRQL3tgdRpmuObn_qE4a" type="video/mp4">
  </video>
  <h3>Look Left</h3>
  <p>
    A car enters from the left side while the driver looks right, so the system issues a warning about potential danger.
  </p>
</div>

</div>

---

# System Architecture

<div align="center">
  <img src="/images/Architecture.jpg" width="85%" alt="System Architecture Diagram">
</div>

<br>

The system integrates two subsystems—driver head pose estimation and external object detection—to generate a final fused decision for safe-driving alerts.

---
