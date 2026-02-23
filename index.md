<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sanicon Valley | Interplanetary Manifesto</title>
    <style>
        @import url('https://fonts.googleapis.com');

        :root {
            --bambu-green: #00E676;
            --electric-blue: #2979FF;
            --nuclear-yellow: #FFEA00;
            --waste-red: #FF3D00;
            --carbon: #050505;
            --white: #ffffff;
            --glass: rgba(255, 255, 255, 0.05);
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

        /* --- 1. THE HERO HUD --- */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
            z-index: 10;
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(3rem, 10vw, 8rem);
            margin: 0;
            background: linear-gradient(90deg, var(--bambu-green), var(--electric-blue), var(--nuclear-yellow));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            filter: drop-shadow(0 0 30px rgba(0, 230, 118, 0.3));
        }

        .hero p {
            letter-spacing: 12px;
            text-transform: uppercase;
            color: var(--electric-blue);
            font-weight: 900;
            margin-top: 20px;
        }

        /* --- 2. THE MASSIVE ZOOM TRIGGER --- */
        .zoom-scroll-engine {
            height: 400vh; /* Controlled scroll duration */
            position: relative;
            background: #000;
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

        /* --- 3. THE HAND-CODED CITY DIAGRAM --- */
        #cityDiagram {
            width: 90%;
            height: 90%;
            transform: scale(1);
            opacity: 1;
            transition: transform 0.1s linear, opacity 0.2s linear;
        }

        /* --- 4. TEXT ANIMATION SYSTEM --- */
        .manifesto-container {
            position: relative;
            z-index: 100;
            background: var(--carbon);
            padding: 100px 10%;
        }

        .text-block {
            max-width: 1100px;
            margin: 0 auto 250px auto;
            opacity: 0;
            transform: translateY(100px) scale(0.95);
            transition: all 1.2s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .text-block.active {
            opacity: 1;
            transform: translateY(0) scale(1);
        }

        .text-block h2 {
            font-family: 'Orbitron';
            font-size: 2.5rem;
            margin-bottom: 40px;
            color: var(--bambu-green);
            border-left: 8px solid var(--electric-blue);
            padding-left: 25px;
        }

        .text-block p {
            font-size: 1.5rem;
            line-height: 2;
            color: #ddd;
            text-align: justify;
            margin-bottom: 30px;
        }

        .highlight { color: var(--electric-blue); font-weight: 900; }
        .nuclear { color: var(--nuclear-yellow); font-weight: 900; }

        footer {
            padding: 100px;
            text-align: center;
            border-top: 1px solid #222;
            font-family: 'Orbitron';
            letter-spacing: 5px;
            color: #555;
        }

    </style>
</head>
<body>

    <section class="hero">
        <h1>SANICON VALLEY</h1>
        <p>Interplanetary Future City</p>
    </section>

    <!-- ZOOMING DIAGRAM SECTION -->
    <div class="zoom-scroll-engine" id="zoomContainer">
        <div class="sticky-view">
            <svg id="cityDiagram" viewBox="0 0 1000 800" xmlns="http://www.w3.org">
                <!-- Outer Grid -->
                <defs>
                    <radialGradient id="nodeGlow" cx="50%" cy="50%" r="50%">
                        <stop offset="0%" stop-color="#00E676" stop-opacity="0.6""")/>>
                        <stop offset="100%" stop-color="#000" stop-opacity="0""")/>>
                    </radialGradient>
                </defs>
                
                <rect x="0" y="0" width="1000" height="800" fill="none" stroke="#111" stroke-width="2" />
                
                <!-- City Zoning Circles -->
                <circle cx="500" cy="400" r="350" fill="none" stroke="#222" stroke-width="1" />
                <circle cx="500" cy="400" r="200" fill="none" stroke="#333" stroke-width="2" stroke-dasharray="15,15" />
                
                <!-- Power Plants (Nuclear) -->
                <g>
                    <rect x="50" y="50" width="80" height="80" fill="none" stroke="var(--nuclear-yellow)" stroke-width="3" />
                    <circle cx="90" cy="90" r="10" fill="var(--nuclear-yellow)" />
                    <text x="50" y="40" fill="var(--nuclear-yellow)" font-family="Orbitron" font-size="12">NUCLEAR_PLANT_01</text>
                </g>
                <g>
                    <rect x="870" y="670" width="80" height="80" fill="none" stroke="var(--nuclear-yellow)" stroke-width="3" />
                    <circle cx="910" cy="710" r="10" fill="var(--nuclear-yellow)" />
                    <text x="820" y="660" fill="var(--nuclear-yellow)" font-family="Orbitron" font-size="12">NUCLEAR_PLANT_02</text>
                </g>

                <!-- Residential Mesh -->
                <circle cx="300" cy="300" r="15" fill="var(--bambu-green)" />
                <circle cx="700" cy="300" r="15" fill="var(--bambu-green)" />
                <circle cx="300" cy="500" r="15" fill="var(--bambu-green)" />
                <circle cx="700" cy="500" r="15" fill="var(--bambu-green)" />
                
                <!-- Interplanetary Link -->
                <line x1="500" y1="400" x2="90" y2="90" stroke="var(--electric-blue)" stroke-width="1" opacity="0.4" />
                <line x1="500" y1="400" x2="910" y2="710" stroke="var(--electric-blue)" stroke-width="1" opacity="0.4" />

                <!-- Central Core -->
                <circle cx="500" cy="400" r="50" fill="url(#nodeGlow)" />
                <text x="500" y="405" fill="white" font-family="Orbitron" font-size="18" text-anchor="middle">SANICON_CORE</text>
            </svg>
        </div>
    </div>

    <!-- THE FULL MANIFESTO TEXT -->
    <main class="manifesto-container">

        <div class="text-block">
            <h2>01. THE INTERPLANETARY HUB</h2>
            <p>Welcome to <span class="highlight">Sanicon Valley</span>, the one and only interplanetary future city, that lies on the great city of San Jose, far more advanced than many other cities in the world. Our city blends advanced technology, with nature, and repurposing waste for the greater good.</p>
            <p>Sanicon Valley is home to more than 1,000,000 residents, as it is the hub of social, economic, and technological advancement, with the forward thinking system of urban planning, and repurposing waste. Our city uses advanced technology to repurpose all kinds of waste to useful nutrients, energy, fuel, and more. We keep our city as simple as possible as we fix the major problem which has never been solved for decades in San Jose, which is to improve our farm to table system.</p>
        </div>

        <div class="text-block">
            <h2>02. WATER REPURPOSING & AGRICULTURE</h2>
            <p>There are many problems in San Jose. A major problem is the extreme water shortage in San Jose. Sanicon Valley not only fixes this problem, but also uses this problem to fix another major problem which is having enough water to keep the plants healthy. We will repurpose shower water which can be used to water the plants, so that the plants will be healthy with less water.</p>
            <p>Also, every house has a <span class="highlight">vertical farm in their backyard</span>. This makes sure that everyone has a farm and a grocery store for agriculture in their own backyard. Everyone will have an app in which they can order a robot which will give the amount and kind of fruit or vegetable upon order. Whenever there is a surplus of fruits or vegetables in a house, then the app will send a notification that there is a surplus and then if the person accepts that they do not want it, then it will notify the entire community that anyone who wants can take it. This ensures that no food is wasted and even the poor can get fruits and vegetables. Also, this enables people to go to each other’s house, communicate, which builds a strong community, which San Jose currently lacks.</p>
        </div>

        <div class="text-block">
            <h2>03. CARBON CAPTURE & ZERO WASTE</h2>
            <p>Our city has little to no carbon footprint. This is because we trap carbon dioxide and use it for various different purposes, from fizz drinks, dry ice, to plants using it. The reason that this is an interplanetary solution is because the carbon dioxide can be used for various purposes like using plants to convert it to oxygen, for air in which you can breathe, and for other uses.</p>
            <p>We use various different kinds of waste for various different purposes, leaving almost zero net waste. For example we will use remaining food waste as compost, and remove some food remains from cooking oil which will be compost, while the remaining oil will be cleaned and used for soaps. Also other waste that cannot be used as compost, and has little to no nutrition will be used as biogas which will be used for the little gas powered cars. Fruit peels, especially oranges can be used as an organic pesticide.</p>
        </div>

        <div class="text-block">
            <h2>04. AUTOMATION & TRANSPORTATION</h2>
            <p>In our city, there will be no supermarkets/grocery stores for fruits and vegetables, as every backyard is a farm. The only food items that will be sold will be meat, snacks, and drinks. This means that there is more space for recreational areas, and squares where people can meet together. This brings a stronger sense of community. Also, there will be zero farms, because every backyard is a farm. This makes more space for other important areas like, industrial areas, schools, and parks. For transportation the car and the bus are used. The train is not used because it takes too much space and it is limited to only a few areas. Every industry that involves manual labor will be automated, meaning that no one has to do that kind of work.</p>
        </div>

        <div class="text-block">
            <h2>05. POLLUTION & PLASTIC BACTERIA</h2>
            <p>Another problem which is worldwide is the effects of the traditional packaging methods. Now, Sanicon Valley still uses plastic as the packaging method, but there is a new innovation that solves pollution. There will be a law in which everyone has to throw away the plastic waste in a certain area and if they do not follow it, they will be heavily fined. This area is special, because it does not go to landfills, or even gets transported. In that bin, there will be <span class="highlight">plastic eating bacteria</span>, which will almost immediately decompose the plastic allowing there to be practically no plastic waste. Every single package will be made out of plastic.</p>
        </div>

        <div class="text-block">
            <h2>06. NUCLEAR & CLEAN ENERGY</h2>
            <p>Our way of generating energy is one of the best ways. We do not just use one method, we use every single possible method. We use solar energy which is mainly for houses, and electric vehicle charging stations. We will use every single water body in our area for hydroelectric power. Lastly we will use wind turbines, which will be commonly installed in extremely windy areas.</p>
            <p>One energy solution which makes this city interplanetary is <span class="nuclear">nuclear energy</span>. The nuclear energy plants will be located in areas which have extremely less population. There will be only two plants, because that is enough to power the entire Sanicon Valley. This will be the main source of energy, as AI will be heavily used and it needs a lot of energy.</p>
        </div>

        <div class="text-block">
            <h2>07. ROBOTIC HOUSEHOLD LOGIC</h2>
            <p>A major part of the residential area is the layout of the average house. Each house will look the same as the houses in San Jose but there is a major difference. Every house will have one robot for the backyard. Another robot is optional and will be for helping with the household tasks and has the ability to communicate with other bots. Just by sitting, and without needing a phone, you can use the bot to instantly talk to anyone you want. It is like having a simulated visitor. You can also instantly order the bot to tell the backyard bot to give fruits or vegetables to the person you are talking to, virtually. The backyard has a vertical farm which has an enormous variety of fruits. These fruits use the shower and wasted tap water. Also after eating the fruits, the bot takes the remaining peel and uses it as compost, or uses the seed to grow another of that kind of plant. There is no sewage system, as the toilets and the shower drain are connected to a pipe which later goes to individual plants.</p>
        </div>

        <div class="text-block">
            <h2>08. STRICT ZONING LAWS</h2>
            <p>Now, this city has a very strict zoning law. All of the existing houses can stay as it is, but every new house can have a maximum area of 3,000 square feet excluding the backyard, and the backyard will have a maximum area of 1,000 square feet. The maximum height of the house is two floors, with each floor being max, 8 feet. This is because our city is trying to make every house just the minimum size needed, so that there is more space for other major infrastructure, especially space for energy plants. For the industrial zone, the maximum floors are 5 floors, each floor having a height of 10 feet along with the maximum area being 5,000 square feet. No industrial building will need more space than that. Hospitals will be really big so that more people can be treated at once reducing the wait time. The maximum area is 100,000 square feet, along with the maximum floors being 10 floors, with each floor being 10 feet high. Just 5 of these hospitals is enough to handle the whole Sanicon Valley at once.</p>
            <p>The benefits of these zoning laws is that there is a lot of space for schools which is enough to have almost every single kid having the access to education. Some space will be left for parks. Now the remaining space will be used for energy generation. Some space is for wind turbines, solar panels, and the majority of the space is for the nuclear power plants which will be secured and will be the farthest from the industries and the residential areas.</p>
        </div>

        <div class="text-block">
            <h2>09. SOCIAL SPACES & COMMERCE</h2>
            <p>The way that offices or small companies will be placed is the perfect way for socialization. The offices will be close by and it will be so that people can roam through different offices, and can see what is going on in the area. This makes everything more engaging and enables people to communicate with different small businesses so that they can combine ideas, making better ideas. These companies will be placed such that it is on the outline of a rectangle meaning that the center is a square where there are many restaurants, and various engaging activities, along with space for people to socialize. If people get bored, then they can take a peek on what the businesses are doing.</p>
        </div>

    </main>

    <footer>
        SANICON VALLEY INTERPLANETARY // CORE V1.0 // FINAL REVISION
    </footer>

    <script>
        const diagram = document.getElementById('cityDiagram');
        const zoomTrigger = document.getElementById('zoomContainer');
        const blocks = document.querySelectorAll('.text-block');

        window.addEventListener('scroll', () => {
            // 1. ZOOM LOGIC
            const rect = zoomTrigger.getBoundingClientRect();
            const scrollPercent = -rect.top / (rect.height - window.innerHeight);
            
            if (scrollPercent >= 0 && scrollPercent <= 1) {
                // MASSIVE 15x ZOOM
                const scaleValue = 1 + (scrollPercent * 14);
                diagram.style.transform = `scale(${scaleValue})`;
                
                // FADE OUT AT 80% SCROLL
                if (scrollPercent > 0.8) {
                    diagram.style.opacity = 1 - ((scrollPercent - 0.8) * 5);
                } else {
                    diagram.style.opacity = 1;
                }
            }

            // 2. REVEAL ANIMATIONS
            blocks.forEach(block => {
                const bTop = block.getBoundingClientRect().top;
                if (bTop < window.innerHeight * 0.85) {
                    block.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
