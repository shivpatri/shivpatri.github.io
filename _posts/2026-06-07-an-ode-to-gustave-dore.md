---
layout: post
title:  "An Ode to Gustave Doré"
date:   2026-06-07 10:00:00 -0500
categories: Product
---

I've been hooked on Paradise Lost for the last few weeks. It's so ironic that a poet who aimed to justify the divine accidentally ended up writing the ultimate defense for the devil. It sets such a cool precedent for storytelling! It also makes you realize that whoever named Al Pacino's character 'John Milton' in The Devil's Advocate (1997) really did their research.

The poem undeniably deserves appreciation. But this post is not about the work itself. It's about how the illustrations to Paradise Lost, made by Gustave Doré, inspired me to build software as a tribute.

Gustave Doré (1832–1883) was a prolific French artist, printmaker, and illustrator whose work essentially defined how the 19th century—and much of the modern world—visualized classic literature. While he worked in painting and sculpture, he is most famous for his intricate, highly detailed wood engravings.

He had a unique genius for translating epic poetry and scripture into visual spectacles, achieving massive success with Dante's Divine Comedy and Cervantes' Don Quixote. But 1866 was the defining year of his career, seeing the publication of his two greatest masterpieces: La Grande Bible de Tours (The Doré Bible) and Milton's Paradise Lost.

<div style="display: flex; justify-content: space-between; gap: 15px; margin: 2rem 0;">
  <figure style="flex: 1; text-align: center; margin: 0;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/5/52/Paradise_Lost_14.jpg" alt="Satan on the Burning Lake" style="max-width: 100%; height: auto; border-radius: 4px;" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 0.75rem; line-height: 1.4;">Illustrating "Satan overlooking Paradise", from Book 9 of Paradise Lost: While physically looking at the breathtaking, uncorrupted beauty of the Garden of Eden, Satan carries the psychological scars of Hell with him. As Milton writes, "Which way I fly is Hell; myself am Hell."</figcaption>
  </figure>
  <figure style="flex: 1; text-align: center; margin: 0;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/d/d2/Paradiso_Canto_31.jpg" alt="Paradise Lost Illustration" style="max-width: 100%; height: auto; border-radius: 4px;" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 0.75rem; line-height: 1.4;">Illustrating the "Celestial Rose", Canto 31 of Dante's Paradiso:  Dante describes the souls of the blessed as the petals of a vast, glowing white rose surrounding God's radiant light.</figcaption>
  </figure>
  <figure style="flex: 1; text-align: center; margin: 0;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/9/9d/Destruction_of_Leviathan.png" alt="The Destruction of Leviathan" style="max-width: 100%; height: auto; border-radius: 4px;" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 0.75rem; line-height: 1.4;">Illustrating the leviathan, from Isaiah 27:1 of the Bible: "In that day the Lord with his sore and great and strong sword shall punish leviathan the piercing serpent..."</figcaption>
  </figure>
</div>


These dramatic, awe-inspiring visuals stuck with me, but I didn't just want to look at them once in a book or on a web page; I wanted to experience them organically. 

This got me thinking about two software experiences I absolutely love.

The first is [Windows Spotlight](https://learn.microsoft.com/en-us/windows/configuration/windows-spotlight/?pivots=windows-11). It's a built-in feature that automatically rotates your lock screen and desktop backgrounds, tagging them with geographic locations and well-curated trivia about the place you're looking at. Clicking the tag reveals a Bing map of the spot. It turns an otherwise static screen into a moment of ambient discovery.

<img src="https://learn.microsoft.com/en-us/windows/configuration/windows-spotlight/images/lockscreen-11.png" alt="Windows Spotlight" style="max-width: 100%; height: auto; margin: 1.5rem 0;" />

The second is [Google Arts & Culture](https://artsandculture.google.com/). It's a brilliant educational platform partnering with over 2,000 cultural institutions to bring high-resolution artworks, historical archives, and interactive exhibits to your screen. Whether you want to zoom in on the microscopic brushstrokes of Vincent van Gogh or wander through a virtual museum, the app perfectly bridges the gap between technology and history.

### The Birth of Wallpaper Genius

I realized I wanted to blend these three things: the breathtaking art of Gustave Doré, the ambient desktop rotation of Windows Spotlight, and the rich educational context of Google Arts & Culture. 

That inspiration led me to build **Wallpaper Genius**.

Wallpaper Genius is an app I created that automatically rotates my desktop background with high-resolution illustrations by Gustave Doré. But since a beautiful image without context loses some of its narrative power, I built a companion widget that populates alongside the wallpaper. 

Whenever the background changes, the widget updates to display:
- The **title** of the illustration.
- The **context** from the original work (like the specific verse from the Bible or lines from *Paradise Lost*).
- A brief **commentary** on the piece's historical or artistic significance.

To bring this to life, I built a native Mac app using Xcode. For the dynamic text generation—specifically crafting the context and commentary for each illustration—I integrated the Gemini API. Interestingly, the development process itself was a fun experiment in modern software engineering; I essentially "vibe coded" the entire application with the help of Codex and Gemini, letting AI assist me in seamlessly weaving together the logic and UI.

### How It Works

Here's a look at the application and its settings menu:

<div style="display: flex; gap: 15px; margin: 2rem 0; flex-wrap: wrap;">
  <figure style="flex: 1; min-width: 300px; text-align: center; margin: 0;">
    <img src="{{ '/_assets/images/WallpaperGenius.png' | relative_url }}" alt="Wallpaper and widgets" style="max-width: 100%; height: auto; border-radius: 4px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 0.75rem;">The desktop wallpaper alongside the dynamic Gemini-powered widgets.</figcaption>
  </figure>
  <figure style="flex: 1; min-width: 300px; text-align: center; margin: 0;">
    <img src="{{ '/_assets/images/AppUI.png' | relative_url }}" alt="App settings" style="max-width: 100%; height: auto; border-radius: 4px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" />
    <figcaption style="font-size: 0.85em; color: #555; margin-top: 0.75rem;">The Wallpaper Genius settings interface.</figcaption>
  </figure>
</div>

The app is designed to be very simple to configure. You can use the **"browse folder"** option to point it to your own downloaded collection of illustrations. In the settings, there is a text field to securely input your **Gemini API key**, alongside a dropdown for **model selection** (so you can choose which Gemini model generates the widget text), and customizable controls like **rotation frequency** to dictate how often your desktop background updates.

### Downloads

If you'd like to try it out yourself, I've gathered everything you need below:

- ⬇️ **[Download Wallpaper Genius App (.dmg)]({{ '/_assets/downloads/WallpaperGenius.dmg' | relative_url }})**
- 🖼️ **[Gustave Doré's La Grande Bible de Tours (.torrent)]({{ '/_assets/downloads/dore_bible.torrent' | relative_url }})**
- 🖼️ **[Gustave Doré's Paradise Lost Illustrations (.zip)]({{ '/_assets/downloads/paradise_lost.zip' | relative_url }})**

Building Wallpaper Genius has been an incredible way to turn my everyday digital workspace into a personal, rotating museum—a small daily tribute to epic poetry and masterful engraving.