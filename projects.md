---
layout: page
title: Projects
---

Here are some of the projects I have been working on.

<style>
  .project-card {
    display: flex;
    flex-wrap: wrap;
    align-items: flex-start;
    margin-bottom: 1.5rem;
    padding: 0.75rem 1rem;
    border: 1px solid #eaeaea;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.02);
    background-color: #ffffff;
    transition: background-color 0.2s ease;
    overflow: hidden;
  }
  .project-card:hover {
    background-color: #f9fafb;
  }
  .project-thumbnail {
    flex: 0 0 140px;
    max-width: 140px;
    height: 198px; /* 140px width * 1.414 aspect ratio = 198px */
    margin-right: 1.25rem;
    overflow: hidden;
  }
  .project-thumbnail img {
    display: block;
    width: 100%;
    height: 100% !important;
    margin: 0 !important;
    border-radius: 4px;
    object-fit: cover;
    border: 1px solid #f1f1f1;
  }
  .project-info {
    flex: 2 1 300px;
    display: flex;
    flex-direction: column;
    height: 198px; /* Strictly match the image height */
    overflow: hidden;
  }
  .project-info h3 {
    margin-top: 0 !important;
    margin-bottom: 0.25rem;
    font-size: 1.15rem;
    line-height: 1.2;
  }
  .project-meta {
    font-size: 0.75rem;
    color: #6b7280;
    margin-bottom: 0.35rem;
  }
  .project-info p {
    margin-bottom: auto;
    font-size: 0.8rem;
    color: #555;
    line-height: 1.4;
    display: -webkit-box;
    -webkit-line-clamp: 4; /* Gracefully truncates text that exceeds 4 lines */
    -webkit-box-orient: vertical;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .project-badges {
    display: flex;
    gap: 6px;
    flex-wrap: wrap;
    margin-top: 0.5rem;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
  }
  .project-badge {
    display: inline-flex;
    align-items: center;
    padding: 3px 8px;
    background-color: #f3f4f6;
    color: #24292e !important;
    text-decoration: none !important;
    border-radius: 5px;
    font-size: 0.7rem;
    border: 1px solid #d1d5db;
    font-weight: 500;
    transition: background-color 0.2s ease, border-color 0.2s ease;
  }
  .project-badge:hover {
    background-color: #e5e7eb;
    border-color: #9ca3af;
  }
</style>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="{{ '/_assets/images/projects/d_4065_1-left_cc-e1506943826655.png' | relative_url }}" alt="Breast Lesion Contours">
  </div>
  <div class="project-info">
    <h3>Feature engineering for classifying lesions in mammograms.</h3>
    <div class="project-meta">📍 Under Graduate Researcher | BITS Pilani</div>
    <p>A new algorithm for feature extraction using polynomial regression on the signatures of benign and malignant contours. Built using MATLAB image processing & machine learning toolboxes.</p>
    <div class="project-badges">
      <a href="http://ieeexplore.ieee.org/document/7150808/" class="project-badge">📄 Publication</a>
      <a href="https://github.com/shivakshit/BenignMalignantClassification" class="project-badge">💻 Code</a>
    </div>
  </div>
</div>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="{{ '/_assets/images/projects/pipe.jpeg' | relative_url }}" alt="Circular Plastic Pipes">
  </div>
  <div class="project-info">
    <h3> Counting plastic pipes.</h3>
    <div class="project-meta">📍 Summer Intern | Supreme Industries</div>
    <p>Software written in MATLAB that applies image segmentation & Hough's circle transform to count the number of circular pipes in an image. Includes a UI for image upload and visualization.</p>
    <div class="project-badges">
      <a href="{{ '/_assets/docs/projects/project-2.docx' | relative_url }}" class="project-badge">📄 Documentation</a>
      <a href="https://github.com/shivakshit/supremeProject" class="project-badge">💻 Code</a>
    </div>
  </div>
</div>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="{{ '/_assets/images/projects/acdc.png' | relative_url }}" alt="ACDC Measurement Device">
  </div>
  <div class="project-info">
    <h3> A 3D printed, raspberry pi based imaging device to detect Glaucoma.</h3>
    <div class="project-meta">📍 Team Lead | LVPEI Engineering the Eye Hackathon</div>
    <p>A 3-D printed prototype that measures the ratio between the Anterior Chamber Depth and Corneal thickness. Built using Raspberry Pi, Pi Camera, Flask, and OpenCV.</p>
    <div class="project-badges">
      <a href="{{ '/_assets/docs/projects/final-project-documentation.pdf' | relative_url }}" class="project-badge">📄 Documentation</a>
      <a href="https://github.com/shivakshit/ACDC" class="project-badge">💻 Code</a>
    </div>
  </div>
</div>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="{{ '/_assets/images/projects/adc-e1506946445701.png' | relative_url }}" alt="Delta-Sigma ADC">
  </div>
  <div class="project-info">
    <h3> An Analog to Digital Converter for Temperature Sensing</h3>
    <div class="project-meta">📍 Circuit Design Intern | Intel Corporation, Bangalore</div>
    <p>Architecture Definition and System level Design. Schematic Design of the entire Thermal Sensor IP in Cadence Virtuoso design environment using Analog-A/AMS modeled devices.</p>
    <div class="project-badges">
      <a href="{{ '/_assets/docs/projects/document1.pdf' | relative_url }}" class="project-badge">📄 Documentation</a>
    </div>
  </div>
</div>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="{{ '/_assets/images/projects/opamp.png' | relative_url }}" alt="2-stage Operational Amplifier">
  </div>
  <div class="project-info">
    <h3> A 14nm Operational Amplifier</h3>
    <div class="project-meta">📍 Circuit Design Intern | Intel Corporation, Bangalore</div>
    <p>Schematic design of a simple miller-compensated two stage operational amplifier using a 14nm PDK. Simulated and verified results across PVT corners in Cadence Spectre.</p>
    <div class="project-badges">
      <a href="{{ '/_assets/docs/projects/document.pdf' | relative_url }}" class="project-badge">📄 Documentation</a>
    </div>
  </div>
</div>