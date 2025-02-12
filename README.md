
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Wishes</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            height: 100vh;
            overflow: hidden;
            background: linear-gradient(to right, #ff758c, #ff7eb3);
            font-family: Arial, sans-serif;
            text-align: center;
            color: white;
            position: relative;
        }
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: red;
            clip-path: polygon(50% 15%, 100% 50%, 75% 100%, 50% 75%, 25% 100%, 0% 50%);
            opacity: 0.6;
            animation: float 5s linear infinite;
        }
        @keyframes float {
            0% { transform: translateY(100vh) scale(0.5); opacity: 1; }
            100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
        }
        .container {
            max-width: 600px;
            padding: 20px;
            position: relative;
            z-index: 1;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 15px;
            backdrop-filter: blur(10px);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            margin-bottom: 20px;
            animation: bounce 2s infinite alternate;
        }
        @keyframes bounce {
            0% { transform: translateY(0); }
            100% { transform: translateY(-10px); }
        }
        h1 {
            font-size: 2.5em;
            animation: fadeIn 2s ease-in-out;
        }
        p {
            font-size: 1.2em;
            margin-bottom: 20px;
            animation: fadeIn 3s ease-in-out;
        }
        .btn {
            padding: 10px 20px;
            background-color: white;
            color: #ff758c;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
            transition: 0.3s;
        }
        .btn:hover {
            background-color: #ffebeb;
        }
        .hidden-message {
            display: none;
            font-size: 1.5em;
            margin-top: 20px;
            animation: fadeIn 2s;
            position: relative;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>
    <script>
        function createHearts() {
            for (let i = 0; i < 20; i++) {
                let heart = document.createElement("div");
                heart.classList.add("heart");
                heart.style.left = Math.random() * 100 + "vw";
                heart.style.animationDuration = (Math.random() * 3 + 2) + "s";
                document.body.appendChild(heart);
                setTimeout(() => { heart.remove(); }, 5000);
            }
        }
        setInterval(createHearts, 500);
    </script>
    <div class="container">
        <h1>Happy Valentine's Day! ❤️</h1>
        <p>Una na yapium kai veda matan 😉🫂🥺🥹</p>
        <button class="btn" onclick="showMessage()">Click for a Surprise</button>
        <p class="hidden-message" id="message">
            Happy Valentine's Day de ma papa. ❤️ Love uhhh as always 💋💋🫂🫂.<br>
            Epo tha purithu na una evlo kasta padathunan nu. ❤️<br>
            kandipa mariruvann nambi thola naya. ❤️ na epo nu kuda ella tha but yapium unaku aaga earrapan papa <br>
            na unaku pudikama earakarathu edhuvum pana matan ok va. ❤️<br>
            I miss uhhh so muchhh de papa ma. ❤️ love uhhhhhhh
        </p>
    </div>
    <script>
        function showMessage() {
            document.getElementById("message").style.display = "block";
        }
    </script>
</body>
</html>
