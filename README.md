<!DOCTYPE html>
<html lang="fi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio – Oppimispäiväkirja</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: black;
            color: white;
            text-align: center;
            background-image: url('WhatsApp-Kuva 2025-02-24 klo 19.04.12_90626095.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }
        header {
            background-color: rgba(0, 0, 0, 0.8);
            padding: 20px;
        }
        nav {
            padding: 10px;
            background: rgba(34, 34, 34, 0.8);
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
            cursor: pointer;
        }
        .container {
            width: 80%;
            margin: auto;
            padding: 20px;
            background: rgba(51, 51, 51, 0.9);
            box-shadow: 0px 0px 10px rgba(255, 255, 255, 0.1);
            text-align: left;
            border-radius: 10px;
            display: none;
        }
        .container.active {
            display: block;
        }
        h2 {
            color: #00aaff;
            cursor: pointer;
        }
        .content {
            display: none;
            padding: 10px;
        }
        img.profile {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            margin: 20px 0;
            border: 3px solid white;
        }
        footer {
            text-align: center;
            padding: 20px;
            background: rgba(0, 0, 0, 0.8);
            color: white;
            margin-top: 20px;
        }
        .language-selector {
            margin: 10px;
        }
    </style>
    <script>
        function toggleSection(id) {
            var section = document.getElementById(id);
            section.style.display = (section.style.display === "none" || section.style.display === "") ? "block" : "none";
        }
        
        function changeLanguage(lang) {
            document.querySelectorAll('.container').forEach(el => {
                el.classList.remove('active');
                if (el.getAttribute('data-lang') === lang) {
                    el.classList.add('active');
                }
            });
        }
        
        document.addEventListener("DOMContentLoaded", function () {
            changeLanguage('fi');
        });
    </script>
</head>
<body>
    <header>
        <h1>Portfolio – Oppimispäiväkirja</h1>
        <div class="language-selector">
            <button onclick="changeLanguage('fi')">Suomi</button>
            <button onclick="changeLanguage('sv')">Svenska</button>
            <button onclick="changeLanguage('en')">English</button>
        </div>
        <img src="WhatsApp-Kuva 2025-01-25 klo 13.37.13_d7cc6feb.jpg" alt="Kuva minusta" class="profile">
    </header>
    
    <nav>
        <a onclick="toggleSection('vahvuudet')">Persoonallisuus ja vahvuudet</a>
        <a onclick="toggleSection('motivaatio')">Motivaatio ja arvot</a>
        <a onclick="toggleSection('unelmatyo')">Unelmatyö</a>
        <a onclick="toggleSection('tyonhaku')">Työllistyminen</a>
        <a onclick="toggleSection('koulutus')">Jatkokoulutus</a>
        <a onclick="toggleSection('tekoaly')">Kiinnostus tekoälyyn ja sijoittamiseen</a>
    </nav>
    
    <div class="container" data-lang="fi">
        <h2 onclick="toggleSection('vahvuudet')">Persoonallisuus ja vahvuudet</h2>
        <div class="content" id="vahvuudet">
            <p>Olen määrätietoinen ja analyyttinen henkilö, jolla on vahva oikeudentaju...</p>
        </div>
    </div>
    
    <div class="container" data-lang="sv">
        <h2 onclick="toggleSection('vahvuudet_sv')">Personlighet och styrkor</h2>
        <div class="content" id="vahvuudet_sv">
            <p>Jag är en målmedveten och analytisk person med stark känsla för rättvisa...</p>
        </div>
    </div>
    
    <div class="container" data-lang="en">
        <h2 onclick="toggleSection('vahvuudet_en')">Personality and Strengths</h2>
        <div class="content" id="vahvuudet_en">
            <p>I am a determined and analytical person with a strong sense of justice...</p>
        </div>
    </div>
    
    <footer>
        <p>&copy; 2024 Portfolio. Kaikki oikeudet pidätetään.</p>
        <p>📧 Ota yhteyttä: <a href="mailto:tomi_r@hotmail.com" style="color: #00aaff;">tomi_r@hotmail.com</a></p>
    </footer>
</body>
</html>
