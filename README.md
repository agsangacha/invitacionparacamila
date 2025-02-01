<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Invitación de San Valentín</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #000;
            color: #fff;
            text-align: center;
            padding: 50px;
            margin: 0;
            overflow: hidden;
            position: relative;
        }
        h1 {
            color: #ff6f61;
            font-size: 3em;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in-out;
        }
        .dedicatoria {
            font-size: 1.5em;
            color: #ff6f61;
            margin-bottom: 30px;
            animation: fadeIn 2s ease-in-out;
        }
        .buttons {
            margin-top: 20px;
        }
        .button {
            padding: 15px 30px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 50px;
            color: white;
            transition: transform 0.3s ease;
        }
        .button.yes {
            background-color: #ff6f61;
        }
        .button.no {
            background-color: #6b5b95;
            position: relative;
        }
        /* Lunas y corazones de fondo */
        .background {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
        }
        .background span {
            position: absolute;
            display: block;
            font-size: 30px;
            animation: animateBackground 10s linear infinite;
            bottom: -150px;
        }
        @keyframes animateBackground {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-1000px) rotate(720deg);
                opacity: 0;
            }
        }
        /* Animación de flotación */
        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-20px);
            }
        }
        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <div class="background">
        <!-- Lunas y corazones de fondo -->
        <span style="left: 5%; animation-delay: 0s;">🌙</span>
        <span style="left: 15%; animation-delay: 2s;">💖</span>
        <span style="left: 25%; animation-delay: 4s;">🌙</span>
        <span style="left: 35%; animation-delay: 6s;">💖</span>
        <span style="left: 45%; animation-delay: 8s;">🌙</span>
        <span style="left: 55%; animation-delay: 10s;">💖</span>
        <span style="left: 65%; animation-delay: 12s;">🌙</span>
        <span style="left: 75%; animation-delay: 14s;">💖</span>
        <span style="left: 85%; animation-delay: 16s;">🌙</span>
        <span style="left: 95%; animation-delay: 18s;">💖</span>
    </div>
    <div class="dedicatoria">
        <p>Para Camila, mi razón de ser...</p>
        <p>De parte de Angelo, con todo mi amor 💖</p>
    </div>
    <h1>¿Quieres ser mi San Valentín?</h1>
    <div class="buttons">
        <button class="button yes" onclick="abrirMensaje()">Sí</button>
        <button class="button no" onmouseover="moverBoton()">No</button>
    </div>

    <script>
        function moverBoton() {
            const botonNo = document.querySelector('.button.no');
            const x = Math.random() * (window.innerWidth - botonNo.offsetWidth);
            const y = Math.random() * (window.innerHeight - botonNo.offsetHeight);
            botonNo.style.position = 'absolute';
            botonNo.style.left = `${x}px`;
            botonNo.style.top = `${y}px`;
        }

        function abrirMensaje() {
            // Abre una nueva pestaña con el mensaje romántico
            const nuevaPestana = window.open('', '_blank');
            nuevaPestana.document.write(`
                <!DOCTYPE html>
                <html lang="es">
                <head>
                    <meta charset="UTF-8">
                    <meta name="viewport" content="width=device-width, initial-scale=1.0">
                    <title>Mensaje para Camila</title>
                    <style>
                        body {
                            font-family: 'Arial', sans-serif;
                            background-color: #000;
                            color: #fff;
                            text-align: center;
                            padding: 50px;
                            margin: 0;
                            overflow: hidden;
                            position: relative;
                        }
                        h1 {
                            color: #ff6f61;
                            font-size: 3em;
                            margin-bottom: 20px;
                        }
                        .message {
                            font-size: 1.5em;
                            color: #ff6f61;
                            max-width: 600px;
                            margin: 0 auto;
                            animation: fadeIn 2s ease-in-out;
                        }
                        .ositos {
                            margin-top: 20px;
                        }
                        .ositos img {
                            width: 100px;
                            margin: 10px;
                            animation: float 3s infinite ease-in-out;
                        }
                        /* Lunas y corazones de fondo */
                        .background {
                            position: absolute;
                            top: 0;
                            left: 0;
                            width: 100%;
                            height: 100%;
                            overflow: hidden;
                            z-index: -1;
                        }
                        .background span {
                            position: absolute;
                            display: block;
                            font-size: 30px;
                            animation: animateBackground 10s linear infinite;
                            bottom: -150px;
                        }
                        @keyframes animateBackground {
                            0% {
                                transform: translateY(0) rotate(0deg);
                                opacity: 1;
                            }
                            100% {
                                transform: translateY(-1000px) rotate(720deg);
                                opacity: 0;
                            }
                        }
                        @keyframes float {
                            0%, 100% {
                                transform: translateY(0);
                            }
                            50% {
                                transform: translateY(-20px);
                            }
                        }
                        @keyframes fadeIn {
                            0% {
                                opacity: 0;
                            }
                            100% {
                                opacity: 1;
                            }
                        }
                    </style>
                </head>
                <body>
                    <div class="background">
                        <!-- Lunas y corazones de fondo -->
                        <span style="left: 5%; animation-delay: 0s;">🌙</span>
                        <span style="left: 15%; animation-delay: 2s;">💖</span>
                        <span style="left: 25%; animation-delay: 4s;">🌙</span>
                        <span style="left: 35%; animation-delay: 6s;">💖</span>
                        <span style="left: 45%; animation-delay: 8s;">🌙</span>
                        <span style="left: 55%; animation-delay: 10s;">💖</span>
                        <span style="left: 65%; animation-delay: 12s;">🌙</span>
                        <span style="left: 75%; animation-delay: 14s;">💖</span>
                        <span style="left: 85%; animation-delay: 16s;">🌙</span>
                        <span style="left: 95%; animation-delay: 18s;">💖</span>
                    </div>
                    <h1>¡Para Camila! 💖</h1>
                    <div class="message">
                        <p>
                            Aunque la distancia nos haya separado, aunque hayamos estado con otras personas, 
                            aunque el mundo haya intentado alejarnos, siempre supe que eras tú. 
                            Tú eres mi persona favorita, mi complicidad, mi risa y mi paz. 
                            No importa lo que pase, siempre serás mi San Valentín, mi todo. 
                            ¿Qué dices, aceptas ser mía para siempre? 😏💖
                        </p>
                        <div class="ositos">
                            <img src="https://i.imgur.com/1qT8Q.png" alt="Osito 1">
                            <img src="https://i.imgur.com/2qT8Q.png" alt="Osito 2">
                            <img src="https://i.imgur.com/jh_de_la_cruz_meme.jpg" alt="JH de la Cruz" style="border-radius: 50%;">
                        </div>
                    </div>
                </body>
                </html>
            `);
            nuevaPestana.document.close();
        }
    </script>
</body>
</html>
