<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parcours Genially - Social-Démocratie Scandinave</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #f4f4f4; padding: 30px; }
        .slide { display: none; padding: 20px; background: white; box-shadow: 0 4px 8px rgba(0,0,0,0.1); border-radius: 10px; max-width: 800px; margin: auto; }
        .active { display: block; }
        img { max-width: 100%; height: auto; border-radius: 10px; }
        button { margin: 15px; padding: 10px 20px; font-size: 16px; border: none; background: #007bff; color: white; border-radius: 5px; cursor: pointer; }
        button:hover { background: #0056b3; }
        .progress-bar { width: 100%; background: #ddd; height: 10px; margin-top: 20px; }
        .progress { height: 10px; background: #007bff; width: 0%; }
        .quiz { margin-top: 20px; display: none; }
        .menu { margin-bottom: 20px; }
    </style>
</head>
<body>
    <h1>Parcours Interactif : Social-Démocratie Scandinave</h1>
    
    <div class="menu">
        <button onclick="goToSlide(0)">Introduction</button>
        <button onclick="goToSlide(1)">Principes Clés</button>
        <button onclick="goToSlide(2)">Pays Modèles</button>
        <button onclick="goToSlide(3)">Défis</button>
        <button onclick="goToSlide(4)">Quiz</button>
    </div>

    <div class="progress-bar"><div class="progress" id="progress-bar"></div></div>

    <div id="slides">

    <div class="slide" id="slide0" class="active">
        <h2>Introduction à la Social-Démocratie Scandinave</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Nordic_Countries_%28orthographic_projection%29.svg/800px-Nordic_Countries_%28orthographic_projection%29.svg.png" alt="Introduction à la Social-Démocratie Scandinave">
        <p>La social-démocratie scandinave repose sur un modèle politique unique, combinant démocratie, État-providence et économie de marché.</p>
        <button onclick="prevSlide()" style="display:none;">Précédent</button>
        <button onclick="nextSlide()" >Suivant</button>
    </div>
    
    <div class="slide" id="slide1" >
        <h2>Les Principes Clés</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/67/Welfare_state.svg/512px-Welfare_state.svg.png" alt="Les Principes Clés">
        <p>1. Fortes politiques de protection sociale
2. Fiscalité élevée mais redistributive
3. Services publics gratuits et accessibles à tous</p>
        <button onclick="prevSlide()" >Précédent</button>
        <button onclick="nextSlide()" >Suivant</button>
    </div>
    
    <div class="slide" id="slide2" >
        <h2>Les Pays Modèles</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/55/Flag_of_Sweden.svg/512px-Flag_of_Sweden.svg.png" alt="Les Pays Modèles">
        <p>Les pays nordiques (Suède, Norvège, Danemark, Finlande, Islande) appliquent ce modèle avec succès, garantissant une égalité économique et sociale.</p>
        <button onclick="prevSlide()" >Précédent</button>
        <button onclick="nextSlide()" >Suivant</button>
    </div>
    
    <div class="slide" id="slide3" >
        <h2>Les Défis</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d1/Old_people_in_Spain_2011.jpg/800px-Old_people_in_Spain_2011.jpg" alt="Les Défis">
        <p>Bien que performant, ce modèle doit s'adapter aux défis modernes : vieillissement de la population, immigration et mondialisation.</p>
        <button onclick="prevSlide()" >Précédent</button>
        <button onclick="nextSlide()" >Suivant</button>
    </div>
    
    <div class="slide" id="slide4" >
        <h2>Quiz : Testez vos connaissances !</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Question_mark.svg/512px-Question_mark.svg.png" alt="Quiz : Testez vos connaissances !">
        <p></p>
        <button onclick="prevSlide()" >Précédent</button>
        <button onclick="nextSlide()" style="display:none;">Suivant</button>
    </div>
    
    <div class="slide quiz" id="slide4">
        <h2>Quiz : Testez vos connaissances !</h2>
        <p>Quel pays n'est PAS considéré comme un modèle de social-démocratie scandinave ?</p>
        <button onclick="checkAnswer('A')">A. Suède</button>
        <button onclick="checkAnswer('B')">B. Norvège</button>
        <button onclick="checkAnswer('C')">C. États-Unis</button>
        <p id="quiz-result"></p>
    </div>
    </div>

    <script>
        let currentSlide = 0;
        const slides = document.querySelectorAll(".slide");
        const progressBar = document.getElementById("progress-bar");

        function showSlide(index) {
            slides.forEach((slide, i) => {
                slide.style.display = i === index ? "block" : "none";
            });
            progressBar.style.width = ((index + 1) / slides.length) * 100 + "%";
        }

        function nextSlide() {
            if (currentSlide < slides.length - 1) {
                currentSlide++;
                showSlide(currentSlide);
            }
        }

        function prevSlide() {
            if (currentSlide > 0) {
                currentSlide--;
                showSlide(currentSlide);
            }
        }

        function goToSlide(index) {
            currentSlide = index;
            showSlide(currentSlide);
        }

        function checkAnswer(answer) {
            const result = document.getElementById("quiz-result");
            if (answer === "C") {
                result.innerHTML = "Bonne réponse ! Les États-Unis ne sont pas un modèle de social-démocratie.";
                result.style.color = "green";
            } else {
                result.innerHTML = "Mauvaise réponse, essayez encore.";
                result.style.color = "red";
            }
        }
    </script>
</body>
</html>
