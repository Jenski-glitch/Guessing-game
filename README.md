<!DOCTYPE html>
<html>
<head>
    <title>Jen's Quiz Adventure ✨🧠🌍</title>
    <meta charset="UTF-8">
    <style>
        body {
            font-family: 'Segoe UI', sans-serif;
            background-color: #ffeef2; /* light pastel pink */
            color: #444;
            text-align: center;
            padding: 40px;
        }

        h1 {
            color: #c77dff;
            font-size: 32px;
        }

        #question {
            font-size: 20px;
            margin-bottom: 20px;
        }

        .btn {
            padding: 10px 25px;
            margin: 10px;
            border: none;
            border-radius: 12px;
            background-color: #ffd6e0;
            color: #333;
            font-size: 16px;
            cursor: pointer;
            transition: 0.3s;
        }

        .btn:hover {
            background-color: #ffb3c6;
        }

        #result {
            font-weight: bold;
            font-size: 18px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <h1>Jen's Quiz Adventure ✨🧠🌍</h1>
    <p id="question">Math 🧮: What is 325 + 178?</p>

    <button class="btn" onclick="checkAnswer(503)">503</button>
    <button class="btn" onclick="checkAnswer(502)">502</button>
    <button class="btn" onclick="checkAnswer(504)">504</button>

    <p id="result"></p>

    <script>
        function checkAnswer(choice) {
            const correct = 503;
            const result = document.getElementById("result");

            if (choice === correct) {
                result.textContent = "✅ Correct! Great job!";
                result.style.color = "green";
            } else {
                result.textContent = "❌ Oops! Try again.";
                result.style.color = "red";
            }
        }
    </script>

</body>
</html>
