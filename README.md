# Tipster-Hub-Sardegna-
Tips a portata di mano 
<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calcio Performance</title>
    <style>
        /* Reset e font */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            overflow-x: hidden;
        }

        /* Sfondo calcio */
        .background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1505678261036-a3fcc5e884ee?auto=format&fit=crop&w=1950&q=80') no-repeat center center;
            background-size: cover;
            z-index: -2;
        }

        /* Overlay blu scuro */
        .overlay {
            background-color: rgba(10, 26, 51, 0.85);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 60px 20px;
            text-align: center;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        p {
            font-size: 1.3rem;
            max-width: 700px;
            margin-bottom: 50px;
            line-height: 1.6;
        }

        /* Pulsante animato con effetto luce */
        a.button {
            display: inline-block;
            background: linear-gradient(90deg, #1E5EFF, #4A7BFF);
            color: white;
            padding: 15px 50px;
            border-radius: 10px;
            text-decoration: none;
            font-size: 1.3rem;
            font-weight: bold;
            transition: 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            position: relative;
            overflow: hidden;
        }

        a.button::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: rgba(255,255,255,0.2);
            transform: rotate(45deg);
            transition: all 0.5s;
        }

        a.button:hover::after {
            top: -20%;
            left: -20%;
        }

        a.button:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.5);
        }

        /* Palloni da calcio animati */
        .icons {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            overflow: hidden;
            z-index: -1;
        }

        .icon {
            position: absolute;
            width: 50px;
            opacity: 0.7;
            animation: float linear infinite;
        }

        @keyframes float {
            0% { transform: translateY(100vh) translateX(0) rotate(0deg); opacity: 0; }
            10% { opacity: 0.7; }
            100% { transform: translateY(-100px) translateX(100px) rotate(360deg); opacity: 0; }
        }

        /* Responsive */
        @media (max-width: 768px) {
            h1 { font-size: 2.2rem; }
            p { font-size: 1.1rem; }
            a.button { font-size: 1.1rem; padding: 12px 40px; }
            .icon { width: 30px; }
        }
    </style>
</head>
<body>

    <!-- Sfondo -->
    <div class="background"></div>

    <!-- Overlay con contenuto -->
    <div class="overlay">
        <h1>Calcio Performance</h1>
        <p>
            Migliora le tue prestazioni calcistiche con strategie, allenamenti e risorse avanzate.  
            Unisciti a noi per portare il tuo gioco al livello successivo!
        </p>

        <a href="https://www.example.com" class="button">
            Vai alla pagina
        </a>
    </div>

    <!-- Palloni da calcio animati -->
    <div class="icons">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/soccer-ball.png" class="icon" style="left:10%; animation-duration: 12s;">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/soccer-ball.png" class="icon" style="left:30%; animation-duration: 15s;">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/soccer-ball.png" class="icon" style="left:50%; animation-duration: 18s;">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/soccer-ball.png" class="icon" style="left:70%; animation-duration: 14s;">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/soccer-ball.png" class="icon" style="left:90%; animation-duration: 16s;">
    </div>

</body>
</html>
