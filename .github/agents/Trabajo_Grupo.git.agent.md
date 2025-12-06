<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio Web Designer</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
            background: #f2f2f2;
        }

        .container {
            display: flex;
            height: 100vh;
        }

        /* --- Columna izquierda --- */
        .left {
            flex: 1;
            background: #e7eefc; /* azul muy claro */
            padding: 80px 60px;
            display: flex;
            justify-content: center;
            flex-direction: column;
        }

        .left h3 {
            color: #222;
            margin-bottom: 10px;
            font-size: 18px;
        }

        .left h1 {
            font-size: 55px;
            margin: 0 0 20px;
            font-weight: 900;
            line-height: 1.1;
        }

        .left p {
            max-width: 400px;
            font-size: 16px;
            margin-bottom: 35px;
            color: #444;
        }

        .buttons {
            display: flex;
            gap: 20px;
        }

        .btn1, .btn2 {
            padding: 14px 28px;
            border-radius: 30px;
            font-size: 16px;
            cursor: pointer;
            border: 2px solid black;
            transition: 0.3s;
        }

        .btn1 {
            background: black;
            color: white;
        }

        .btn1:hover {
            background: white;
            color: black;
        }

        .btn2 {
            background: white;
            color: black;
        }

        .btn2:hover {
            background: black;
            color: white;
        }

        /* --- Columna derecha (imagen) --- */
        .right {
            flex: 1;
            background: #f7d7f3; /* rosado pastel */
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
        }

        .photo-area {
            width: 400px;
            height: auto;
            position: relative;
        }

        .photo-area img {
            width: 100%;
            border-radius: 10px;
            z-index: 2;
            position: relative;
        }

        /* Figura estilo "burbuja" detrás */
        .bubble {
            background: #8bc3ff;
            width: 430px;
            height: 430px;
            border-radius: 40% 60% 55% 45%;
            position: absolute;
            top: -20px;
            left: -15px;
            z-index: 1;
        }

        /* --- Footer de iconos --- */
        footer {
            padding: 20px;
            display: flex;
            justify-content: center;
            gap: 40px;
            background: white;
            border-top: 1px solid #ccc;
        }

        footer span {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 18px;
        }

        footer span::before {
            content: "•";
            font-size: 25px;
        }
    </style>
</head>

<body>

    <!-- Contenedor principal -->
    <div class="container">

        <!-- Columna izquierda -->
        <div class="left">
            <h3>Welcome 👋</h3>
            <h1>I’m Reachle Green<br>a web designer<br>from New York</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p>

            <div class="buttons">
                <button class="btn1">Contact me</button>
                <button class="btn2">Send me a message</button>
            </div>
        </div>

        <!-- Columna derecha -->
        <div class="right">
            <div class="photo-area">
                <div class="bubble"></div>

                <!-- Imagen (pon la tuya propia aquí) -->
                <img src="tu-imagen.png" alt="Foto persona">
            </div>
        </div>

    </div>

    <!-- Footer -->
    <footer>
        <span>Agency</span>
        <span>Company</span>
        <span>Business</span>
        <span>Startup</span>
        <span>Venture</span>
    </footer>

</body>
</html>