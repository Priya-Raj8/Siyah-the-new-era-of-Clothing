# 🏔️ SIYAH — Premium Indian Ethnic Wear Landing Page

> **Acdyon Technologies Take-Home Assessment (Track 2: Premium Home Page)**  
> *A fresh, modern frontend landing page created for SIYAH — an authentic ethnic wear brand born in Himachal Pradesh.*

🌐 **Live Website Link**: **[https://priya-raj8.github.io/Siyah-the-new-era-of-Clothing/](https://priya-raj8.github.io/Siyah-the-new-era-of-Clothing/)**  
📂 **GitHub Repository**: **[https://github.com/Priya-Raj8/Siyah-the-new-era-of-Clothing](https://github.com/Priya-Raj8/Siyah-the-new-era-of-Clothing)**

---

## 👋 Why I Built This

A few days ago, I stumbled upon **SIYAH** on social media after reading about their appearance on *Shark Tank India* and how they grew from 10 retail outlets across Himachal Pradesh. I was curious to check out their collection, but when I tried visiting their official website, it wasn't working. 

When I received this take-home assessment for Acdyon Technologies, I decided to build a landing page specifically for SIYAH. Given the tight time constraints, I chose **Track 2 (Premium Home Page)** so I could dedicate my time to polishing the UI, crafting smooth animations, and creating a shopping experience that feels authentic to Indian ethnic fashion.

---

## 🌟 Visual Preview

![SIYAH Desktop Preview](desktop_preview.png)

---

## 💡 What Makes This Unique

Instead of relying on heavy third-party libraries, I wanted to keep the codebase clean, fast, and light. Here are a few details I built into the page:

1. **Swaying Saree Pallu (Inline SVG Animation)**: 
   Rather than loading a 2MB+ 3D canvas library, I created a dual-layer SVG ribbon background with CSS keyframe motion and dotted zari borders. It runs smoothly at 60 FPS without draining battery life on mobile.

2. **Live Drape Shade Studio**: 
   Right below the hero section, visitors can click color dots (*Rani Pink*, *Marigold Gold*, *Forest Green*, *Plum Silk*) to live-morph the background saree ribbons in real-time.

3. **Honest Price Math Breakdown Modal**: 
   Ethnic wear often suffers from 4x festival markups. Clicking "View Price Math" on any product card opens a breakdown showing exact fabric costs, master tailoring costs, and logistics vs traditional retail markups.

4. **Gold Zari Sparkle Cursor Trail**: 
   Moving the mouse over the hero section leaves a subtle trail of gold and rani pink zari sparkles using an HTML5 Canvas particle engine.

5. **Real-time Launch Countdown Ticker**: 
   A top notification bar with a live countdown timer (`03d : 14h : 22m : 45s`) to build anticipation for the online launch.

6. **Honesty-First Promise**: 
   No fake testimonials or fabricated "10,000+ happy buyers" counts — just real craft, transparent pricing, and limited small-batch drops.

---

## 📂 Project Structure

```
├── index.html           # Main landing page (HTML5, CSS3, Vanilla JS)
├── DECISIONS.md        # My personal design & engineering decisions write-up
├── README.md           # This project guide & live links
├── desktop_preview.png  # Desktop screenshot preview
└── mobile_preview.png   # Mobile responsiveness preview
```

---

## 🛠️ How to Run Locally

You don't need any complex installation steps to run this project:

1. Clone the repository:
   ```bash
   git clone https://github.com/Priya-Raj8/Siyah-the-new-era-of-Clothing.git
   ```
2. Open `index.html` directly in your web browser, or serve it locally:
   ```bash
   npx http-server -p 8000
   ```
3. Visit `http://localhost:8000`.

---

## 📝 Engineering Decisions

For my detailed breakdown on trade-offs, AI usage transparency, and what I would build with a full week, take a look at [`DECISIONS.md`](DECISIONS.md).
