
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
        }
        header {
            background-color: #111;
            padding: 20px;
        }
        nav {
            padding: 10px;
            background: #222;
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
            background: #333;
            box-shadow: 0px 0px 10px rgba(255, 255, 255, 0.1);
            text-align: left;
            border-radius: 10px;
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
        img.background {
            width: 100%;
            height: auto;
            margin-bottom: 20px;
        }
        footer {
            text-align: center;
            padding: 20px;
            background: #111;
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
            document.querySelectorAll('[data-lang]').forEach(el => {
                el.style.display = el.getAttribute('data-lang') === lang ? 'block' : 'none';
            });
        }
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
        <img src="profile.jpg" alt="WhatsApp-Kuva 2025-01-25 klo 13.37.13_d7cc6feb.jpg" class="profile">
    </header>
    
    <nav>
        <a onclick="toggleSection('vahvuudet')">Persoonallisuus ja vahvuudet</a>
        <a onclick="toggleSection('motivaatio')">Motivaatio ja arvot</a>
        <a onclick="toggleSection('unelmatyo')">Unelmatyö</a>
        <a onclick="toggleSection('tyonhaku')">Työllistyminen</a>
        <a onclick="toggleSection('koulutus')">Jatkokoulutus</a>
        <a onclick="toggleSection('tekoaly')">Kiinnostus tekoälyyn ja sijoittamiseen</a>
    </nav>
    
    <img src="background.jpg" alt="Visuaalinen taustakuva" class="background">
    
    <div class="container" data-lang="fi">
        <h2 onclick="toggleSection('vahvuudet')">Persoonallisuus ja vahvuudet</h2>
        <div class="content" id="vahvuudet">
            <p>Olen määrätietoinen ja analyyttinen henkilö, jolla on vahva oikeudentaju...</p>
        </div>
    </div>
    
    <footer>
        <p>&copy; 2024 Portfolio. Kaikki oikeudet pidätetään.</p>
        <p>📧 Ota yhteyttä: <a href="mailto:tomi_r@hotmail.com" style="color: #00aaff;">tomi_r@hotmail.com</a></p>
    </footer>
</body>
</html>
