<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>SCC | Simulador de Colectivos Cordobeses</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Rajdhani:wght@500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --ersa-red: #e31e24;
            --coniferal-orange: #f39200;
            --inter-green: #2ecc71;
            --fonobus-blue: #0055a4;
            --neon-blue: #00f2ff;
            --bg-black: #050507;
            --gold: #ffd700;
        }

        body {
            margin: 0;
            background-color: var(--bg-black);
            color: white;
            font-family: 'Rajdhani', sans-serif;
            overflow-x: hidden;
        }

        .hero {
            height: 60vh;
            background: linear-gradient(rgba(0,0,0,0.6), var(--bg-black)), 
                        url('https://r2.community.samsungsurvey.com/aside/a658276f62774989b6c0717387d3a870') center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            border-bottom: 4px solid var(--ersa-red);
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(2.5rem, 8vw, 5rem);
            margin: 0;
            text-shadow: 0 0 20px rgba(227, 30, 36, 0.8);
        }

        .container { padding: 40px 10%; }

        h2.section-title {
            font-family: 'Orbitron', sans-serif;
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 40px;
            text-transform: uppercase;
            letter-spacing: 5px;
        }

        .grid-empresas {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-bottom: 80px;
        }

        .card {
            background: rgba(255,255,255,0.03);
            border-radius: 15px;
            padding: 25px;
            border: 1px solid rgba(255,255,255,0.1);
            transition: 0.3s;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .card:hover {
            transform: translateY(-10px);
            background: rgba(255,255,255,0.07);
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }

        .full-border { border-top: 5px solid var(--gold); }
        .free-border { border-top: 5px solid var(--neon-blue); }

        .badge {
            display: inline-block;
            padding: 5px 15px;
            border-radius: 5px;
            font-weight: bold;
            font-size: 0.8rem;
            margin-bottom: 15px;
            text-transform: uppercase;
        }

        .badge-full { background: var(--gold); color: black; }
        .badge-free { background: var(--neon-blue); color: black; }

        .price-tag {
            font-size: 1.8rem;
            color: var(--neon-blue);
            font-weight: bold;
            margin-top: 15px;
            font-family: 'Orbitron';
        }

        .release-box {
            text-align: center;
            background: linear-gradient(45deg, #111, #1a1a1a);
            padding: 40px;
            border-radius: 30px;
            border: 2px solid var(--neon-blue);
            margin: 50px 0;
        }

        .countdown-container {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 20px 0;
        }

        .time-segment {
            background: rgba(255, 255, 255, 0.05);
            padding: 15px;
            border-radius: 10px;
            min-width: 70px;
            border-bottom: 2px solid var(--neon-blue);
        }

        .time-val { font-family: 'Orbitron'; font-size: 1.8rem; color: var(--neon-blue); display: block; }

        .discord-btn {
            background: #5865F2;
            color: white;
            padding: 15px 35px;
            border-radius: 10px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            margin-top: 20px;
            transition: 0.3s;
        }

        .discord-btn:hover { background: #4752c4; transform: scale(1.05); }
    </style>
</head>
<body>

    <section class="hero">
        <h1>SCC <span style="color: var(--ersa-red);">CORDOBESES</span></h1>
        <p style="letter-spacing: 3px;">SIMULADOR DE COLECTIVOS CORDOBESES</p>
        <a href="https://discord.gg/MCt99e8a" class="discord-btn">UNITE AL DISCORD OFICIAL DE SCC</a>
    </section>

    <div class="container">
        
        <!-- SECCIÓN FULL -->
        <h2 class="section-title" style="color: var(--gold);">pases scc</h2>
        <div class="grid-empresas">
            <!-- COCHE 1 -->
            <div class="card full-border">
                <div>
                    <span class="badge badge-full">EMPRESA FULL</span>
                    <h3>ERSA</h3>
                    <p>NUEVOBUS CITTA O500U. El VIP del juego con muchas mas cosas.</p>
                </div>
                <div class="price-tag">150 <small style="font-size: 0.8rem;">ROBUX</small></div>
            </div>

            <!-- COCHE 2 -->
            <div class="card full-border" style="border-top-color: var(--inter-green);">
                <div>
                    <span class="badge badge-full" style="background: var(--inter-green);">intercordoba pase</span>
                    <h3>INTERCORDOBA</h3>
                    <p>ITALBUS TROPEA IV INTERURBANO (Interno 409).</p>
                </div>
                <div class="price-tag">50 <small style="font-size: 0.8rem;">ROBUX</small></div>
            </div>

            <!-- COCHE 3 (NUEVO) -->
            <div class="card full-border" style="border-top-color: var(--coniferal-orange);">
                <div>
                    <span class="badge badge-full" style="background: var(--coniferal-orange); color: white;">coniferal pase</span>
                    <h3>CONIFERAL</h3>
                    <p>nuovobus citta 0500u (linea 62) beneficios en discord.</p>
                </div>
                <div class="price-tag">65 <small style="font-size: 0.8rem;">ROBUX</small></div>
            </div>

            
        </div>

        <!-- SECCIÓN FREE -->
        <h2 class="section-title" style="color: var(--neon-blue);">Empresas Free</h2>
        <div class="grid-empresas">
            <div class="card free-border" style="border-top-color: var(--coniferal-orange);">
                <span class="badge badge-free">GRATIS</span>
                <h3>CONIFERAL</h3>
                <p>empresa de cordoba emblematica por sus recorridos.</p>
            </div>
            <div class="card free-border" style="border-top-color: var(--tamse-blue);">
                <span class="badge badge-free">GRATIS</span>
                <h3>TAMSE</h3>
                <p>proximamente en scc.</p>
            </div>
            <div class="card free-border">
                <span class="badge badge-free">GRATIS</span>
                <h3>SI BUS</h3>
                <p>empresa linda con muchos modelos de colectivos
													  .</p>
            </div>
        </div>

        <!-- CUENTA REGRESIVA -->
        <div class="release-box">
            <h3 style="font-family: 'Orbitron'; margin: 0; color: #888;">FALTAN</h3>
            <div class="countdown-container">
                <div class="time-segment"><span class="time-val" id="days">00</span><span>Días</span></div>
                <div class="time-segment"><span class="time-val" id="hours">00</span><span>Hs</span></div>
                <div class="time-segment"><span class="time-val" id="minutes">00</span><span>Min</span></div>
                <div class="time-segment"><span class="time-val" id="seconds">00</span><span>Seg</span></div>
            </div>
            <p style="font-weight: bold; font-size: 1.5rem; letter-spacing: 2px;">LANZAMIENTO: 10 / 06 / 2026</p>
        </div>

    </div>

    <footer style="text-align: center; padding: 40px; color: #555; background: #020202;">
        <p>SCC STAFF &copy; 2026 - SIMULADOR DE COLECTIVOS CORDOBESES</p>
    </footer>

    <script>
        const launchDate = new Date("June 10, 2026 00:00:00").getTime();
        setInterval(function() {
            const now = new Date().getTime();
            const diff = launchDate - now;
            if (diff > 0) {
                document.getElementById("days").innerHTML = Math.floor(diff / (1000 * 60 * 60 * 24)).toString().padStart(2, '0');
                document.getElementById("hours").innerHTML = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)).toString().padStart(2, '0');
                document.getElementById("minutes").innerHTML = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60)).toString().padStart(2, '0');
                document.getElementById("seconds").innerHTML = Math.floor((diff % (1000 * 60)) / 1000).toString().padStart(2, '0');
            } else {
                document.querySelector(".countdown-container").innerHTML = "<h2>¡YA DISPONIBLE!</h2>";
            }
        }, 1000);
    </script>
</body>
</html>
