---
layout: default
title: "Behavior Analysis of Car Drivers Based on Computer Vision"
permalink: /driver-behavior/
---

<style>
body {
    background: #f6f7f9;
}

/* Title */
.section-title {
    text-align: center;
    font-size: 34px;
    font-weight: 700;
    margin-top: 40px;
}

/* Intro Section */
.intro-container {
    display: grid;
    grid-template-columns: 1fr 1.3fr;
    align-items: center;
    background: white;
    padding: 30px;
    width: 90%;
    margin: 0 auto;
    border-radius: 16px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.10);
}

.intro-image {
    width: 100%;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

.intro-text {
    padding-left: 30px;
    font-size: 18px;
    line-height: 1.55;
}

/* 2-column grid */
.grid-2 {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 40px;
    width: 90%;
    margin: 0 auto;
}

/* Videos */
.video-box {
    width: 100%;
    border-radius: 12px;
    overflow: hidden;
    background: black;
    box-shadow: 0 4px 12px rgba(0,0,0,0.20);
}

.video-box iframe {
    width: 100%;
    height: 250px;
}

/* Captions */
.caption-title {
    text-align: center;
    font-size: 20px;
    font-weight: 700;
    margin-top: 12px;
}

.caption-text {
    text-align: center;
    margin: 0 auto;
    font-size: 16px;
    width: 90%;
}

/* Architecture */
.arch-img {
    width: 60%;
    display: block;
    margin: 20px auto;
    border-radius: 12px;
    box-shadow: 0 4px 14px rgba(0,0,0,0.15);
}

.divider {
    height: 1px;
    width: 75%;
    background: #ccc;
    margin: 45px auto;
}
</style>


<!-- TITLE -->
<div class="section-title">Behavior Analysis of Car Drivers Based on Computer Vision</div>


<!-- INTRO -->
<div class="intro-container">
    <img src="/images/Intro.jpg" class="intro-image">

    <div class="intro-text">
        The project focuses on developing an advanced driver assistance system (ADAS) using computer vision.
        By combining <b>YOLOv8</b>, <b>Optical Flow</b>, and <b>SSD face detection</b>, the system detects
        objects outside the vehicle while analyzing the driver’s head pose inside the car.

        <br><br>A <b>Voice Assistant</b> informs the driver about dangers and traffic conditions in real time.
    </div>
</div>

<div class="divider"></div>


<!-- SYSTEM COMPONENTS -->
<div class="section-title">System Components</div>

<div class="grid-2">
    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1A2q3yyOWNahFMdCXNqwSgLiplSm0I8R8/preview"></iframe>
        </div>
        <div class="caption-title">Head Direction Detection</div>
        <div class="caption-text">Uses SSD face detection to estimate head direction accurately.</div>
    </div>

    <div>
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/10NZdcjuLJwZpQkWyuejilv89bkpzwO8w/preview"></iframe>
        </div>
        <div class="caption-title">Object Detection and Tracking</div>
        <div class="caption-text">
            YOLOv8 detects objects outside the vehicle, while Optical Flow tracks motion.
        </div>
    </div>
</div>

<div class="divider"></div>


<!-- DEMOS -->
<div class="section-title">Examples of the Running System</div>

<div class="grid-2">
    <div>
        <div class="video-box">
            <ifra
