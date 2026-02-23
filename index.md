---
layout: home
title: Sanicon Valley v.1 - Interplanetary Core
---

<style>
  @import url('https://fonts.googleapis.com');

  :root {
    --blue: #00d2ff;
    --green: #00ff88;
    --red: #ff3e3e;
    --space-black: #02040a;
  }

  body {
    background-color: var(--space-black);
    color: #ffffff;
    font-family: 'Space Grotesk', sans-serif;
    margin: 0;
    overflow-x: hidden;
    scroll-behavior: smooth;
  }

  /* Fixed Background Starfield & Nebulas */
  .stars-container {
    position: fixed;
    top: 0; left: 0; width: 100%; height: 100%;
    z-index: -2;
    background: radial-gradient(circle at center, #0a0a1a 0%, #02040a 100%);
  }

  .nebula {
    position: fixed;
    width: 80vw; height: 80vh;
    border-radius: 50%;
    filter: blur(150px);
    z-index: -1;
    opacity: 0.15;
    transition: all 1.5s cubic-bezier(0.4, 0, 0.2, 1);
  }

  /* Parallax Scrolling Engine */
  .scroll-wrapper {
    perspective: 1500px;
    height: 100vh;
    overflow-y: auto;
    overflow-x: hidden;
    scroll-snap-type: y mandatory;
  }

  .section-container {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    scroll-snap-align: start;
    perspective: 1000px;
  }

  /* Expanding Interplanetary Cards */
  .sector-card {
    width: 85%;
    max-width: 1200px;
    padding: 100px 80px;
    background: rgba(255, 255, 255, 0.02);
    backdrop-filter: blur(30px);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 60px;
    transform: rotateX(25deg) translateY(150px) scale(0.7);
    opacity: 0;
    transition: all 1.2s cubic-bezier(0.16, 1, 0.3, 1);
    box-shadow: 0 50px 100px rgba(0,0,0,0.9);
    position: relative;
    overflow: hidden;
  }

  /* Active State (Triggered by Scroll) */
  .section-container.active .sector-card {
    transform: rotateX(0deg) translateY(0) scale(1.05);
    opacity: 1;
    border-color: var(--accent);
    box-shadow: 0 0 80px rgba(var(--accent-rgb), 0.15);
  }

  /* Text Styling */
  .sector-card h2 {
    font-family: 'Orbitron', sans-serif;
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    margin-bottom: 40px;
    text-transform: uppercase;
    letter-spacing: 6px;
    color: var(--accent);
    text-shadow: 0 0 20px rgba(var(--accent-rgb), 0.5);
  }

  .sector-card p {
    font-size: 1.45rem;
    line-height: 1.8;
    color: rgba(255, 255, 255, 0.85);
    font-weight: 300;
    margin-bottom: 30px;
    text-align: justify;
  }

  /* Color Schemes */
  .blue-sector { --accent: var(--blue); --accent-rgb: 0, 210, 255; }
  .green-sector { --accent: var(--green); --accent-rgb: 0, 255, 136; }
  .red-sector { --accent: var(--red); --accent-rgb: 255, 62, 62; }

  /* Hero HUD */
  .hero-text {
    text-align: center;
    transform: translateZ(100px);
  }

  .hero-title {
    font-family: 'Orbitron', sans-serif;
    font-size: clamp(4rem, 15vw, 11rem);
    font-weight: 900;
    background: linear-gradient(to bottom, #fff 40%, var(--blue));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin: 0;
  }

  #progress-bar {
    position: fixed;
    top: 0; left: 0; height: 4px;
    background: linear-gradient(90deg, var(--blue), var(--green), var(--red));
    z-index: 1000;
    transition: width 0.2s ease;
  }
</style>

<div id="progress-bar"></div>
<div class="stars-container"></div>
<div id="nebula-bg" class="nebula" style="top: 10%; right: 10%; background: var(--blue);"></div>

<div class="scroll-wrapper" id="main-scroll">

  <!-- HERO SECTION -->
  <section class="section-container active">
    <div class="hero-text">
      <div style="border: 1px solid var(--blue); display: inline-block; padding: 10px 30px; border-radius: 50px; margin-bottom: 30px; color: var(--blue); letter-spacing: 5px; font-size: 0.8rem;">SANICON PROTOCOL V.1</div>
      <h1 class="hero-title">SANICON</h1>
      <h1 class="hero-title" style="font-size: 0.5em; -webkit-text-fill-color: white; margin-top: -20px;">VALLEY</h1>
      <p style="margin-top: 40px; opacity: 0.5; letter-spacing: 10px; font-family: 'Orbitron';">INITIATING NAV-SYNC</p>
    </div>
  </section>

  <!-- SECTION 1: VISION -->
  <section class="section-container blue-sector" data-color="var(--blue)">
    <div class="sector-card">
      <h2>Sanicon Valley</h2>
      <p>Welcome to <b>Sanicon Valley</b>, the one and only interplanetary future city, that lies on the great city of San Jose, far more advanced than many other cities in the world. Our city blends advanced technology, with nature, and repurposing waste for the greater good.</p>
      <p>Sanicon Valley is home to more than 1,000,000 residents, as it is the hub of social, economic, and technological advancement, with the forward thinking system of urban planning, and repurposing waste. We keep our city as simple as possible as we fix the major problem which has never been solved for decades in San Jose, which is to improve our farm to table system.</p>
    </div>
  </section>

  <!-- SECTION 2: WATER -->
  <section class="section-container green-sector" data-color="var(--green)">
    <div class="sector-card">
      <h2>Hydraulic Core</h2>
      <p>There are many problems in San Jose. A major problem is the extreme water shortage. Sanicon Valley not only fixes this problem, but also uses this problem to fix another major problem which is having enough water to keep the plants healthy. We will repurpose shower water which can be used to water the plants, so that the plants will be healthy with less water.</p>
      <p>Also, every house has a <b>vertical farm</b> in their backyard. This makes sure that everyone has a farm and a grocery store for agriculture in their own backyard. Everyone will have an app in which they can order a robot which will give the amount and kind of fruit or vegetable upon order.</p>
    </div>
  </section>

  <!-- SECTION 3: SOCIAL AGRI -->
  <section class="section-container blue-sector" data-color="var(--blue)">
    <div class="sector-card">
      <h2>Community OS</h2>
      <p>Whenever there is a surplus of fruits or vegetables in a house, then the app will send a notification that there is a surplus and then if the person accepts that they do not want it, then it will notify the entire community that anyone who wants can take it. This ensures that no food is wasted and even the poor can get fruits and vegetables.</p>
      <p>Also, this enables people to go to each other’s house, communicate, which builds a strong community, which San Jose currently lacks. Our city has little to no carbon footprint.</p>
    </div>
  </section>

  <!-- SECTION 4: NET ZERO -->
  <section class="section-container red-sector" data-color="var(--red)">
    <div class="sector-card">
      <h2>Zero-Waste Logic</h2>
      <p>We trap carbon dioxide and use it for various different purposes, from fizz drinks, dry ice, to plants using it. The reason that this is an interplanetary solution is because the carbon dioxide can be used for purposes like using plants to convert it to oxygen, for air in which you can breathe, and for other uses.</p>
      <p>We use various different kinds of waste for various different purposes, leaving almost zero net waste. Fruit peels, especially oranges, can be used as an <b>organic pesticide</b>. Also other waste that cannot be used as compost will be used as biogas for the little gas powered cars.</p>
    </div>
  </section>

  <!-- SECTION 5: ENERGY -->
  <section class="section-container green-sector" data-color="var(--green)">
    <div class="sector-card">
      <h2>Nuclear Grid</h2>
      <p>Our way of generating energy is one of the best ways. We use every single possible method: solar energy, hydroelectric power from every water body, and wind turbines installed in extremely windy areas. But the anchor of this city is <b>nuclear energy</b>.</p>
      <p>The nuclear energy plants will be located in areas which have extremely less population. Just two plants are enough to power the entire Sanicon Valley. This will be the main source of energy, as AI will be heavily used and it needs a lot of energy.</p>
    </div>
  </section>

  <!-- SECTION 6: ZONING -->
  <section class="section-container red-sector" data-color="var(--red)">
    <div class="sector-card">
      <h2>Urban Zoning</h2>
      <p>Hospitals will be really big so that more people can be treated at once reducing the wait time. The maximum area is 100,000 square feet, along with the maximum floors being 10 floors. Just 5 of these hospitals is enough to handle the whole Sanicon Valley at once.</p>
      <p>The benefits of these zoning laws is that there is a lot of space for schools which is enough to have almost every single kid having access to education. Some space will be left for parks. Now the remaining space will be used for energy generation.</p>
    </div>
  </section>

  <footer style="height: 50vh; display: flex; align-items: center; justify-content: center; opacity: 0.2; letter-spacing: 10px; font-family: 'Orbitron'; font-size: 0.8rem;">
    END OF TRANSMISSION // 2026
  </footer>

</div>

<script>
  const scrollWrapper = document.getElementById('main-scroll');
  const progressBar = document.getElementById('progress-bar');
  const sections = document.querySelectorAll('.section-container');
  const nebula = document.getElementById('nebula-bg');

  scrollWrapper.addEventListener('scroll', () => {
    // Update Progress Bar
    const totalHeight = scrollWrapper.scrollHeight - scrollWrapper.clientHeight;
    const progress = (scrollWrapper.scrollTop / totalHeight) * 100;
    progressBar.style.width = progress + '%';

    // Intersection Logic for Parallax Cards
    sections.forEach(section => {
      const rect = section.getBoundingClientRect();
      if (rect.top < window.innerHeight / 2 && rect.bottom > window.innerHeight / 2) {
        section.classList.add('active');
        
        // Update Nebula Background Color
        const color = section.getAttribute('data-color');
        if (color) {
          nebula.style.background = color;
          nebula.style.transform = `translate(${rect.top / 10}px, ${rect.top / 10}px)`;
        }
      } else {
        section.classList.remove('active');
      }
    });
  });
</script>
