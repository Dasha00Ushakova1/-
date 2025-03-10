
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ответы на тесты</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }
        header {
            background: #007BFF;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        .content {
            background: white;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .question {
            margin-bottom: 10px;
        }
        .answer {
            display: none;
            margin-top: 5px;
            color: green;
        }
        button {
            margin-top: 5px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Ответы на тесты Google</h1>
    </header>
    <div class="content">
        <div class="question">
            <p>Вопрос 1: Какой язык программирования используется для веб-разработки?</p>
            <button onclick="toggleAnswer('answer1')">Показать ответ</button>
            <p class="answer" id="answer1">Ответ: JavaScript</p>
        </div>
        <div class="question">
            <p>Вопрос 2: Что такое HTML?</p>
            <button onclick="toggleAnswer('answer2')">Показать ответ</button>
            <p class="answer" id="answer2">Ответ: Язык разметки гипертекста</p>
        </div>
        <div class="question">
            <p>Вопрос 3: Что такое CSS?</p>
            <button onclick="toggleAnswer('answer3')">Показать ответ</button>
            <p class="answer" id="answer3">Ответ: Каскадные таблицы стилей</p>
        </div>
    </div>
    <script>
        function toggleAnswer(answerId) {
            const answer = document.getElementById(answerId);
            if (answer.style.display === "none" || answer.style.display === "") {
                answer.style.display = "block";
            } else {
                answer.style.display = "none";
            }
        }
    </script>
</body>
</html>
