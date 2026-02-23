---
layout: home
title: Sanicon Valley v.1 - The Interplanetary Journey
---

<style>
  @import url('https://fonts.googleapis.com');

  :root {
    --blue: #00d2ff;
    --green: #00ff88;
    --red: #ff3e3e;
    --gold: #ffcc00;
    --space: #02040a;
  }

  * { box-sizing: border-box; }

  body {
    background-color: var(--space);
    color: #ffffff;
    font-family: 'Inter', sans-serif;
    margin: 0;
    padding: 0;
    overflow-x: hidden;
  }

  /* Progress Bar Top */
  #progress-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 6px;
    background: rgba(255,255,255,0.1);
    z-index: 9999;
  }
  #progress-bar {
    height: 100%;
    width: 0%;
    background: linear-gradient(90deg, var(--blue), var(--green), var(--red), var(--gold));
    box-shadow: 0 0 20px var(--blue);
    transition: width 0.1s ease-out;
  }
  #percentage-text {
    position: fixed;
    top: 15px;
    right: 20px;
    font-family: 'Orbitron';
    font-size: 0.8rem;
    color: var(--blue);
    z-index: 10000;
  }

  /* Background Space Engine */
  #universe {
    position: fixed;
    width: 100vw;
    height: 100vh;
    z-index: -1;
    background: radial-gradient(circle at center, #0a1128 0%, #02040a 100%);
  }

  .star {
    position: absolute;
    background: white;
    border-radius: 50%;
    opacity: 0.5;
    animation: twinkle var(--duration) infinite;
  }

  @keyframes twinkle {
    0%, 100% { opacity: 0.3; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.2); }
  }

  /* Epic Typography Sections */
  .v-section {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 10vh 10vw;
    position: relative;
    opacity: 0;
    transform: translateY(100px) scale(0.9);
    transition: all 1.5s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .v-section.active {
    opacity: 1;
    transform: translateY(0) scale(1);
  }

  .huge-text {
    font-family: 'Orbitron', sans-serif;
    font-size: clamp(3rem, 8vw, 12rem);
    line-height: 0.8;
    text-align: center;
    text-transform: uppercase;
    margin-bottom: 50px;
  }

  .fact-paragraph {
    font-size: clamp(1.2rem, 2.5vw, 2.2rem);
    line-height: 1.6;
    max-width: 1200px;
    text-align: center;
    font-weight: 200;
    color: rgba(255,255,255,0.8);
    margin-bottom: 5vh;
  }

  /* Section Colors */
  .blue-zone { --accent: var(--blue); }
  .green-zone { --accent: var(--green); }
  .red-zone { --accent: var(--red); }
  .gold-zone { --accent: var(--gold); }

  .accent-text {
    color: var(--accent);
    text-shadow: 0 0 30px var(--accent);
    font-weight: 700;
  }

  .divider {
    width: 200px;
    height: 2px;
    background: var(--accent);
    margin: 40px 0;
    box-shadow: 0 0 15px var(--accent);
  }

</style>

<div id="progress-container"><div id="progress-bar"></div></div>
<div id="percentage-text">0% COMPLETE</div>
<div id="universe"></div>

<div id="content-scroller">

  <!-- THE INTRO -->
  <section class="v-section blue-zone active">
    <div style="font-family: 'Orbitron'; letter-spacing: 10px; margin-bottom: 20px; opacity: 0.5;">INITIATING SEQUENCE</div>
    <h1 class="huge-text">SANICON<br><span class="accent-text">VALLEY</span></h1>
    <p class="fact-paragraph">
      Welcome to Sanicon Valley, the one and only <span class="accent-text">interplanetary future city</span>. 
      Lying on the foundations of San Jose, this metropolis is engineered to be more advanced than any urban center in history.
    </p>
    <div class="divider"></div>
  </section>

  <!-- SECTOR 1: THE FOUNDATION -->
  <section class="v-section blue-zone">
    <h2 class="huge-text" style="font-size: 5rem;">THE<br>VISION</h2>
    <p class="fact-paragraph">
      Our city blends <span class="accent-text">Advanced Technology with nature</span>, repurposing the remnants of the old world for the greater good. 
      Sanicon Valley is home to more than <span class="accent-text">1,000,000 residents</span>. 
    </p>
    <p class="fact-paragraph">
      It is the ultimate hub of social, economic, and technological advancement, utilizing a forward-thinking system of urban planning that prioritizes human life and efficiency over bureaucracy.
    </p>
  </section>

  <!-- SECTOR 2: WATER RECLAMATION -->
  <section class="v-section green-zone">
    <h2 class="huge-text" style="font-size: 5rem;">HYDRO<br>LOGIC</h2>
    <p class="fact-paragraph">
      San Jose has faced extreme water shortages for decades. <span class="accent-text">Sanicon Valley solves this.</span> 
      We turn a crisis into a solution by repurposing every drop of shower water.
    </p>
    <p class="fact-paragraph">
      This greywater is filtered and redirected to keep the city's vegetation and vertical farms vibrant and healthy, ensuring that no plant suffers while using less freshwater than ever before.
    </p>
  </section>

  <!-- SECTOR 3: PERSONAL AGRICULTURE -->
  <section class="v-section green-zone">
    <h2 class="huge-text" style="font-size: 5rem;">BACKYARD<br>FARMS</h2>
    <p class="fact-paragraph">
      Every single house is equipped with a <span class="accent-text">Vertical Farm</span>. 
      This ensures that every resident owns their own grocery store. 
    </p>
    <p class="fact-paragraph">
      Through a dedicated app, you order your personal robot to harvest specific fruits and vegetables. When a surplus occurs, the system notifies the entire community, allowing anyone in need to take it for free. No food is wasted.
    </p>
  </section>

  <!-- SECTOR 4: ATMOSPHERICS -->
  <section class="v-section blue-zone">
    <h2 class="huge-text" style="font-size: 5rem;">ZERO<br>CARBON</h2>
    <p class="fact-paragraph">
      We maintain <span class="accent-text">Zero Net Waste</span>. Carbon dioxide is trapped and converted for use in fizz drinks, dry ice, and oxygen conversion for interplanetary life support.
    </p>
    <p class="fact-paragraph">
      Leftover food becomes compost. Cooking oil is cleaned into soaps. Non-compostable waste is converted into <span class="accent-text">Biogas</span> to power the city's fleet of light vehicles. Even orange peels are distilled into organic pesticides.
    </p>
  </section>

  <!-- SECTOR 5: TRANSPORT -->
  <section class="v-section red-zone">
    <h2 class="huge-text" style="font-size: 5rem;">LOGISTIC<br>SHIFT</h2>
    <p class="fact-paragraph">
      Supermarkets are obsolete because every backyard is a farm. This reclaims massive amounts of land for <span class="accent-text">recreational areas</span> and public squares where people meet.
    </p>
    <p class="fact-paragraph">
      We utilize automated buses and cars. Trains have been removed because they consume too much space and limit mobility. Every manual labor industry is <span class="accent-text">100% Automated</span>, freeing humans from repetitive toil.
    </p>
  </section>

  <!-- SECTOR 6: PLASTIC DECOMP -->
  <section class="v-section red-zone">
    <h2 class="huge-text" style="font-size: 5rem;">BACTERIAL<br>CLEANSE</h2>
    <p class="fact-paragraph">
      Sanicon Valley still uses plastic, but we have solved pollution. A strict law mandates disposal into specialized zones where <span class="accent-text">Plastic-Eating Bacteria</span> decompose waste immediately.
    </p>
    <p class="fact-paragraph">
      There are no landfills. There is no transportation of trash. The cycle of plastic ends exactly where it is discarded.
    </p>
  </section>

  <!-- SECTOR 7: ENERGY CORE -->
  <section class="v-section gold-zone">
    <h2 class="huge-text" style="font-size: 5rem;">THE ENERGY<br>TRIAD</h2>
    <p class="fact-paragraph">
      We use Solar for housing and EV charging. We use every water body for Hydroelectric power. We use Wind Turbines in designated high-wind corridors. 
    </p>
    <p class="fact-paragraph">
      But the main source is <span class="accent-text">Nuclear Fusion</span>. Two secure plants power the entire valley, providing the massive energy required for the AI that manages our interplanetary systems.
    </p>
  </section>

  <!-- SECTOR 8: DOMESTIC ROBOTICS -->
  <section class="v-section blue-zone">
    <h2 class="huge-text" style="font-size: 5rem;">SMART<br>LIVING</h2>
    <p class="fact-paragraph">
      Every home features a backyard robot and an optional household task bot. You can communicate with anyone instantly—it is like having a <span class="accent-text">Simulated Visitor</span> in your living room.
    </p>
    <p class="fact-paragraph">
      Your bot can even gift fruits from your vertical farm to the person you are talking to virtually. Sewage is non-existent; toilets and drains feed individual plants via a closed-loop pipe network.
    </p>
  </section>

  <!-- SECTOR 9: ZONING & INFRASTRUCTURE -->
  <section class="v-section red-zone">
    <h2 class="huge-text" style="font-size: 5rem;">STRICT<br>ZONING</h2>
    <p class="fact-paragraph">
      New houses are limited to 3,000 square feet with 1,000 square feet backyards. Ceilings are capped at 8 feet. We minimize personal space to maximize <span class="accent-text">Infrastructure Space</span>.
    </p>
    <p class="fact-paragraph">
      Hospitals are massive: <span class="accent-text">100,000 square feet</span> and 10 floors high. Just five of these facilities handle the entire population of Sanicon Valley with zero wait times.
    </p>
  </section>

  <!-- FINAL SECTION -->
  <section class="v-section gold-zone">
    <h2 class="huge-text" style="font-size: 3rem;">COORDINATES SET</h2>
    <p class="fact-paragraph">
      By optimizing space, we provide education for every child and lush parks for every adult. 
      Sanicon Valley is not just a city; it is the blueprint for the <span class="accent-text">Interplanetary Future</span>.
    </p>
    <div style="font-family: 'Orbitron'; margin-top: 50px; opacity: 0.3;">END OF TRANSMISSION // 2026</div>
  </section>

</div>

<script>
  // 1. Progress Bar Logic
  window.addEventListener('scroll', () => {
    const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
    const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
    const scrolled = (winScroll / height) * 100;
    document.getElementById("progress-bar").style.width = scrolled + "%";
    document.getElementById("percentage-text").innerText = Math.round(scrolled) + "% COMPLETE";

    // 2. Intersection Observer for Animations
    const sections = document.querySelectorAll('.v-section');
    sections.forEach(sec => {
      const top = sec.getBoundingClientRect().top;
      if (top < window.innerHeight * 0.75) {
        sec.classList.add('active');
      }
    });
  });

  // 3. Create Stars
  const universe = document.getElementById('universe');
  for (let i = 0; i < 200; i++) {
    const star = document.createElement('div');
    star.className = 'star';
    star.style.width = Math.random() * 3 + 'px';
    star.style.height = star.style.width;
    star.style.top = Math.random() * 100 + 'vh';
    star.style.left = Math.random() * 100 + 'vw';
    star.style.setProperty('--duration', (Math.random() * 3 + 2) + 's');
    universe.appendChild(star);
  }
</script>
