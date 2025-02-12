
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Love Mail Cover</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 100%);
            font-family: 'poppin', bold;
            color: #fff;
            text-align: center;
        }

        .mail-cover {
            position: relative;
            width: 300px;
            height: 200px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            overflow: hidden;
            cursor: pointer;
            transition: transform 0.5s;
        }

        .mail-content {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            box-sizing: border-box;
        }

        .mail-front {
            background: rgba(255, 255, 255, 0.2);
        }

        .mail-back {
            background: rgba(255, 255, 255, 0.9);
            color: #ee0000;
            transform: rotateX(180deg);
        }

        .mail-back h1 {
            font-size: 1.5em;
            margin-bottom: 10px;
        }

        .mail-back p {
            font-size: 1em;
            line-height: 1.5;
        }

        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.4);
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background-color: #fefefe;
            margin: auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 600px;
            border-radius: 10px;
            text-align: center;
            color: #000; /* Change text color to black */
        }

        .modal-content h1 {
            font-size: 1.2em; /* Make the heading smaller */
        }

        .modal-content p {
            font-size: 0.9em; /* Make the paragraph text smaller */
        }

        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }

        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="mail-cover" id="mail-cover">
        <div class="mail-content mail-front">
            <h1>Click Panu de pondati💋💋</h1>
        </div>
    </div>

    <div id="myModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h1>Happy Valentine's Day</h1>
            <p>de ma papa. Love uhhh as always 💋💋🫂🫂. Epo tha purithu na una evlo kasta padathunan nu. kandipa mariruvann nambi thola naya. na epo nu kuda ella tha but yapium unaku aaga earrapan papa na unaku pudikama earakarathu edhuvum pana matan ok va. i miss uhhh so muchhh de papa ma. love uhhhhhhh💋💋</p>
        </div>
    </div>

    <script>
        var modal = document.getElementById("myModal");
        var btn = document.getElementById("mail-cover");
        var span = document.getElementsByClassName("close")[0];

        btn.onclick = function() {
            modal.style.display = "flex";
        }

        span.onclick = function() {
            modal.style.display = "none";
        }

        window.onclick = function(event) {
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
    </script>
</body>
</html>
