<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>La Social-Démocratie Scandinave</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #f4f4f4; }
        h1 { color: #2C3E50; }
        .container { width: 80%; margin: auto; padding: 20px; background: white; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
        .button { background: #3498DB; color: white; padding: 10px 20px; border: none; cursor: pointer; margin-top: 10px; }
        .quiz { display: none; padding: 10px; text-align: left; }
        .map { width: 100%; max-width: 600px; margin-top: 20px; }
    </style>
</head>
<body>

    <div class="container">
        <h1>La Social-Démocratie Scandinave</h1>
        <p>Un modèle politique et social basé sur la démocratie et la protection sociale.</p>
        
        <button class="button" onclick="showSection('chiffres')">📊 Voir les chiffres clés</button>
        <button class="button" onclick="showSection('quiz')">🧠 Tester ses connaissances</button>

        <div id="chiffres" class="quiz">
            <h2>Les démocraties scandinaves en chiffres</h2>
            <p>Les pays nordiques sont classés parmi les **démocraties les plus avancées du monde**.</p>
            <img class="map" src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7c/Democracy_Index_2020.png/800px-Democracy_Index_2020.png" alt="Carte des démocraties">
        </div>

        <div id="quiz" class="quiz">
            <h2>Quiz sur la Social-Démocratie Scandinave</h2>
            <p>1. Quel pays ne fait pas partie des démocraties scandinaves ?</p>
            <button class="button" onclick="checkAnswer(1, 'A')">A) Allemagne</button>
            <button class="button" onclick="checkAnswer(1, 'B')">B) Norvège</button>
            <p id="result1"></p>

            <p>2. Quels sont les piliers du modèle scandinave ?</p>
            <button class="button" onclick="checkAnswer(2, 'A')">A) Protection sociale et démocratie</button>
            <button class="button" onclick="checkAnswer(2, 'B')">B) Capitalisme sauvage</button>
            <p id="result2"></p>
        </div>
    </div>

    <script>
        function showSection(id) {
            document.querySelectorAll('.quiz').forEach(div => div.style.display = 'none');
            document.getElementById(id).style.display = 'block';
        }

        function checkAnswer(question, answer) {
            const correctAnswers = { 1: 'A', 2: 'A' };
            let result = document.getElementById('result' + question);
            if (correctAnswers[question] === answer) {
                result.innerHTML = "✅ Bonne réponse !";
                result.style.color = "green";
            } else {
                result.innerHTML = "❌ Mauvaise réponse, essaye encore.";
                result.style.color = "red";
            }
        }
    </script>

</body>
</html>
