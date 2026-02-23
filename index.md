---
layout: home
title: Sanicon Valley v.1
---

<style>
  @import url('https://fonts.googleapis.com');

  :root {
    --blue: #00f2ff;
    --green: #00ff88;
    --red: #ff3e3e;
    --dark: #020205;
  }

  body {
    background-color: var(--dark);
    color: #ffffff;
    font-family: 'Plus Jakarta Sans', sans-serif;
    margin: 0;
    overflow-x: hidden;
  }

  /* Progress HUD */
  #hud {
    position: fixed;
    top: 50%;
    right: 30px;
    transform: translateY(-50%);
    z-index: 100;
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .hud-dot {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: rgba(255,255,255,0.2);
    border: 2px solid transparent;
    transition: 0.4s;
  }
  .hud-dot.active { background: var(--blue); transform: scale(1.5); box-shadow: 0 0 15px var(--blue); }

  /* Background Gradient Engine */
  .bg-gradient {
    position: fixed;
    top: 0; left: 0; width: 100%; height: 100%;
    z-index: -1;
    opacity: 0.15;
    transition: 1.5s ease;
  }

  /* Typography Enhancements */
  h1, h2 { font-family: 'Orbitron', sans-serif; text-transform: uppercase; letter-spacing: 4px; }
  
  .hero-title {
    font-size: clamp(3rem, 12vw, 10rem);
    font-weight: 900;
    line-height: 0.8;
    background: linear-gradient(to bottom, #fff 30%, var(--blue));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 20px;
  }

  /* Animation Classes */
  .scroll-section {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 100px 10%;
    box-sizing: border-box;
    position: relative;
  }

  .glass-box {
    background: rgba(255, 255, 255, 0.03);
    backdrop-filter: blur(15px);
    border: 1px solid rgba(255, 255, 255, 0.1);
    padding: 60px;
    border-radius: 40px;
    max-width: 1000px;
    transform: translateY(100px) scale(0.9);
    opacity: 0;
    transition: all 1.2s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .glass-box.visible {
    transform: translateY(0) scale(1);
    opacity: 1;
  }

  .highlight-blue { color: var(--blue); text-shadow: 0 0 15px rgba(0, 242, 255, 0.4); font-weight: 800; }
  .highlight-green { color: var(--green); text-shadow: 0 0 15px rgba(0, 255, 136, 0.4); font-weight: 800; }
  .highlight-red { color: var(--red); text-shadow: 0 0 15px rgba(255, 62, 62, 0.4); font-weight: 800; }

  p { font-size: 1.25rem; line-height: 1.8; color: rgba(255,255,255,0.8); margin-bottom: 25px; text-align: justify; }

</style>

<!-- Background Layer -->
<div id="bg-dynamic" class="bg-gradient"></div>

<!-- Navigation HUD -->
<div id="hud">
  <div class="hud-dot active" data-section="0"></div>
  <div class="hud-dot" data-section="1"></div>
  <div class="hud-dot" data-section="2"></div>
  <div class="hud-dot" data-section="3"></div>
</div>

<!-- Hero Section -->
<section class="scroll-section">
  <div style="text-align: center;">
    <p style="text-transform: uppercase; letter-spacing: 12px; color: var(--blue);">Sector 01: The Launch</p>
    <h1 class="hero-title">SANICON<br>VALLEY</h1>
    <p style="font-size: 1.5rem; letter-spacing: 5px;">THE INTERPLANETARY FUTURE CITY</p>
  </div>
</section>

<!-- Section 1: The Vision -->
<section class="scroll-section" data-color="var(--blue)">
  <div class="glass-box">
    <h2 class="highlight-blue">A New San Jose</h2>
    <p>Welcome to <strong>Sanicon Valley</strong>, the definitive interplanetary city. Nestled within the footprint of San Jose, this metropolis exists as the most advanced urban center on Earth. Our city represents a radical fusion of high-technology, natural preservation, and a philosophy of total waste repurposing.</p>
    <p>Home to over <span class="highlight-blue">1,000,000 residents</span>, Sanicon Valley serves as a global hub for social and technological evolution. We solve the decades-old inefficiencies of San Jose by implementing a sophisticated <strong>farm-to-table</strong> logistics system and intelligent urban planning.</p>
  </div>
</section>

<!-- Section 2: Hydro & Agriculture -->
<section class="scroll-section" data-color="var(--green)">
  <div class="glass-box" style="border-left: 4px solid var(--green);">
    <h2 class="highlight-green">Hydraulic Sustainability</h2>
    <p>San Jose has long suffered from water shortages. Sanicon Valley eliminates this crisis. We utilize an <strong>integrated greywater system</strong>; every drop of water from showers and taps is filtered and redirected to nourish the city’s vegetation.</p>
    <p>Every residence features a <span class="highlight-green">Personal Vertical Farm</span>. Agriculture is no longer distant—it is in your backyard. Residents use a unified OS to deploy robotic harvesters. When a surplus occurs, the system triggers a community-wide notification, allowing those in need to claim fresh produce for free. This fosters the deep human connection San Jose has lacked for years.</p>
  </div>
</section>

<!-- Section 3: Zero Waste -->
<section class="scroll-section" data-color="var(--blue)">
  <div class="glass-box">
    <h2 class="highlight-blue">Atmospheric Engineering</h2>
    <p>We boast a <span class="highlight-blue">Zero Carbon Footprint</span>. By trapping CO2, we create dry ice, carbonated beverages, and oxygen for interplanetary life support. Our waste management is absolute: food waste becomes high-grade compost, cooking oils are refined into organic soaps, and non-compostables are converted into <strong>biogas</strong> for our light-vehicle fleet.</p>
    <p>Even orange peels are repurposed into organic pesticides, ensuring that "waste" is a concept left in the 20th century.</p>
  </div>
</section>

<!-- Section 4: Urban Logistics -->
<section class="scroll-section" data-color="var(--red)">
  <div class="glass-box" style="border-left: 4px solid var(--red);">
    <h2 class="highlight-red">Automated Society</h2>
    <p>By moving agriculture to backyards, we have deleted supermarkets. These vacated spaces are now lush parks and social squares. We have replaced the intrusive footprint of trains with automated buses and biogas cars. Because every manual task is <strong>fully automated</strong>, our citizens are free to pursue education, art, and community growth.</p>
    <p>To solve global plastic pollution, Sanicon Valley uses <span class="highlight-red">Plastic-Eating Bacteria</span>. All packaging is uniform; once discarded into specialized local bins, the bacteria decompose the polymers instantly. There are no landfills here.</p>
  </div>
</section>

<!-- Section 5: The Energy Core -->
<section class="scroll-section" data-color="var(--green)">
  <div class="glass-box">
    <h2 class="highlight-green">Interplanetary Energy</h2>
    <p>Our power grid is a symphony of sources: Solar roofs, hydroelectric waterways, and wind turbine corridors. However, our main engine is <strong>Nuclear Fusion</strong>. Two secure, high-capacity plants power the entire valley, providing the massive energy required to sustain our advanced AI infrastructure.</p>
  </div>
</section>

<!-- Section 6: Zoning & Infrastructure -->
<section class="scroll-section" data-color="var(--red)">
  <div class="glass-box" style="border-left: 4px solid var(--red);">
    <h2 class="highlight-red">The Final Blueprint</h2>
    <p>Residential life is optimized. Each home supports a robotic assistant that allows for <strong>simulated visitors</strong> and instant communication without the need for a handheld phone. Zoning is strict: new homes are limited to 3,000 sq ft to ensure maximum efficiency. Hospitals are massive, 10-floor hubs capable of treating thousands simultaneously, eliminating wait times entirely.</p>
    <p>Through these zoning laws, we have reclaimed the Earth. Space is allocated with precision: for schools, for parks, and for the energy plants that fuel the <strong>interplanetary future</strong>.</p>
  </div>
</section>

<script>
  // Intersection Observer for Animations
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
        
        // Update background color based on section
        const color = entry.target.parentElement.getAttribute('data-color');
        if (color) {
          document.getElementById('bg-dynamic').style.boxShadow = `inset 0 0 300px ${color}`;
          document.getElementById('bg-dynamic').style.background = color;
        }
      }
    });
  }, { threshold: 0.3 });

  document.querySelectorAll('.glass-box').forEach(box => observer.observe(box));

  // HUD Update on Scroll
  window.addEventListener('scroll', () => {
    const sections = document.querySelectorAll('.scroll-section');
    const dots = document.querySelectorAll('.hud-dot');
    
    sections.forEach((section, i) => {
      const rect = section.getBoundingClientRect();
      if (rect.top < window.innerHeight/2 && rect.bottom > window.innerHeight/2) {
        dots.forEach(d => d.classList.remove('active'));
        if(dots[i]) dots[i].classList.add('active');
      }
    });
  });
</script>
