<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flores para ti</title>
    <style>
        body {
            background-color: #000;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .container {
            text-align: center;
        }
        .flowers {
            display: flex;
            flex-direction: column;
            align-items: center;
            animation: bloom 3s ease-in-out infinite alternate;
        }
        .flower {
            width: 100px;
            height: 100px;
            background: radial-gradient(circle at 50% 50%, yellow 50%, transparent 51%);
            border-radius: 50%;
            position: relative;
            margin: 10px;
        }
        .flower::before {
            content: '';
            position: absolute;
            width: 100px;
            height: 100px;
            background: radial-gradient(circle at 50% 50%, yellow 50%, transparent 51%);
            border-radius: 50%;
            top: -50px;
            left: -50px;
        }
        @keyframes bloom {
            from { transform: scale(0.9); }
            to { transform: scale(1.1); }
        }
        h1 {
            color: #fff;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Flores para ti, mi amor</h1>
        <div class="flowers">
            <div class="flower"></div>
            <div class="flower"></div>
            <div class="flower"></div>
        </div>
    </div>
</body>
</html># flores_M
