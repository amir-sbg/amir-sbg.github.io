---
layout: page
title: "Behavior Analysis of Car Drivers Based on Computer Vision"
permalink: /driver-behavior/
---

<style>
/* overall layout */
.section-title {
    text-align: center;
    font-size: 34px;
    font-weight: 700;
    margin-top: 40px;
    margin-bottom: 25px;
}

/* intro image */
.intro-img {
    width: 80%;
    max-width: 900px;
    display: block;
    margin: 0 auto 20px auto;
    border-radius: 12px;
    box-shadow: 0 4px 14px rgba(0,0,0,0.15);
}

/* intro text */
.intro-text {
    width: 80%;
    max-width: 900px;
    margin: 0 auto;
    font-size: 18px;
    line-height: 1.6;
}

/* grid layout */
.grid-2 {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(360px, 1fr));
    grid-gap: 40px;
    width: 90%;
    margin: 0 auto;
}

/* video styling */
.video-box {
    width: 100%;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

.video-box iframe,
.video-box video {
    width: 100%;
    height: 240px;
    object-fit: cover;
}

.caption-title {
    text-align: center;
    font-size: 20px;
    font-weight: 700;
    margin-top: 10px;
}

.caption-text {
    text-align: center;
    font-size: 16px;
    width: 85%;
    margin: 0 auto;
}

/* architecture image */
.arch-img {
    width: 80%;
    max-width: 900px;
    display: block;
    margin: 20px auto;
    border-radius: 10px;
    box-shadow: 0 4px 14px rgba(0,0,0,0.15);
}

/* subtle divider */
.divider {
    height: 1px;
    width: 70%;
    background: #ccc;
    margin: 40px auto;
}
</style>


<!-- INTRO SECTION -->
<div class="section-title">Introduction</div>

<img src="/images/Intro.jpg" class="intro-img"/>

<div class="intro-text">
The project focuses on developing an advanced driver assistance system (ADAS) using computer vision.  
By combining <b>YOLOv8</b>, <b>Optical Flow</b>, and <b>SSD face detection</b>, the system detects objects outside the vehicle while analyzing the driver’s head pose inside the vehicle.

To further improve safety, a <b>Voice Assistant</b> continuously informs the driver about dangers and traffic conditions.
</div>

<div class="divider"></div>


<!-- SYSTEM COMPONENTS -->
<div class="section-title">System Components</div>

<p style="text-align:center; font-style:italic; margin-top:-15px;">(videos are clickable)</p>

<div class="grid-2">

    <!-- Head Direction -->
    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1A2q3yyOWNahFMdCXNqwSgLiplSm0I8R8/preview" allow="autoplay"></iframe>
        </div>
        <div class="caption-title">Head Direction Detection</div>
        <div class="caption-text">
            This part of the system uses the SSD algorithm to detect the driver's face and estimate head direction with high accuracy.
        </div>
    </div>

    <!-- Object detection -->
    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/10NZdcjuLJwZpQkWyuejilv89bkpzwO8w/preview" allow="autoplay"></iframe>
        </div>
        <div class="caption-title">Object Detection and Tracking</div>
        <div class="caption-text">
            YOLOv8 detects surrounding objects, and Optical Flow tracks them. The system recognizes pedestrians, vehicles, traffic lights, and more.
        </div>
    </div>

</div>

<div class="divider"></div>



<!-- DEMO SECTION -->
<div class="section-title">Examples of the Running System</div>

<div class="grid-2">

    <!-- Wake Up -->
    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1OBGQBOWgTtPI4M-Lg9MHks1ceZ5gpF04/preview"></iframe>
        </div>
        <div class="caption-title">Wake Up!</div>
        <div class="caption-text">The system detects driver drowsiness and alerts the driver to prevent accidents.</div>
    </div>

    <!-- Traffic Light -->
    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1SKdeQcPozlHjiXv1Xai9ZFWGEwpoZ0t2/preview"></iframe>
        </div>
        <div class="caption-title">Traffic Light</div>
        <div class="caption-text">The system detects traffic lights ahead and informs the driver.</div>
    </div>

    <!-- Pedestrian -->
    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/175rLPKxnW_U6EwKj4D845NgkOWCcjafd/preview"></iframe>
        </div>
        <div class="caption-title">Pedestrian</div>
        <div class="caption-text">The system detects nearby pedestrians and warns the driver.</div>
    </div>

    <!-- Look Left -->
    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1Xo7zvCDjAGA3eRQL3tgdRpmuObn_qE4a/preview"></iframe>
        </div>
        <div class="caption-title">Look Left</div>
        <div class="caption-text">The system identifies hazards from the left side and alerts the driver.</div>
    </div>

</div>

<div class="divider"></div>


<!-- ARCHITECTURE SECTION -->
<div class="section-title">System Architecture</div>

<img src="/images/Architecture.jpg" class="arch-img"/>

