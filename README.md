- 👋 Hi, I’m @bricenopgn
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
bricenopgn/bricenopgn is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tablero de Ajedrez</title>
    <style>
        /* Estilos para las casillas del tablero */
        .board {
            display: grid;
            grid-template-columns: repeat(8, 50px);
            grid-template-rows: repeat(8, 50px);
        }
        .white {
            background-color: #f0d9b5;
        }
        .black {
            background-color: #b58863;
        }
    </style>
</head>
<body>
    <div class="board" id="chessboard"></div>

    <script>
        // Crear el tablero de ajedrez
        const board = document.getElementById('chessboard');

        for (let row = 0; row < 8; row++) {
            for (let col = 0; col < 8; col++) {
                const square = document.createElement('div');
                square.classList.add((row + col) % 2 === 0 ? 'white' : 'black');
                board.appendChild(square);
            }
        }
    </script>
</body>
</html>
