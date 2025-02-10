<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eu Te Amo</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #ffe6e6;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .message {
            font-size: 24px;
            color: #d9534f;
            margin-bottom: 20px;
        }
        .heart {
            position: relative;
            width: 60px; /* Diminuído o tamanho */
            height: 60px; /* Diminuído o tamanho */
            background-color: red;
            transform: rotate(-45deg);
            margin: 0 auto;
            animation: pulse 1s infinite;
        }
        .heart::before,
        .heart::after {
            content: "";
            position: absolute;
            width: 60px; /* Diminuído o tamanho */
            height: 60px; /* Diminuído o tamanho */
            background-color: red;
            border-radius: 50%;
        }
        .heart::before {
            top: -30px; /* Ajustado para o novo tamanho */
            left: 0;
        }
        .heart::after {
            left: 30px; /* Ajustado para o novo tamanho */
            top: 0;
        }
        .name {
            font-size: 18px;
            color: #d9534f;
            margin-top: 10px;
        }
        @keyframes pulse {
            0%, 100% {
                transform: scale(1) rotate(-45deg);
            }
            50% {
                transform: scale(1.1) rotate(-45deg);
            }
        }
    </style>
</head>
<body>
    <div>
        <div class="message">Eu te amo</div>
        <div class="heart"></div>
        <div class="name">Elane</div>
    </div>
</body>
</html>
