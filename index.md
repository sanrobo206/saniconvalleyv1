<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sanicon Valley — Final Interplanetary Manifesto</title>
    <style>
        @import url('https://fonts.googleapis.com');

        :root {
            --bambu: #00E676;
            --electric: #2979FF;
            --nuclear: #FFEA00;
            --waste: #FF3D00;
            --carbon: #050505;
            --white: #ffffff;
        }

        * { box-sizing: border-box; }

        body, html {
            margin: 0;
            padding: 0;
            background-color: var(--carbon);
            color: var(--white);
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* --- 1. THE HERO LANDING (FULL SCREEN) --- */
        .hero {
            height: 100vh;
            width: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle at center, #111 0%, #000 100%);
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(4rem, 15vw, 10rem);
            margin: 0;
            background: linear-gradient(90deg, var(--bambu), var(--electric), var(--nuclear));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            filter: drop-shadow(0 0 50px rgba(0, 230, 118, 0.4));
        }

        .hero p {
            letter-spacing: 20px;
            text-transform: uppercase;
            color: var(--electric);
            font-weight: 900;
            margin-top: 20px;
            opacity: 0.8;
        }

        /* --- 2. THE ZOOM ENGINE (FULL SECTION) --- */
        .zoom-engine {
            height: 400vh; /* Long scroll for smooth zoom */
            position: relative;
        }

        .sticky-view {
            position: sticky;
            top: 0;
            height: 100vh;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
        }

        /* SVG DIAGRAMS SCALE TO FILL SCREEN */
        .full-svg {
            width: 100vw;
            height: 100vh;
            transform: scale(1);
            transition: transform 0.1s linear, opacity 0.2s linear;
        }

        /* --- 3. TEXT CONTENT SECTIONS --- */
        .content-wrap {
            padding: 150px 10%;
            background: var(--carbon);
            position: relative;
            z-index: 100;
        }

        .manifesto-block {
            max-width: 1200px;
            margin: 0 auto 300px auto;
            opacity: 0;
            transform: translateY(100px);
            transition: all 1s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .manifesto-block.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .manifesto-block h2 {
            font-family: 'Orbitron';
            font-size: 3.5rem;
            margin-bottom: 40px;
            color: var(--bambu);
            border-left: 15px solid var(--electric);
            padding-left: 30px;
        }

        .manifesto-block p {
            font-size: 1.8rem;
            line-height: 1.8;
            color: #ccc;
            text-align: justify;
        }

        .highlight { color: var(--electric); font-weight: 900; }
        .nuclear-glow { color: var(--nuclear); font-weight: 900; text-shadow: 0 0 10px var(--nuclear); }

        footer {
            padding: 100px;
            text-align: center;
            border-top: 1px solid #222;
            font-family: 'Orbitron';
            letter-spacing: 8px;
            color: #444;
        }
    </style>
</head>
<body>

    <!-- HERO HUD -->
    <section class="hero">
        <p>INITIATING INTERPLANETARY LINK</p>
        <h1>SANICON VALLEY</h1>
        <p>SAN JOSE REBORN</p>
    </section>

    <!-- SECTION 1: CITY GRID ZOOM -->
    <div class="zoom-engine" id="cityZoomTrigger">
        <div class="sticky-view">
            <svg id="cityDiagram" class="full-svg" viewBox="0 0 1200 800" xmlns="http://www.w3.org">
                <rect width="1200" height="800" fill="#000" />
                <g stroke="#111" stroke-width="1">
                    <line x1="0" y1="400" x2="1200" y2="400" />
                    <line x1="600" y1="0" x2="600" y2="800" />
                </g>
                <!-- Nuclear Plants -->
                <rect x="50" y="50" width="120" height="120" fill="none" stroke="var(--nuclear)" stroke-width="4" />
                <circle cx="110" cy="110" r="10" fill="var(--nuclear)" />
                <text x="50" y="40" fill="var(--nuclear)" font-family="Orbitron" font-size="14">NUCLEAR_PLANT_NORTH</text>
                
                <rect x="1030" y="630" width="120" height="120" fill="none" stroke="var(--nuclear)" stroke-width="4" />
                <circle cx="1090" cy="690" r="10" fill="var(--nuclear)" />
                <text x="950" y="620" fill="var(--nuclear)" font-family="Orbitron" font-size="14">NUCLEAR_PLANT_SOUTH</text>

                <!-- City Matrix -->
                <circle cx="600" cy="400" r="300" fill="none" stroke="var(--electric)" stroke-width="2" stroke-dasharray="20,10" />
                <circle cx="600" cy="400" r="100" fill="none" stroke="var(--bambu)" stroke-width="5" />
                <text x="600" y="405" fill="white" font-family="Orbitron" font-size="24" text-anchor="middle">SANICON_CORE</text>
            </svg>
        </div>
    </div>

    <main class="content-wrap">
        <div class="manifesto-block">
            <h2>I. THE INTERPLANETARY HUB</h2>
            <p>Welcome to <span class="highlight">Sanicon Valley</span>, the one and only interplanetary future city, that lies on the great city of San Jose, far more advanced than many other cities in the world. Our city blends advanced technology, with nature, and repurposing waste for the greater good. Sanicon Valley is home to more than 1,000,000 residents, as it is the hub of social, economic, and technological advancement, with the forward thinking system of urban planning, and repurposing waste. Our city uses advanced technology to repurpose all kinds of waste to useful nutrients, energy, fuel, and more. We keep our city as simple as possible as we fix the major problem which has never been solved for decades in San Jose, which is to improve our farm to table system.</p>
        </div>

        <div class="manifesto-block">
            <h2>II. THE WATER CRISIS SOLUTION</h2>
            <p>There are many problems in San Jose. A major problem is the extreme water shortage in San Jose. Sanicon Valley not only fixes this problem, but also uses this problem to fix another major problem which is having enough water to keep the plants healthy. We will repurpose shower water which can be used to water the plants, so that the plants will be healthy with less water.</p>
        </div>
    </main>

    <!-- SECTION 2: VERTICAL FARM ZOOM -->
    <div class="zoom-engine" id="farmZoomTrigger">
        <div class="sticky-view">
            <svg id="farmDiagram" class="full-svg" viewBox="0 0 1200 800" xmlns="http://www.w3.org">
                <rect width="1200" height="800" fill="#050505" />
                <!-- Vertical Trays -->
                <rect x="400" y="100" width="400" height="40" fill="var(--bambu)" opacity="0.3" stroke="var(--bambu)" />
                <rect x="400" y="250" width="400" height="40" fill="var(--bambu)" opacity="0.5" stroke="var(--bambu)" />
                <rect x="400" y="400" width="400" height="40" fill="var(--bambu)" opacity="0.7" stroke="var(--bambu)" />
                <rect x="400" y="550" width="400" height="40" fill="var(--bambu)" stroke="var(--bambu)" />
                
                <!-- Water Recycling Pipe -->
                <path d="M300 100 L300 700 L400 700" stroke="var(--electric)" stroke-width="10" fill="none" />
                <text x="250" y="80" fill="var(--electric)" font-family="Orbitron" font-size="14">RECYCLED_SHOWER_WATER</text>
                <text x="500" y="700" fill="var(--bambu)" font-family="Orbitron" font-size="20">VERTICAL_BACKYARD_FARM</text>
            </svg>
        </div>
    </div>

    <main class="content-wrap">
        <div class="manifesto-block">
            <h2>III. BACKYARD AGRICULTURE</h2>
            <p>Also, every house has a <span class="highlight">vertical farm in their backyard</span>. This makes sure that everyone has a farm and a grocery store for agriculture in their own backyard. Everyone will have an app in which they can order a robot which will give the amount and kind of fruit or vegetable upon order. Whenever there is a surplus of fruits or vegetables in a house, then the app will send a notification that there is a surplus and then if the person accepts that they do not want it, then it will notify the entire community that anyone who wants can take it. This ensures that no food is wasted and even the poor can get fruits and vegetables. Also, this enables people to go to each other’s house, communicate, which builds a strong community, which San Jose currently lacks.</p>
        </div>

        <div class="manifesto-block">
            <h2>IV. CARBON CAPTURE & WASTE</h2>
            <p>Our city has little to no carbon footprint. This is because we trap carbon dioxide and use it for various different purposes, from fizz drinks, dry ice, to plants using it. The reason that this is an interplanetary solution is because the carbon dioxide can be used for various purposes like using plants to convert it to oxygen, for air in which you can breathe, and for other uses. We use various different kinds of waste for various different purposes, leaving almost zero net waste. For example we will use remaining food waste as compost, and remove some food remains from cooking oil which will be compost, while the remaining oil will be cleaned and used for soaps. Also other waste that cannot be used as compost, and has little to no nutrition will be used as biogas which will be used for the little gas powered cars. Fruit peels, especially oranges can be used as an organic pesticide.</p>
        </div>

        <div class="manifesto-block">
            <h2>V. AUTOMATION & TRANSPORT</h2>
            <p>In our city, there will be no supermarkets/grocery stores for fruits and vegetables, as every backyard is a farm. The only food items that will be sold will be meat, snacks, and drinks. This means that there is more space for recreational areas, and squares where people can meet together. This brings a stronger sense of community. Also, there will be zero farms, because every backyard is a farm. This makes more space for other important areas like, industrial areas, schools, and parks. For transportation the car and the bus are used. The train is not used because it takes too much space and it is limited to only a few areas. Every industry that involves manual labor will be automated, meaning that no one has to do that kind of work.</p>
        </div>

        <div class="manifesto-block">
            <h2>VI. PLASTIC REVOLUTION</h2>
            <p>Another problem which is worldwide is the effects of the traditional packaging methods. Now, Sanicon Valley still uses plastic as the packaging method, but there is a new innovation that solves pollution. There will be a law in which everyone has to throw away the plastic waste in a certain area and if they do not follow it, they will be heavily fined. This area is special, because it does not go to landfills, or even gets transported. In that bin, there will be <span class="highlight">plastic eating bacteria</span>, which will almost immediately decompose the plastic allowing there to be practically no plastic waste. Every single package will be made out of plastic.</p>
        </div>

        <div class="manifesto-block">
            <h2>VII. NUCLEAR ENERGY GRID</h2>
            <p>Our way of generating energy is one of the best ways. We do not just use one method, we use every single possible method. We use solar energy which is mainly for houses, and electric vehicle charging stations. We will use every single water body in our area for hydroelectric power. Lastly we will use wind turbines, which will be commonly installed in extremely windy areas. One energy solution which makes this city interplanetary is <span class="nuclear-glow">nuclear energy</span>. The nuclear energy plants will be located in areas which have extremely less population. There will be only two plants, because that is enough to power the entire Sanicon Valley. This will be the main source of energy, as AI will be heavily used and it needs a lot of energy.</p>
        </div>

        <div class="manifesto-block">
            <h2>VIII. ROBOTIC RESIDENTIALS</h2>
            <p>A major part of the residential area is the layout of the average house. Each house will look the same as the houses in San Jose but there is a major difference. Every house will have one robot for the backyard. Another robot is optional and will be for helping with the household tasks and has the ability to communicate with other bots. Just by sitting, and without needing a phone, you can use the bot to instantly talk to anyone you want. It is like having a simulated visitor. You can also instantly order the bot to tell the backyard bot to give fruits or vegetables to the person you are talking to, virtually. The backyard has a vertical farm which has an enormous variety of fruits. These fruits use the shower and wasted tap water. Also after eating the fruits, the bot takes the remaining peel and uses it as compost, or uses the seed to grow another of that kind of plant. There is no sewage system, as the toilets and the shower drain are connected to a pipe which later goes to individual plants.</p>
        </div>

        <div class="manifesto-block">
            <h2>IX. ZONING & SOCIAL SPACES</h2>
            <p>Now, this city has a very strict zoning law. All of the existing houses can stay as it is, but every new house can have a maximum area of 3,000 square feet excluding the backyard, and the backyard will have a maximum area of 1,000 square feet. The maximum height of the house is two floors, with each floor being max, 8 feet. This is because our city is trying to make every house just the minimum size needed, so that there is more space for other major infrastructure, especially space for energy plants. For the industrial zone, the maximum floors are 5 floors, each floor having a height of 10 feet along with the maximum area being 5,000 square feet. No industrial building will need more space than that. Hospitals will be really big so that more people can be treated at once reducing the wait time. The maximum area is 100,000 square feet, along with the maximum floors being 10 floors, with each floor being 10 feet high. Just 5 of these hospitals is enough to handle the whole Sanicon Valley at once.</p>
            <p>The benefits of these zoning laws is that there is a lot of space for schools which is enough to have almost every single kid having the access to education. Some space will be left for parks. Now the remaining space will be used for energy generation. Some space is for wind turbines, solar panels, and the majority of the space is for the nuclear power plants which will be secured and will be the farthest from the industries and the residential areas.</p>
            <p>The way that offices or small companies will be placed is the perfect way for socialization. The offices will be close by and it will be so that people can roam through different offices, and can see what is going on in the area. This makes everything more engaging and enables people to communicate with different small businesses so that they can combine ideas, making better ideas. These companies will be placed such that it is on the outline of a rectangle meaning that the center is a square where there are many restaurants, and various engaging activities, along with space for people to socialize. If people get bored, then they can take a peek on what the businesses are doing.</p>
        </div>
    </main>

    <footer>
        SANICON VALLEY INTERPLANETARY // CORE V1.0.9 // FINAL BUILD
    </footer>

    <script>
        const cityDiag = document.getElementById('cityDiagram');
        const farmDiag = document.getElementById('farmDiagram');
        const cityTrigger = document.getElementById('cityZoomTrigger');
        const farmTrigger = document.getElementById('farmZoomTrigger');
        const blocks = document.querySelectorAll('.manifesto-block');

        window.addEventListener('scroll', () => {
            // CITY ZOOM
            const cRect = cityTrigger.getBoundingClientRect();
            const cProg = -cRect.top / (cRect.height - window.innerHeight);
            if (cProg >= 0 && cProg <= 1) {
                cityDiag.style.transform = `scale(${1 + cProg * 14})`;
                cityDiag.style.opacity = cProg > 0.8 ? 1 - (cProg - 0.8) * 5 : 1;
            }

            // FARM ZOOM
            const fRect = farmTrigger.getBoundingClientRect();
            const fProg = -fRect.top / (fRect.height - window.innerHeight);
            if (fProg >= 0 && fProg <= 1) {
                farmDiag.style.transform = `scale(${1 + fProg * 14})`;
                farmDiag.style.opacity = fProg > 0.8 ? 1 - (fProg - 0.8) * 5 : 1;
            }

            // REVEAL ANIMATIONS
            blocks.forEach(b => {
                if (b.getBoundingClientRect().top < window.innerHeight * 0.85) {
                    b.classList.add('visible');
                }
            });
        });
    </script>
</body>
</html>
