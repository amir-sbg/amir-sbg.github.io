---
layout: default
title: "Behavior Analysis of Car Drivers Based on Computer Vision"
permalink: /driver-behavior/
author_profile: true
---

<span class='anchor' id='driver-behavior'></span>

<div class="project-page driver-behavior-page">

<div class="project-section-title project-hero-title">
Behavior Analysis of Car Drivers Based on Computer Vision
</div>

<div class="project-action-row">
  <a class="btn btn--primary" href="https://github.com/amir-sbg/Behavior-Analysis-of-Car-Drivers-Based-on-Computer-Vision" target="_blank" rel="noopener noreferrer">
    <i class="fab fa-github" aria-hidden="true"></i> GitHub Repository
  </a>
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

<div class="project-section-title">End-to-End ADAS Workflow</div>

<div class="project-workflow">
  <img src="/images/driver-behavior/adas-workflow-full.gif" alt="Animated workflow of the driver-behavior analysis system">
  <div class="project-caption-text">
    The full pipeline processes the forward road view and the in-cabin camera in parallel. YOLOv8 identifies road users and traffic objects, optical flow adds temporal motion cues, and face/head-direction analysis estimates whether the driver is attentive. These signals are combined by the warning logic to produce timely spoken safety alerts.
  </div>
  <div class="project-caption-text">
    <strong>Full system demonstration:</strong>
    <a href="https://drive.google.com/file/d/1oFX282GvolzIu95fmWailKjWrnFShlqV/view?usp=drive_link" target="_blank" rel="noopener noreferrer">watch the project video on Google Drive</a> to see the perception and alert modules operating together on driving footage.
  </div>
</div>

<!-- Embedded project video temporarily hidden.
<div class="project-local-video">
  <video controls playsinline preload="metadata">
    <source src="/images/driver-behavior/adas-overview.mp4" type="video/mp4">
    Your browser does not support embedded video. <a href="/images/driver-behavior/adas-overview.mp4">Download the project video</a>.
  </video>
  <div class="project-caption-title">System Demonstration</div>
  <div class="project-caption-text">
    A full-resolution demonstration of the perception and alert pipeline running together.
  </div>
</div>
-->

<div class="project-divider"></div>

<div class="project-section-title">Core Perception Components</div>

<div class="project-grid-2 project-grid-featured-videos">

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1A2q3yyOWNahFMdCXNqwSgLiplSm0I8R8/preview" title="In-cabin head-direction monitoring demonstration" allow="autoplay" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="project-caption-title">In-Cabin Head-Direction Monitoring</div>
    <div class="project-caption-text">
      An SSD-based detector first localizes the driver’s face, after which head orientation is estimated across successive frames. The temporal signal helps distinguish normal mirror checks from sustained attention loss and supplies the in-cabin evidence used by the warning system.
    </div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/10NZdcjuLJwZpQkWyuejilv89bkpzwO8w/preview" title="Road-scene object detection and motion tracking demonstration" allow="autoplay" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="project-caption-title">Road-Scene Detection and Motion Tracking</div>
    <div class="project-caption-text">
      YOLOv8 detects vehicles, pedestrians, traffic lights, and other relevant road objects in the forward camera stream. Optical flow then follows their frame-to-frame movement, adding direction and motion context that a single detection frame cannot provide.
    </div>
  </div>

</div>

<div class="project-divider"></div>

<div class="project-section-title">Safety Alerts in the Running System</div>

<div class="project-grid-2">

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1OBGQBOWgTtPI4M-Lg9MHks1ceZ5gpF04/preview" title="Driver drowsiness warning demonstration" allow="autoplay" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="project-caption-title">Drowsiness Alert — “Wake Up”</div>
    <div class="project-caption-text">The in-cabin stream identifies a sustained inattentive or drowsy head state. Once the condition persists beyond the decision threshold, the voice assistant issues an immediate wake-up warning rather than reacting to a single noisy frame.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1SKdeQcPozlHjiXv1Xai9ZFWGEwpoZ0t2/preview" title="Traffic-light awareness demonstration" allow="autoplay" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="project-caption-title">Traffic-Light Awareness</div>
    <div class="project-caption-text">The forward camera detects a traffic light in the driving corridor and passes the event to the alert layer. The example shows how road-scene perception is translated into a concise spoken cue for the driver.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/175rLPKxnW_U6EwKj4D845NgkOWCcjafd/preview" title="Pedestrian proximity warning demonstration" allow="autoplay" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="project-caption-title">Pedestrian Proximity Warning</div>
    <div class="project-caption-text">A pedestrian is localized in the road scene and tracked as the vehicle approaches. Combining object identity with temporal motion makes the warning more informative than an isolated bounding-box detection.</div>
  </div>

  <div>
    <div class="project-video-box">
      <iframe src="https://drive.google.com/file/d/1Xo7zvCDjAGA3eRQL3tgdRpmuObn_qE4a/preview" title="Left-side hazard warning demonstration" allow="autoplay" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="project-caption-title">Left-Side Hazard Warning</div>
    <div class="project-caption-text">The perception stream detects relevant activity on the vehicle’s left side while the driver-monitoring signal indicates where attention is directed. The assistant responds with a specific “look left” cue to connect the observed hazard with an actionable check.</div>
  </div>

</div>

<div class="project-divider"></div>

<div class="project-section-title">System Architecture</div>
<img src="/images/driver-behavior/system-architecture.png" class="project-arch-img" alt="System architecture diagram for the driver-behavior analysis pipeline">

</div> <!-- END project-page -->
