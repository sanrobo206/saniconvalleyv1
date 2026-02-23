---
layout: home
title: Sanicon Valley - Interplanetary Future City
---

<style>
  @import url('https://fonts.googleapis.com');
  
  :root { --b: #00d2ff; --g: #00ff88; --s: #000000; }

  body, html { 
    margin: 0; padding: 0; background: var(--s); color: #fff; 
    font-family: 'Plus Jakarta Sans', sans-serif; 
    overflow-x: hidden; height: 12000vh; /* Controlled height for fast scroll completion */
    scroll-behavior: auto; 
  }

  /* Professional HUD */
  #h { position: fixed; top: 0; left: 0; width: 100%; height: 5px; background: rgba(255,255,255,0.05); z-index: 10000; }
  #p { height: 100%; width: 0%; background: linear-gradient(90deg, var(--b), var(--g)); box-shadow: 0 0 15px var(--b); }
  #u { position: fixed; top: 30px; right: 40px; font-family: 'Orbitron'; font-size: 0.9rem; color: var(--b); z-index: 10001; letter-spacing: 3px; }

  /* Kinetic Zoom Stage */
  .v { position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; display: flex; justify-content: center; align-items: center; perspective: 1000px; pointer-events: none; }
  
  .z { 
    position: absolute; width: 85%; max-width: 1200px; text-align: center; 
    opacity: 0; transform: scale(0.01); will-change: transform, opacity; 
    padding: 60px; border-radius: 40px; background: rgba(255,255,255,0.02); 
    backdrop-filter: blur(20px); border: 1px solid rgba(255,255,255,0.1);
  }

  .big { font-family: 'Orbitron', sans-serif; font-size: clamp(2rem, 5vw, 6rem); line-height: 1; text-transform: uppercase; margin-bottom: 30px; font-weight: 900; letter-spacing: -2px; }
  .para { font-size: clamp(1.1rem, 1.8vw, 2.2rem); line-height: 1.6; font-weight: 300; color: rgba(255,255,255,0.9); text-align: justify; text-justify: inter-word; }
  
  .ab { color: var(--b); text-shadow: 0 0 30px var(--b); }
  .ag { color: var(--g); text-shadow: 0 0 30px var(--g); }

  canvas#stars { position: fixed; inset: 0; z-index: -1; }
  footer { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); font-family: 'Orbitron'; font-size: 0.7rem; letter-spacing: 5px; opacity: 0.5; z-index: 10002; color: #fff; }
</style>

<div id="h"><div id="p"></div></div>
<div id="u">DATA STREAM: 0%</div>
<canvas id="stars"></canvas>
<footer>COPYRIGHT SANATAN SINHA</footer>

<div class="v">
  <!-- Paragraph 1 -->
  <div class="z" data-s="0" data-e="9">
    <h1 class="big ab">Sanicon Valley</h1>
    <p class="para">The interplanetary Future City. Welcome to Sanicon Valley, the one and only interplanetary future city, that lies on the great city of San Jose, far more advanced than many other cities in the world. Our city blends advanced technology, with nature, and repurposing waste for the greater good. Sanicon Valley is home to more than 1,000,000 residents, as it is the hub of social, economic, and technological advancement, with the forward thinking system of urban planning, and repurposing waste. Our city uses advanced technology to repurpose all kinds of waste to useful nutrients, energy, fuel, and more. We keep our city as simple as possible as we fix the major problem which has never been solved for decades in San Jose, which is to improve our farm to table system.</p>
  </div>

  <!-- Paragraph 2 -->
  <div class="z" data-s="10" data-e="19">
    <h1 class="big ag">Resource Recovery</h1>
    <p class="para">There are many problems in San Jose. A major problem is the extreme water shortage in San Jose. Sanicon Valley not only fixes this problem, but also uses this problem to fix another major problem which is having enough water to keep the plants healthy. We will repurpose shower water which can be used to water the plants, so that the plants will be healthy with less water. Also, every house has a vertical farm in their backyard. This makes sure that everyone has a farm and a grocery store for agriculture in their own backyard. Everyone will have an app in which they can order a robot which will give the amount and kind of fruit or vegetable upon order. Whenever there is a surplus of fruits or vegetables in a house, then the app will send a notification that there is a surplus and then if the person accepts that they do not want it, then it will notify the entire community that anyone who wants can take it. This ensures that no food is wasted and even the poor can get fruits and vegetables. Also, this enables people to go to each other’s house, communicate, which builds a strong community, which San Jose currently lacks.</p>
  </div>

  <!-- Paragraph 3 -->
  <div class="z" data-s="20" data-e="29">
    <h1 class="big ab">Zero Net Waste</h1>
    <p class="para">Our city has little to no carbon footprint. This is because we trap carbon dioxide and use it for various different purposes, from fizz drinks, dry ice, to plants using it. The reason that this is an interplanetary solution is because the carbon dioxide can be used for various purposes like using plants to convert it to oxygen, for air in which you can breathe, and for other uses. We use various different kinds of waste for various different purposes, leaving almost zero net waste. For example we will use remaining food waste as compost, and remove some food remains from cooking oil which will be compost, while the remaining oil will be cleaned and used for soaps. Also other waste that cannot be used as compost, and has little to no nutrition will be used as biogas which will be used for the little gas powered cars. Fruit peels, especially oranges can be used as an organic pesticide.</p>
  </div>

  <!-- Paragraph 4 -->
  <div class="z" data-s="30" data-e="39">
    <h1 class="big ag">Urban Planning</h1>
    <p class="para">In our city, there will be no supermarkets/grocery stores for fruits and vegetables, as every backyard is a farm. The only food items that will be sold will be meat, snacks, and drinks. This means that there is more space for recreational areas, and squares where people can meet together. This brings a stronger sense of community. Also, there will be zero farms, because every backyard is a farm. This makes more space for other important areas like, industrial areas, schools, and parks. For transportation the car and the bus are used. The train is not used because it takes too much space and it is limited to only a few areas. Every industry that involves manual labor will be automated, meaning that no one has to do that kind of work.</p>
  </div>

  <!-- Paragraph 5 -->
  <div class="z" data-s="40" data-e="49">
    <h1 class="big ab">Decomposition Tech</h1>
    <p class="para">Another problem which is worldwide is the effects of the traditional packaging methods. Now, Sanicon Valley still uses plastic as the packaging method, but there is a new innovation that solves pollution. There will be a law in which everyone has to throw away the plastic waste in a certain area and if they do not follow it, they will be heavily fined. This area is special, because it does not go to landfills, or even gets transported. In that bin, there will be plastic eating bacteria, which will almost immediately decompose the plastic allowing there to be practically no plastic waste. Every single package will be made out of plastic.</p>
  </div>

  <!-- Paragraph 6 -->
  <div class="z" data-s="50" data-e="59">
    <h1 class="big ag">Energy Matrix</h1>
    <p class="para">Our way of generating energy is one of the best ways. We do not just use one method, we use every single possible method. We use solar energy which is mainly for houses, and electric vehicle charging stations. We will use every single water body in our area for hydroelectric power. Lastly we will use wind turbines, which will be commonly installed in extremely windy areas. One energy solution which makes this city interplanetary is nuclear energy. The nuclear energy plants will be located in areas which have extremely less population. There will be only two plants, because that is enough to power the entire Sanicon Valley. This will be the main source of energy, as AI will be heavily used and it needs a lot of energy.</p>
  </div>

  <!-- Paragraph 7 -->
  <div class="z" data-s="60" data-e="69">
    <h1 class="big ab">Residential Layout</h1>
    <p class="para">A major part of the residential area is the layout of the average house. Each house will look the same as the houses in San Jose but there is a major difference. Every house will have one robot for the backyard. Another robot is optional and will be for helping with the household tasks and has the ability to communicate with other bots. Just by sitting, and without needing a phone, you can use the bot to instantly talk to anyone you want. It is like having a simulated visitor. You can also instantly order the bot to tell the backyard bot to give fruits or vegetables to the person you are talking to, virtually. The backyard has a vertical farm which has an enormous variety of fruits. These fruits use the shower and wasted tap water. Also after eating the fruits, the bot takes the remaining peel and uses it as compost, or uses the seed to grow another of that kind of plant. There is no sewage system, as the toilets and the shower drain are connected to a pipe which later goes to individual plants.</p>
  </div>

  <!-- Paragraph 8 -->
  <div class="z" data-s="70" data-e="79">
    <h1 class="big ag">Zoning Efficiency</h1>
    <p class="para">Now, this city has a very strict zoning law. All of the existing houses can stay as it is, but every new house can have a maximum area of 3,000 square feet excluding the backyard, and the backyard will have a maximum area of 1,000 square feet. The maximum height of the house is two floors, with each floor being max, 8 feet. This is because our city is trying to make every house just the minimum size needed, so that there is more space for other major infrastructure, especially space for energy plants. For the industrial zone, the maximum floors are 5 floors, each floor having a height of 10 feet along with the maximum area being 5,000 square feet. No industrial building will need more space than that. Hospitals will be really big so that more people can be treated at once reducing the wait time. The maximum area is 100,000 square feet, along with the maximum floors being 10 floors, with each floor being 10 feet high. Just 5 of these hospitals is enough to handle the whole Sanicon Valley at once.</p>
  </div>

  <!-- Paragraph 9 -->
  <div class="z" data-s="80" data-e="89">
    <h1 class="big ab">Land Use</h1>
    <p class="para">The benefits of these zoning laws is that there is a lot of space for schools which is enough to have almost every single kid having the access to education. Some space will be left for parks. Now the remaining space will be used for energy generation. Some space is for wind turbines, solar panels, and the majority of the space is for the nuclear power plants which will be secured and will be the farthest from the industries and the residential areas.</p>
  </div>

  <!-- Paragraph 10 -->
  <div class="z" data-s="90" data-e="100">
    <h1 class="big ag">Social Interaction</h1>
    <p class="para">The way that offices or small companies will be placed is the perfect way for socialization. The offices will be close by and it will be so that people can roam through different offices, and can see what is going on in the area. This makes everything more engaging and enables people to communicate with different small businesses so that they can combine ideas, making better ideas. These companies will be placed such that it is on the outline of a rectangle meaning that the center is a square where there are many restaurants, and various engaging activities, along with space for people to socialize. If people get bored, then they can take a peek on what the businesses are doing. With all of these innovations, Sanicon Valley is truly the city of the future.</p>
  </div>
</div>

<script>
const progress = document.getElementById('p');
const syncText = document.getElementById('u');
const modules = document.querySelectorAll('.z');
const canvas = document.getElementById('stars');
const ctx = canvas.getContext('2d');

let w, h;
let stars = [];

function init() {
  w = window.innerWidth;
  h = window.innerHeight;
  canvas.width = w;
  canvas.height = h;
  stars = [];
  for(let i=0; i<400; i++) {
    stars.push({ x: Math.random()*w, y: Math.random()*h, z: Math.random()*w });
  }
}

function update() {
  const scrollPos = window.scrollY;
  const maxScroll = document.documentElement.scrollHeight - h;
  const percent = (scrollPos / maxScroll) * 100;
  
  progress.style.width = percent + '%';
  syncText.innerText = `DATA STREAM: ${Math.floor(percent)}%`;

  modules.forEach(m => {
    const s = parseFloat(m.dataset.s);
    const e = parseFloat(m.dataset.e);
    
    if(percent >= s && percent <= e) {
      const pInRange = (percent - s) / (e - s);
      let op = 1;
      // Ultra-fast transitions
      if(pInRange < 0.1) op = pInRange * 10;
      if(pInRange > 0.9) op = (1 - pInRange) * 10;
      
      const scale = 0.05 + (pInRange * 5); // Dramatic zoom speed
      m.style.opacity = Math.min(op, 1);
      m.style.transform = `scale(${scale}) translateZ(0px)`;
      m.style.pointerEvents = op > 0.5 ? 'auto' : 'none';
    } else {
      m.style.opacity = 0;
      m.style.transform = `scale(0.01)`;
    }
  });

  // Background Star Warp
  ctx.fillStyle = '#000';
  ctx.fillRect(0,0,w,h);
  stars.forEach(s => {
    s.z -= 10; // High speed stars
    if(s.z <= 0) s.z = w;
    let sx = (s.x - w/2) * (w/s.z) + w/2;
    let sy = (s.y - h/2) * (w/s.z) + h/2;
    let sz = (w/s.z) * 1.5;
    ctx.fillStyle = `rgba(0, 210, 255, ${1 - s.z/w})`;
    ctx.beginPath(); ctx.arc(sx, sy, sz, 0, Math.PI*2); ctx.fill();
  });

  requestAnimationFrame(update);
}

window.addEventListener('resize', init);
init(); update();
</script>
