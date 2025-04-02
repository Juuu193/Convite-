# Convite-
<!DOCTYPE html><html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Convite Encantado</title>
    <style>
        body {
            background: linear-gradient(to bottom, #2c003e, #6a0572);
            color: #fff;
            font-family: 'Garamond', serif;
            text-align: center;
            padding: 20px;
            overflow: hidden;
        }
        .container {
            max-width: 500px;
            margin: auto;
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(255, 223, 0, 0.8);
        }
        h1 {
            font-size: 28px;
            text-shadow: 0 0 10px gold;
        }
        .lantern {
            position: absolute;
            width: 30px;
            height: 50px;
            background: gold;
            border-radius: 10px;
            opacity: 0.7;
            animation: floatLanterns 5s linear infinite;
        }
        @keyframes floatLanterns {
            from { transform: translateY(100vh); opacity: 0.2; }
            to { transform: translateY(-10vh); opacity: 1; }
        }
        .button {
            background: gold;
            color: #2c003e;
            padding: 10px 20px;
            border-radius: 10px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            margin-top: 15px;
            box-shadow: 0 0 10px gold;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Convite Encantado - Uma Aventura Iluminada!</h1>
        <p>Era uma vez, em um reino encantado, uma celebração mágica estava prestes a acontecer...</p>
        <p><strong>Data:</strong> [Insira a data] <br> <strong>Horário:</strong> [Insira o horário] <br> <strong>Local:</strong> [Insira o local]</p>
        <p>Vista-se como um verdadeiro habitante do reino e embarque nessa história mágica!</p>
        <a href="#" class="button">Confirmar Presença</a>
    </div><script>
    function createLantern() {
        const lantern = document.createElement("div");
        lantern.classList.add("lantern");
        lantern.style.left = Math.random() * window.innerWidth + "px";
        document.body.appendChild(lantern);
        setTimeout(() => lantern.remove(), 5000);
    }
    setInterval(createLantern, 800);
</script>

</body>
</html>
