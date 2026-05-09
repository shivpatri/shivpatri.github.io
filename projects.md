---
layout: page
title: Projects
---
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
  .project-tags {
    display: flex;
    gap: 4px;
    flex-wrap: wrap;
    margin-top: 0.5rem;
  }
  .project-tag {
    padding: 2px 6px;
    background-color: #e0e7ff;
    color: #3730a3;
    border-radius: 4px;
    font-size: 0.65rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
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
  h2 {
    font-size: 1.25rem !important;
    text-align: left !important;
    border-bottom: 1px solid #eaeaea;
    padding-bottom: 0.5rem;
    margin-top: 2.5rem !important;
    margin-bottom: 1rem !important;
  }
  .section-description {
    font-size: 0.9rem;
    color: #555;
    margin-bottom: 1.5rem;
  }
</style>

## Algorithms

## Image Processing

<p class="section-description">I was a little late to the deep learning party, so I did these feature engineering projects on my way.</p>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="{{ '/_assets/images/projects/d_4065_1-left_cc-e1506943826655.png' | relative_url }}" alt="Breast Lesion Contours">
  </div>
  <div class="project-info">
    <h3>Feature engineering to classify lesions in mammograms.</h3>
    <div class="project-meta"> Under Graduate Research | BITS Pilani | December 2014 </div>
    <p>A novel technique using simple polynomial regression on lesion contour signatures to classify mammograms into benign and malignant classes.</p>
    <div class="project-tags">
      <span class="project-tag">MATLAB</span>
      <span class="project-tag">Image Procesing</span>
    </div>
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
    <div class="project-meta"> Summer Internship | Supreme Industries | May 2014 </div>
    <p> A count of circular pipes in an image is calculated using Image Segmentation and Hough's circle transform.</p>
    <div class="project-tags">
      <span class="project-tag">MATLAB</span>
      <span class="project-tag">Image Processing</span>
    </div>
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
    <h3> A medical imaging prototype to detect glaucoma.</h3>
    <div class="project-meta"> 5th "Engineering the Eye" Hackathon | L.V Prasad Eye Institute | July 2017 </div>
    <p>A 3-D printed optical setup with lenses and slits, a raspberry pi and a camera make for an portable eye imaging device that measures the ratio between the Anterior Chamber Depth and Corneal thickness. This metric is an estimate for intra-ocular pressure, an indicator of glaucoma.</p>
    <div class="project-tags">
      <span class="project-tag">Raspberry Pi</span>
      <span class="project-tag">Python</span>
      <span class="project-tag">OpenCV</span>
    </div>
    <div class="project-badges">
      <a href="{{ '/_assets/docs/projects/final-project-documentation.pdf' | relative_url }}" class="project-badge">📄 Documentation</a>
    </div>
  </div>
</div>

## Analog Electronics

<p class="section-description">My undergraduate major was Electronics & Communications, so I romanced with the field before finding my true love: AI and software engineering.</p>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="{{ '/_assets/images/projects/adc-e1506946445701.png' | relative_url }}" alt="Delta-Sigma ADC">
  </div>
  <div class="project-info">
    <h3> An analog to digital converter for temperature sensing.</h3>
    <div class="project-meta"> Internship | Intel, Bangalore | December 2015 </div>
    <p>System-level schematic design of a Thermal Sensor IP with a sigma-delta ADC using behavioral Verilog-A/AMS models to ensure PDK independence and ease of porting.</p>
    <div class="project-tags">
      <span class="project-tag">Cadence Virtuoso</span>
      <span class="project-tag">Verilog-A/AMS</span>
    </div>
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
    <h3> A 14nm operational amplifier.</h3>
    <div class="project-meta"> Internship | Intel, Bangalore | August 2015 </div>
    <p>Schematic design of a simple two-stage operational amplifier using a 14nm Process Development Kit. Simulated and verified results across PVT corners.</p>
    <div class="project-tags">
      <span class="project-tag">Cadence Virtuoso</span>
      <span class="project-tag">Cadence Spectre</span>
      <span class="project-tag">14nm PDK</span>
    </div>
    <div class="project-badges">
      <a href="{{ '/_assets/docs/projects/document.pdf' | relative_url }}" class="project-badge">📄 Documentation</a>
    </div>
  </div>
</div>