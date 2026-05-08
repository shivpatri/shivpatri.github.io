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
    <img src="https://images.unsplash.com/photo-1555949963-aa79dcee981c?q=80&w=250&h=150&fit=crop" alt="Project 1">
  </div>
  <div class="project-info">
    <h3>Computer Vision Pipeline</h3>
    <div class="project-meta">🗓 Aug 2022 - Dec 2022 | 📍 University of XYZ</div>
    <p>A brief description of your project goes here. Explain the core functionality, the technologies and frameworks used (e.g., PyTorch, OpenCV), and the problem it solves. Inspired by the layout seen on Papers with Code.</p>
    <div class="project-badges">
      <a href="#" class="project-badge">▶ Demo</a>
      <a href="#" class="project-badge">📄 Documentation</a>
      <a href="#" class="project-badge">💻 Code</a>
    </div>
  </div>
</div>

<div class="project-card">
  <div class="project-thumbnail">
    <img src="https://images.unsplash.com/photo-1526374965328-7f61d4dc18c5?q=80&w=250&h=150&fit=crop" alt="Project 2">
  </div>
  <div class="project-info">
    <h3>Natural Language Processing Model</h3>
    <div class="project-meta">🗓 Jan 2023 - May 2023 | 📍 Remote</div>
    <p>This project features a transformer-based language model trained to summarize dense technical documentation. It utilizes HuggingFace's transformers library and is deployed as a lightweight API.</p>
    <div class="project-badges">
      <a href="#" class="project-badge">▶ Demo</a>
      <a href="#" class="project-badge">📄 Documentation</a>
      <a href="#" class="project-badge">💻 Code</a>
    </div>
  </div>
</div>