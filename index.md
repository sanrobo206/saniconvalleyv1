<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sanicon Valley — Ultimate Centered Manifesto</title>
    <style>
        @import url('https://fonts.googleapis.com');

        :root {
            --bambu: #00E676;
            --electric: #2979FF;
            --nuclear: #FFEA00;
            --carbon: #000000;
            --white: #ffffff;
            /* High-Intensity Glow Variable */
            --nuclear-glow: 0 0 30px #FFEA00, 0 0 60px #FFEA00;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }

        body, html {
            background-color: var(--carbon);
            color: var(--white);
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
            width: 100vw;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* --- 1. HERO SECTION (CENTERED) --- */
        .hero {
            height: 100vh;
            width: 100vw;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle at center, #111 0%, #000 100%);
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(3rem, 15vw, 10rem);
            background: linear-gradient(90deg, var(--bambu), var(--electric), var(--nuclear));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            filter: drop-shadow(0 0 50px rgba(0, 230, 118, 0.5));
            animation: pulse-glow 3s infinite ease-in-out;
        }

        @keyframes pulse-glow {
            0% { filter: drop-shadow(0 0 20px rgba(0, 230, 118, 0.3)); }
            50% { filter: drop-shadow(0 0 60px rgba(0, 230, 118, 0.7)); }
            100% { filter: drop-shadow(0 0 20px rgba(0, 230, 118, 0.3)); }
        }

        /* --- 2. THE ZOOM ENGINE --- */
        .zoom-engine {
            height: 400vh;
            width: 100vw;
            position: relative;
        }

        .sticky-wrapper {
            position: sticky;
            top: 0;
            height: 100vh;
            width: 100vw;
            display: flex;
            justify-content: center;
            align-items: center;
            background: #000;
        }

        .full-svg {
            width: 100%;
            height: 100%;
            transform: scale(1);
            transition: transform 0.1s linear, opacity 0.2s linear;
        }

        /* --- 3. MANIFESTO CONTENT (MAX CENTERING) --- */
        .manifesto-body {
            padding: 100px 5%;
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            background: var(--carbon);
        }

        .text-block {
            width: 100%;
            max-width: 1100px;
            margin-bottom: 350px;
            opacity: 0;
            transform: translateY(100px);
            transition: all 1.2s cubic-bezier(0.16, 1, 0.3, 1);
            text-align: center;
        }

        .text-block.active {
            opacity: 1;
            transform: translateY(0);
        }

        .text-block h2 {
            font-family: 'Orbitron';
            font-size: clamp(2rem, 5vw, 4rem);
            margin-bottom: 40px;
            color: var(--bambu);
            display: inline-block;
            padding-bottom: 10px;
            border-bottom: 5px solid var(--electric);
        }

        .nuclear-header {
            color: var(--nuclear) !important;
            text-shadow: var(--nuclear-glow);
            border-bottom: 5px solid var(--nuclear) !important;
            animation: nuclear-pulse 2s infinite ease-in-out;
        }

        @keyframes nuclear-pulse {
            0% { text-shadow: 0 0 20px #FFEA00; }
            50% { text-shadow: 0 0 50px #FFEA00, 0 0 80px #FFEA00; }
            100% { text-shadow: 0 0 20px #FFEA00; }
        }

        .text-block p {
            font-size: clamp(1.2rem, 2.2vw, 1.9rem);
            line-height: 1.9;
            color: #ddd;
            margin-bottom: 2rem;
            text-align: center;
        }

        .highlight { color: var(--electric); font-weight: 900; }

        footer {
            padding: 100px;
            width: 100%;
            text-align: center;
            border-top: 1px solid #222;
            font-family: 'Orbitron';
            letter-spacing: 12px;
            color: #444;
        }
    </style>
</head>
<body>

    <section class="hero">
        <p style="letter-spacing: 15px; color: var(--electric); font-weight: 900;">SYSTEM_LINK // INTERPLANETARY</p>
        <h1>SANICON VALLEY</h1>
        <p style="letter-spacing: 12px; color: var(--white); opacity: 0.8; margin-top: 15px;">SAN JOSE REIMAGINED</p>
    </section>

    <!-- CITY MATRIX ZOOM -->
    <div class="zoom-engine" id="cityZoom">
        <div class="sticky-wrapper">
            <svg id="cityDiagram" class="full-svg" viewBox="0 0 1200 800" xmlns="http://www.w3.org">
                <rect width="1200" height="800" fill="#000" />
                <circle cx="600" cy="400" r="350" fill="none" stroke="var(--electric)" stroke-width="2" stroke-dasharray="20,10" />
                <circle cx="600" cy="400" r="150" fill="none" stroke="var(--bambu)" stroke-width="6" />
                <text x="600" y="410" fill="white" font-family="Orbitron" font-size="32" text-anchor="middle">SANICON_CORE</text>
                <!-- Nuclear Glow Nodes -->
                <circle cx="150" cy="150" r="20" fill="var(--nuclear)">
                    <animate attributeName="opacity" values="0.3;1;0.3" dur="2s" repeatCount="indefinite" />
                </circle>
                <text x="150" y="110" fill="var(--nuclear)" font-family="Orbitron" font-size="16" text-anchor="middle">NUCLEAR_PLANT_ALPHA</text>
            </svg>
        </div>
    </div>

    <main class="manifesto-body">
        <div class="text-block">
            <h2>I. THE HUB OF ADVANCEMENT</h2>
            <p>Welcome to <span class="highlight">Sanicon Valley</span>, the one and only interplanetary future city. Our city blends advanced technology with nature, repurposing waste for the greater good. Sanicon Valley is home to more than 1,000,000 residents, serving as the global hub of social and technological advancement.</p>
            <p>Our city fixes the major problems of San Jose, starting with a revolutionary farm-to-table system that integrates agriculture directly into the urban layout.</p>
        </div>

        <div class="text-block">
            <h2 class="nuclear-header">II. NUCLEAR ENERGY PROTOCOL</h2>
            <p>One energy solution which makes this city interplanetary is <span class="highlight">nuclear energy</span>. The nuclear energy plants are located in low-population areas. Just two plants are enough to power the entire Sanicon Valley, fueling the AI-driven infrastructure that requires massive power loads.</p>
            <p>We use every possible method: solar energy for houses, hydroelectric power from local water bodies, and wind turbines in high-velocity areas.</p>
        </div>

        <div class="text-block">
            <h2>III. THE BIO-FARM BACKYARD</h2>
            <p>Every house has a vertical farm in their backyard. We repurpose <span class="highlight">shower water</span> to keep plants healthy with minimal fresh water usage. An integrated app and robotic system ensure that food surpluses are distributed to the community, building social bonds San Jose currently lacks.</p>
            <p>No food is wasted. Robotic bots take remaining peels for compost or seeds for replanting, creating a perfect zero-waste cycle.</p>
        </div>

        <div class="text-block">
            <h2>IV. ZONING & SOCIAL COMMERCE</h2>
            <p>Strict zoning laws ensure maximum space for energy and infrastructure. New houses are capped at 3,000 square feet, and industrial areas are automated for maximum efficiency. Offices are placed in a rectangular outline centered around <span class="highlight">social squares</span> filled with restaurants and engagement hubs.</p>
            <p>By trapping carbon dioxide and using it for everything from fizz drinks to oxygen conversion, Sanicon Valley leaves zero net waste.</p>
        </div>
    </main>

    <footer>SANICON VALLEY // FINAL BUILD // MAX GLOW ACTIVE</footer>

    <script>
        const cityDiag = document.getElementById('cityDiagram');
        const cityTrigger = document.getElementById('cityZoom');
        const blocks = document.querySelectorAll('.text-block');

        window.addEventListener('scroll', () => {
            const cRect = cityTrigger.getBoundingClientRect();
            const cProg = -cRect.top / (cRect.height - window.innerHeight);
            if (cProg >= 0 && cProg <= 1) {
                cityDiag.style.transform = `scale(${1 + cProg * 14})`;
                cityDiag.style.opacity = cProg > 0.8 ? 1 - (cProg - 0.8) * 5 : 1;
            }

            blocks.forEach(b => {
                if (b.getBoundingClientRect().top < window.innerHeight * 0.9) {
                    b.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
