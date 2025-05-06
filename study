<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SA7.L07 | Cyber Visionary</title>
    <style>
        :root {
            --primary: #1a1a1a;
            --accent: #00ff9d;
            --text: #e0e0e0;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Space Mono', monospace;
        }

        body {
            background: var(--primary);
            color: var(--text);
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* Matrix-like background effect */
        .digital-rain {
            position: fixed;
            z-index: -1;
            opacity: 0.1;
        }

        .container {
            padding: 4rem 8%;
            min-height: 100vh;
            position: relative;
        }

        .logo {
            position: fixed;
            top: 2rem;
            left: 2rem;
            font-family: 'Orbitron', sans-serif;
            font-size: 1.8rem;
            color: var(--accent);
            cursor: pointer;
            z-index: 100;
        }

        .portal-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 8rem;
        }

        .portal-card {
            background: rgba(255, 255, 255, 0.02);
            border: 1px solid rgba(255, 255, 255, 0.1);
            padding: 2rem;
            cursor: pointer;
            transition: all 0.4s cubic-bezier(0.215, 0.610, 0.355, 1);
            position: relative;
            overflow: hidden;
        }

        .portal-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, var(--accent), transparent);
            transform: rotate(45deg);
            opacity: 0;
            transition: 0.5s;
        }

        .portal-card:hover::before {
            opacity: 0.2;
            animation: glitch 0.8s infinite;
        }

        .portal-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 0 30px rgba(0, 255, 157, 0.1);
        }

        .back-btn {
            position: fixed;
            top: 2rem;
            right: 2rem;
            cursor: pointer;
            opacity: 0;
            transition: 0.3s;
        }

        /* Content Sections */
        .section {
            display: none;
            opacity: 0;
            max-width: 800px;
            margin: 4rem auto;
            padding: 2rem;
            border-left: 3px solid var(--accent);
        }

        .section.active {
            display: block;
            animation: contentAppear 1s forwards;
        }

        @keyframes glitch {
            0% { transform: rotate(45deg) translate(0); }
            20% { transform: rotate(45deg) translate(-5px, 5px); }
            40% { transform: rotate(45deg) translate(5px, -5px); }
            60% { transform: rotate(45deg) translate(-5px, 5px); }
            80% { transform: rotate(45deg) translate(5px, -5px); }
            100% { transform: rotate(45deg) translate(0); }
        }

        @keyframes contentAppear {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Space+Mono&family=Orbitron&display=swap" rel="stylesheet">
</head>
<body>
    <div class="logo">@SA7.L07</div>
    
    <!-- Main Portal -->
    <div class="container" id="mainPortal">
        <div class="portal-grid">
            <div class="portal-card" data-section="cyber">
                <h2>// Cyber Genesis</h2>
                <p>Explore my digital odyssey</p>
            </div>
            
            <div class="portal-card" data-section="photography">
                <h2>// Frozen Moments</h2>
                <p>Through the lens of time</p>
            </div>

            <div class="portal-card" data-section="essence">
                <h2>// Binary Soul</h2>
                <p>Human behind the code</p>
            </div>
        </div>
    </div>

    <!-- Sections -->
    <div class="section" id="cyber">
        <h1>The Code That Shapes Me</h1>
        <p>".................... "</p>
    </div>

    <div class="section" id="photography">
        <h1>Capturing Light in Darkness</h1>
        <p>In the corridors of The Indian School Bahrain, I discovered... </p>
    </div>

    <div class="section" id="essence">
        <h1>Between 1s and 0s</h1>
        <p>.......................]</p>
    </div>

    <div class="back-btn" onclick="showPortal()">↩ RETURN TO VOID</div>

    <script>
        document.querySelectorAll('.portal-card').forEach(card => {
            card.addEventListener('click', () => {
                document.getElementById('mainPortal').style.display = 'none';
                document.querySelector('.back-btn').style.opacity = '1';
                const section = document.getElementById(card.dataset.section);
                section.classList.add('active');
            });
        });

        function showPortal() {
            document.getElementById('mainPortal').style.display = 'block';
            document.querySelector('.back-btn').style.opacity = '0';
            document.querySelectorAll('.section').forEach(section => {
                section.classList.remove('active');
            });
        }
    </script>
</body>
</html>
