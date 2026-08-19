# Engineering & Design Decisions — SIYAH Landing Page

**Candidate Submission**: Acdyon Technologies Frontend Take-Home Assessment  
**Track Selected**: Track 2 — Premium Home Page  
**Brand Chosen**: **SIYAH** (Indian Ethnic Wear: Sarees, Kurtis & 3-Piece Suit Sets)  
**Live Site Link**: **[https://priya-raj8.github.io/Siyah-the-new-era-of-Clothing/](https://priya-raj8.github.io/Siyah-the-new-era-of-Clothing/)**

---

## 1. Why I Chose Track 2 & My Real-Life Inspiration for SIYAH

When reviewing the assessment options under tight time constraints, I decided to choose **Track 2 (Premium Home Page)** over Track 1 so I could dedicate 100% of my focus to frontend craft, smooth animations, and visual polish within the submission deadline.

My decision to build specifically for **SIYAH** came from a real experience:
> *I recently discovered SIYAH on social media after hearing about their Shark Tank India deal and Himachal retail roots. However, when I tried visiting their official website that day, the website was down and not working. When this assessment was assigned, I immediately knew what I wanted to build: a high-performing, reliable, and beautiful landing page for SIYAH that does complete justice to their brand story.*

### Key Brand Context Reflected in the Code:
- 🏔️ **Grown in Himachal Pradesh**: Highlighting Pahadi weaving heritage and mountain roots.
- 🏬 **First 10 Physical Outlets**: Celebrating their initial 10 offline retail stores across Himachal before expanding online nationwide.
- 🦈 **Shark Tank India Deal**: Featuring their national television appearance and successful investment deal.
- 💡 **Core Value Proposition**: *"Ethnic wear, minus the boring price tag."*

---

## 2. Technical & Design Trade-Offs I Made

### A. Swaying SVG Ribbons over Heavy 3D Canvas
I wanted a background element that felt like a fluttering saree pallu. I considered using Three.js or WebGL, but loading 2MB+ of 3D JavaScript libraries didn't make sense for a landing page where load speed is critical. Instead, I built a dual-layer SVG ribbon background with CSS keyframe animation and zari dotted borders. It weighs less than 2KB, runs at 60 FPS, and respects `prefers-reduced-motion`.

### B. Interactive Touches for Immediate Engagement
To make the page feel alive within the first 3 seconds of visiting, I added four interactive details:
1. **Live Drape Shade Studio**: Color dots under the hero text that instantly morph the background SVG saree pallu colors in real-time.
2. **Honest Price Math Breakdown Modal**: A click-to-view modal breaking down exact fabric cost (`₹1,100`), master tailoring (`₹750`), shipping (`₹249`), vs traditional 4x retailer markups (`+ ₹4,500 ❌`).
3. **Gold Zari Sparkle Cursor Trail**: An HTML5 Canvas particle engine spawning subtle gold and rani pink zari sparkles as the user moves their mouse over the hero.
4. **Real-time Launch Countdown Ticker**: A top notification bar with a live ticking drop timer (`03d : 14h : 22m : 45s`).

---

## 3. What I Would Build With a Full Week

If I had a full week instead of a short deadline, here is what I would expand:

1. **Interactive 3D Saree Fabric Inspection**: Build a 3D canvas viewer allowing visitors to zoom in and drag to inspect fabric weave patterns up close.
2. **Mix-and-Match Outfit Builder**: A drag-and-drop tool for pairing kurtis with different dupattas and pants.
3. **Interactive Himachal Store Locator**: An interactive map showing all 10 physical retail outlets across Himachal Pradesh.
4. **Full Database Integration**: Connect the VIP account modal to a Supabase/Firebase backend with automated promo code delivery.

---

## 4. Honest Reflection on Using AI Tools

The assessment prompt highlights **Honesty** as a core evaluation criterion, so I want to be completely open about how I used AI tools while working on this project:

### How AI Helped Me:
- Drafting initial HTML layout tags and CSS variable setups.
- Writing math helper formulas for particle opacity fade in the canvas sparkle trail loop.

### What I Rejected & Built Myself:
- **Rejected Generic Templates**: AI initially suggested standard generic Tailwind themes and generic light cream palettes. I replaced them with a custom brand identity based on Siyah near-black (`#161213`), Rani Pink (`#B23A6B`), Marigold Gold (`#E8A33D`), and Fraunces serif display typography.
- **Removed Fake Social Proof**: AI template drafts included fake review quotes like *"Loved by 10,000+ happy women ⭐⭐⭐⭐⭐"*. I removed all fabricated metrics and replaced them with an **Honesty First Banner** (*"No fake testimonials or manufactured metrics — just real craft and transparent pricing"*).
- **Custom Brand Shapes**: I designed the price-tag shaped CTA buttons using CSS `clip-path` polygon clipping to physically reflect the brand pitch (*"minus the boring price tag"*).

---

## 5. Verification & Testing

- **Cross-Browser Verification**: Tested across Chrome, Edge, and Mobile Safari.
- **Mobile Responsiveness**: Checked fluid scaling from 390px mobile screens to 1440px+ desktop displays.
- **Header Offset Alignment**: Set `scroll-margin-top: 80px` on section headings so scrolling via navigation links lands neatly below the sticky header.
