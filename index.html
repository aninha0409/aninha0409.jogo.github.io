<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jogo da Velha!</title>
    <style>
        /* Estilos gerais */
        body {
            font-family: 'Comic Sans MS', sans-serif;
            background: linear-gradient(135deg, #fbc2eb, #a6c1ee);
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
        }

        h1 {
            font-size: 32px;
            color: #333;
            margin-bottom: 20px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
        }

        /* Estilo do tabuleiro */
        .board {
            display: grid;
            grid-template-columns: repeat(3, 120px);
            grid-template-rows: repeat(3, 120px);
            gap: 10px;
            justify-content: center;
        }

        .cell {
            width: 120px;
            height: 120px;
            background-color: #fff;
            border: 3px solid #333;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 3em;
            color: #333;
            cursor: pointer;
            border-radius: 10px;
            transition: transform 0.2s ease, background-color 0.3s;
        }

        .cell:hover {
            transform: scale(1.1);
            background-color: #fce0ec;
        }

        .cell.taken {
            pointer-events: none;
        }

        /* Estilo da mensagem */
        .message {
            margin-top: 30px;
            font-size: 24px;
            color: #333;
            font-weight: bold;
            text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.2);
        }

        button {
            background-color: #ff4f70;
            color: white;
            font-size: 20px;
            padding: 10px 20px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            margin-top: 20px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
            transition: background-color 0.3s, transform 0.3s;
        }

        button:hover {
            background-color: #ff647c;
            transform: scale(1.1);
        }

        /* Animações */
        .shake {
            animation: shake 0.5s ease-in-out;
        }

        @keyframes shake {
            0% { transform: translateX(-10px); }
            25% { transform: translateX(10px); }
            50% { transform: translateX(-10px); }
            75% { transform: translateX(10px); }
            100% { transform: translateX(0); }
        }

        /* Responsividade */
        @media (max-width: 600px) {
            .board {
                grid-template-columns: repeat(3, 100px);
                grid-template-rows: repeat(3, 100px);
            }

            .cell {
                font-size: 2em;
            }

            h1 {
                font-size: 26px;
            }
        }
    </style>
</head>
<body>

    <div>
        <h1>Jogo da Velha!</h1>
        <div class="board" id="board">
            <div class="cell" id="cell-0"></div>
            <div class="cell" id="cell-1"></div>
            <div class="cell" id="cell-2"></div>
            <div class="cell" id="cell-3"></div>
            <div class="cell" id="cell-4"></div>
            <div class="cell" id="cell-5"></div>
            <div class="cell" id="cell-6"></div>
            <div class="cell" id="cell-7"></div>
            <div class="cell" id="cell-8"></div>
        </div>
        <div class="message" id="message">Jogador 1 (X) é o primeiro a jogar!</div>
        <button onclick="reiniciarJogo()">Reiniciar Jogo</button>
    </div>

    <script>
        const board = document.getElementById('board');
        const message = document.getElementById('message');
        let currentPlayer = 'X'; // Começa com o jogador X
        let gameBoard = ['', '', '', '', '', '', '', '', '']; // Representação interna do tabuleiro
        let gameOver = false;

        // Função chamada quando uma célula é clicada
        function handleClick(cellId) {
            if (gameBoard[cellId] === '' && !gameOver) {
                // Preenche a célula com o símbolo do jogador atual
                gameBoard[cellId] = currentPlayer;
                document.getElementById(`cell-${cellId}`).textContent = currentPlayer;
                document.getElementById(`cell-${cellId}`).classList.add('taken');
                
                // Verifica se alguém ganhou
                if (verificarVitoria()) {
                    message.textContent = `Jogador ${currentPlayer} ganhou!`;
                    document.querySelectorAll('.cell').forEach(cell => {
                        cell.classList.add('shake');
                    });
                    gameOver = true;
                    return;
                }

                // Alterna para o outro jogador
                currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
                message.textContent = `Agora é a vez do Jogador ${currentPlayer}`;
            }
        }

        // Função que verifica se há vitória
        function verificarVitoria() {
            const vitorias = [
                [0, 1, 2], [3, 4, 5], [6, 7, 8], // linhas
                [0, 3, 6], [1, 4, 7], [2, 5, 8], // colunas
                [0, 4, 8], [2, 4, 6] // diagonais
            ];

            for (let i = 0; i < vitorias.length; i++) {
                const [a, b, c] = vitorias[i];
                if (gameBoard[a] && gameBoard[a] === gameBoard[b] && gameBoard[a] === gameBoard[c]) {
                    return true;
                }
            }
            return false;
        }

        // Função que reinicia o jogo
        function reiniciarJogo() {
            gameBoard = ['', '', '', '', '', '', '', '', ''];
            gameOver = false;
            currentPlayer = 'X';
            message.textContent = 'Jogador 1 (X) é o primeiro a jogar!';

            // Limpar a tela
            const cells = document.querySelectorAll('.cell');
            cells.forEach(cell => {
                cell.textContent = '';
                cell.classList.remove('taken', 'shake');
            });
        }

        // Adiciona os eventos de clique nas células
        document.querySelectorAll('.cell').forEach((cell, index) => {
            cell.addEventListener('click', () => handleClick(index));
        });
    </script>

</body>
</html>
