<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Landing Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            color: #fff;
            overflow: hidden;
        }

        h1 {
            margin-top: 20px;
            font-size: 3em;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            width: 80%;
            margin-top: 20px;
        }

        .character {
            background: #fff;
            border-radius: 10px;
            padding: 10px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.2s;
        }

        .character img {
            width: 100%;
            height: auto;
            border-radius: 10px;
        }

        .character:hover {
            transform: scale(1.05);
        }

        .buttons {
            display: flex;
            justify-content: space-around;
            margin-top: 10px;
        }

        .love, .hate {
            background: #ff9a9e;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            color: #fff;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
        }

        .love:hover {
            background: #ff6a6a;
        }

        .hate:hover {
            background: #c0392b;
        }

        .share {
            margin-top: 30px;
        }

        .share button {
            background: #6a82fb;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            color: #fff;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
        }

        .share button:hover {
            background: #4a69bd;
        }

        .explosion {
            animation: explode 0.5s forwards;
        }

        @keyframes explode {
            0% {
                transform: scale(1);
                opacity: 1;
            }
            100% {
                transform: scale(2);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <h1>Tap to Share Love or Hate!</h1>
    <div class="grid">
        <!-- Example Character -->
        <div class="character">
            <img src="https://via.placeholder.com/150" alt="Character">
            <div class="buttons">
                <button class="love" onclick="loveAction(this)">Love ❤️</button>
                <button class="hate" onclick="hateAction(this)">Hate 💔</button>
            </div>
        </div>
        <!-- Add more characters as needed -->
    </div>
    <div class="share">
        <button>Share Your Reaction</button>
    </div>

    <script>
        function loveAction(button) {
            alert("You loved this character! They thank you with a smile!");
            // Implement AI video popup or message
        }

        function hateAction(button) {
            const character = button.closest('.character');
            character.classList.add('explosion');
            setTimeout(() => character.remove(), 500); // Remove after animation
        }
    </script>
</body>
</html>
