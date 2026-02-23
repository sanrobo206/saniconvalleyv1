---
layout: home
title: Sanicon Valley — Technical Manifesto v.1
---

<style>
  @import url('https://fonts.googleapis.com');
  
  :root { --accent: #00d2ff; --bg: #ffffff; --text: #1a1a1a; --muted: #64748b; --paper: #f8fafc; }

  body { margin: 0; background: var(--bg); color: var(--text); font-family: 'Plus Jakarta Sans', sans-serif; line-height: 1.7; overflow-x: hidden; }

  /* Research HUD */
  #progress-bar { position: fixed; top: 0; left: 0; width: 0%; height: 5px; background: linear-gradient(90deg, #00d2ff, #00ff88); z-index: 10000; }
  #sync-status { position: fixed; top: 20px; right: 30px; font-family: 'Orbitron'; font-size: 0.7rem; color: var(--accent); z-index: 10001; letter-spacing: 2px; }

  /* Paper Layout */
  .paper-container { max-width: 900px; margin: 0 auto; padding: 100px 40px; perspective: 1200px; }
  header { text-align: center; border-bottom: 2px solid #000; padding-bottom: 40px; margin-bottom: 60px; }
  .journal-title { font-weight: 800; text-transform: uppercase; letter-spacing: 4px; font-size: 0.8rem; color: var(--muted); margin-bottom: 10px; }
  h1.main-title { font-size: 3.5rem; font-weight: 800; line-height: 1.1; margin: 0; letter-spacing: -2px; }
  
  /* Tilt Paragraphs - Subtle 3D Depth */
  .tilt-para { 
    margin-bottom: 50px; text-align: justify; color: #334155; 
    transition: transform 0.1s ease-out;
    transform-style: preserve-3d;
    will-change: transform;
    font-size: 1.1rem;
  }

  .abstract { font-family: 'Libre Baskerville', serif; font-size: 1.15rem; font-style: italic; background: var(--paper); padding: 40px; border-radius: 8px; margin-bottom: 60px; line-height: 1.8; border-left: 5px solid #000; }

  h2 { font-size: 1.8rem; font-weight: 800; border-bottom: 1px solid #eee; padding-bottom: 10px; margin-top: 100px; text-transform: uppercase; letter-spacing: 1px; color: #000; }

  /* ZOOM ENGINE SECTIONS (FOR DIAGRAMS) */
  .diagram-zoom-trigger { height: 200vh; position: relative; margin: 60px 0; }
  .diagram-viewport { position: sticky; top: 0; width: 100%; height: 100vh; display: flex; align-items: center; justify-content: center; overflow: hidden; }
  .diagram-content { 
    position: absolute; width: 85%; max-width: 900px; opacity: 0; 
    transform: scale(0.3); transition: opacity 0.2s;
    text-align: center;
  }
  .diagram-svg-wrap { 
    background: #ffffff; padding: 40px; border-radius: 20px; 
    border: 1px solid #e2e8f0; box-shadow: 0 30px 60px rgba(0,0,0,0.08);
  }
  .zoom-label { font-family: 'Orbitron'; font-size: 1.8rem; margin-top: 25px; color: #000; text-transform: uppercase; letter-spacing: 2px; }
  .zoom-desc { color: var(--muted); font-size: 1rem; margin-top: 5px; font-weight: 600; }

  footer { background: #000; color: #fff; padding: 100px 40px; text-align: center; font-family: 'Orbitron'; letter-spacing: 5px; font-size: 0.8rem; }
</style>

<div id="progress-bar"></div>
<div id="sync-status">LOAD_ENGINEERING_DATA: 0%</div>

<div class="paper-container">
  <header>
    <div class="journal-title">Proceedings of Interplanetary Urbanism • 2026</div>
    <h1 class="main-title">Sanicon Valley: A Blueprint for Interplanetary Urban Habitats</h1>
    <div style="margin-top:20px; font-weight:700;">By Sanatan Sinha</div>
  </header>

  <div class="abstract">
    <b>Abstract—</b> This paper presents the technical framework for Sanicon Valley, a city engineered to thrive in San Jose and future Martian environments. This document catalogs the robotic, hydraulic, and nuclear sub-systems required for 100% urban efficiency.
  </div>

  <h2>1.0 The Sanicon Overview</h2>
  <div class="tilt-para">Welcome to Sanicon Valley, the one and only interplanetary future city, that lies on the great city of San Jose, far more advanced than many other cities in the world. Our city blends advanced technology, with nature, and repurposing waste for the greater good. Sanicon Valley is home to more than 1,000,000 residents, as it is the hub of social, economic, and technological advancement, with the forward thinking system of urban planning, and repurposing waste.</div>

  <!-- DIAGRAM 1: URBAN HUB -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <circle cx="200" cy="100" r="70" stroke="#000" stroke-width="1" stroke-dasharray="4 4"/>
            <rect x="180" y="80" width="40" height="40" fill="#00d2ff" fill-opacity="0.2" stroke="#00d2ff"/>
            <path d="M100 100 L180 100 M220 100 L300 100 M200 30 L200 80 M200 120 L200 170" stroke="#000" stroke-width="1.5"/>
            <text x="200" y="105" text-anchor="middle" font-family="Orbitron" font-size="10" fill="#000">CITY_HUB</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 1.1: CENTRAL HUB CONNECTIVITY</div>
        <div class="zoom-desc">Network topology of 1M resident integration.</div>
      </div>
    </div>
  </section>

  <div class="tilt-para">Our city uses advanced technology to repurpose all kinds of waste to useful nutrients, energy, fuel, and more. We keep our city as simple as possible as we fix the major problem which has never been solved for decades in San Jose, which is to improve our farm to table system.</div>

  <!-- DIAGRAM 2: WASTE TO NUTRIENT -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <rect x="50" y="75" width="80" height="50" rx="4" stroke="#000" stroke-width="2"/>
            <path d="M130 100 H270" stroke="#00ff88" stroke-width="4" stroke-dasharray="10 5"/>
            <rect x="270" y="75" width="80" height="50" rx="4" stroke="#000" stroke-width="2" fill="#00ff88" fill-opacity="0.1"/>
            <text x="90" y="105" text-anchor="middle" font-size="10" fill="#000">WASTE</text>
            <text x="310" y="105" text-anchor="middle" font-size="10" fill="#000">FUEL</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 1.2: WASTE REPURPOSING FLOW</div>
        <div class="zoom-desc">Conversion of domestic refuse into organic nutrients.</div>
      </div>
    </div>
  </section>

  <h2>2.0 Hydraulic Survival</h2>
  <div class="tilt-para">There are many problems in San Jose. A major problem is the extreme water shortage in San Jose. Sanicon Valley not only fixes this problem, but also uses this problem to fix another major problem which is having enough water to keep the plants healthy. We will repurpose shower water which can be used to water the plants, so that the plants will be healthy with less water.</div>

  <!-- DIAGRAM 3: SHOWER TO PLANT -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <path d="M100 50 V150 Q100 170 150 170 H250 Q300 170 300 150 V50" stroke="#00d2ff" stroke-width="3"/>
            <path d="M150 100 L250 100" stroke="#00d2ff" stroke-width="1" stroke-dasharray="5 5"/>
            <text x="200" y="90" text-anchor="middle" font-size="10" fill="#00d2ff">GRAYWATER RECOVERY</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 2.1: HYDRAULIC RECIRCULATION</div>
        <div class="zoom-desc">Closed-loop shower-to-hydroponic pipeline.</div>
      </div>
    </div>
  </section>

  <h2>3.0 Vertical Agriculture</h2>
  <div class="tilt-para">Also, every house has a vertical farm in their backyard. This makes sure that everyone has a farm and a grocery store for agriculture in their own backyard. Everyone will have an app in which they can order a robot which will give the amount and kind of fruit or vegetable upon order.</div>

  <!-- DIAGRAM 4: BOT INTERFACE -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <rect x="150" y="50" width="100" height="100" stroke="#000" stroke-width="2"/>
            <circle cx="200" cy="80" r="15" stroke="#00ff88" stroke-width="2"/>
            <path d="M180 120 H220" stroke="#000" stroke-width="2"/>
            <text x="200" y="170" text-anchor="middle" font-family="Orbitron" font-size="12">APP_CONTROL</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 3.1: ROBOTIC HARVEST INTERFACE</div>
        <div class="zoom-desc">Mobile application link to autonomous backyard bots.</div>
      </div>
    </div>
  </section>

  <div class="tilt-para">Whenever there is a surplus of fruits or vegetables in a house, then the app will send a notification that there is a surplus and then if the person accepts that they do not want it, then it will notify the entire community that anyone who wants can take it. This ensures that no food is wasted and even the poor can get fruits and vegetables.</div>

  <!-- DIAGRAM 5: SURPLUS SHARING -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <circle cx="100" cy="100" r="20" stroke="#000"/>
            <circle cx="300" cy="100" r="20" stroke="#000"/>
            <path d="M120 100 H280" stroke="#00d2ff" stroke-width="2" marker-end="url(#arrow)"/>
            <text x="200" y="90" text-anchor="middle" font-size="10" fill="#00d2ff">SURPLUS_TRANSFER</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 3.2: COMMUNITY MESH NETWORK</div>
        <div class="zoom-desc">Logistics of localized food redistribution.</div>
      </div>
    </div>
  </section>

  <h2>4.0 Interplanetary Energy</h2>
  <div class="tilt-para">Our way of generating energy is one of the best ways. We do not just use one method, we use every single possible method. We use solar energy which is mainly for houses, and electric vehicle charging stations. One energy solution which makes this city interplanetary is nuclear energy.</div>

  <!-- DIAGRAM 6: NUCLEAR DENSITY -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <path d="M200 50 L250 150 L150 150 Z" stroke="#ff3e3e" stroke-width="2" fill="#ff3e3e" fill-opacity="0.1"/>
            <circle cx="200" cy="110" r="10" fill="#ff3e3e"/>
            <text x="200" y="180" text-anchor="middle" font-family="Orbitron" font-size="12">NUCLEAR_CORE</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 4.1: ENERGY DENSITY MATRIX</div>
        <div class="zoom-desc">Nuclear core placement for high-demand AI logic.</div>
      </div>
    </div>
  </section>

  <h2>5.0 Zoning & Infrastructure</h2>
  <div class="tilt-para">All of the existing houses can stay as it is, but every new house can have a maximum area of 3,000 square feet excluding the backyard, and the backyard will have a maximum area of 1,000 square feet. This is because our city is trying to make every house just the minimum size needed.</div>

  <!-- DIAGRAM 7: ZONING MAP -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <rect x="50" y="50" width="300" height="100" stroke="#000" stroke-width="1"/>
            <rect x="60" y="60" width="100" height="80" fill="#eee" stroke="#000"/>
            <text x="110" y="105" text-anchor="middle" font-size="8">RESIDENTIAL</text>
            <rect x="240" y="60" width="100" height="80" fill="#ffcc00" fill-opacity="0.2" stroke="#ffcc00"/>
            <text x="290" y="105" text-anchor="middle" font-size="8">INDUSTRIAL</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 5.1: ZONING PROTOCOL</div>
        <div class="zoom-desc">Spatial distribution of 3000 sq ft residential plots.</div>
      </div>
    </div>
  </section>

  <div class="tilt-para">With all of these innovations, Sanicon Valley is truly the city of the future. The offices will be close by and it will be so that people can roam through different offices, and can see what is going on in the area. This makes everything more engaging and enables people to communicate.</div>

  <!-- DIAGRAM 8: SOCIAL SQUARE -->
  <section class="diagram-zoom-trigger">
    <div class="diagram-viewport">
      <div class="diagram-content">
        <div class="diagram-svg-wrap">
          <svg viewBox="0 0 400 200" fill="none" xmlns="http://www.w3.org">
            <rect x="150" y="50" width="100" height="100" stroke="#000" stroke-dasharray="5 5"/>
            <circle cx="170" cy="70" r="5" fill="#00d2ff"/>
            <circle cx="230" cy="130" r="5" fill="#00d2ff"/>
            <circle cx="200" cy="100" r="20" stroke="#00d2ff" stroke-width="1"/>
            <text x="200" y="170" text-anchor="middle" font-size="10">ENGAGEMENT SQUARE</text>
          </svg>
        </div>
        <div class="zoom-label">FIG 5.2: SOCIALIZATION HUB</div>
        <div class="zoom-desc">Architectural center-point for cross-industry communication.</div>
      </div>
    </div>
  </section>
</div>

<footer>
  <p>© COPYRIGHT SANATAN SINHA — ALL RIGHTS RESERVED</p>
  <p style="font-size: 0.6rem; opacity: 0.5; margin-top: 20px;">ENGINEERED IN SAN JOSE • 2026</p>
</footer>

<script>
  window.addEventListener('scroll', () => {
    const scrollPos = window.scrollY;
    const maxScroll = document.documentElement.scrollHeight - window.innerHeight;
    const percent = (scrollPos / maxScroll) * 100;
    
    // HUD
    document.getElementById('progress-bar').style.width = percent + '%';
    document.getElementById('sync-status').innerText = `ANALYZING_DATA: ${Math.floor(percent)}%`;

    // 1. TILT ANIMATION for Paragraphs
    const paras = document.querySelectorAll('.tilt-para');
    paras.forEach(p => {
      const rect = p.getBoundingClientRect();
      if(rect.top < window.innerHeight && rect.bottom > 0) {
        const center = window.innerHeight / 2;
        const distFromCenter = rect.top + rect.height/2 - center;
        // 2-degree tilt based on scroll position
        const tilt = (distFromCenter / window.innerHeight) * 5;
        p.style.transform = `rotateX(${tilt}deg) translateZ(0)`;
      }
    });

    // 2. KINETIC ZOOM for Diagrams
    const triggers = document.querySelectorAll('.diagram-zoom-trigger');
    triggers.forEach(trigger => {
      const rect = trigger.getBoundingClientRect();
      const content = trigger.querySelector('.diagram-content');
      
      if (rect.top <= 0 && rect.bottom >= 0) {
        const progress = Math.abs(rect.top) / (rect.height - window.innerHeight);
        
        let opacity = 1;
        if (progress < 0.1) opacity = progress * 10;
        if (progress > 0.9) opacity = (1 - progress) * 10;
        
        const scale = 0.1 + (progress * 3.5);
        content.style.opacity = Math.min(opacity, 1);
        content.style.transform = `scale(${scale})`;
      } else {
        content.style.opacity = 0;
      }
    });
  });
</script>
