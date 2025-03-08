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
    </style>
    <script>
        function toggleSection(id) {
            var section = document.getElementById(id);
            section.style.display = (section.style.display === "none" || section.style.display === "") ? "block" : "none";
        }
    </script>
</head>
<body>
    <header>
        <h1>Portfolio – Oppimispäiväkirja</h1>
        <img src="profile.jpg" alt="Kuva minusta" class="profile">
    </header>
    
    <nav>
        <a onclick="toggleSection('vahvuudet')">Persoonallisuus ja vahvuudet</a>
        <a onclick="toggleSection('motivaatio')">Motivaatio ja arvot</a>
        <a onclick="toggleSection('unelmatyo')">Unelmatyö</a>
        <a onclick="toggleSection('tyonhaku')">Työllistyminen</a>
        <a onclick="toggleSection('koulutus')">Jatkokoulutus</a>
    </nav>
    
    <img src="background.jpg" alt="Visuaalinen taustakuva" class="background">
    
    <div class="container">
        <h2 onclick="toggleSection('vahvuudet')">Persoonallisuus ja vahvuudet</h2>
        <div class="content" id="vahvuudet">
            <p>Olen johtajatyyppinen henkilö, jolla on vahva oikeudentaju. Tunnistan itsessäni myös piirteitä kuten täsmällisyys, tehokkuus ja miellyttävyys.</p>
        </div>
        
        <h2 onclick="toggleSection('motivaatio')">Motivaatio ja arvot</h2>
        <div class="content" id="motivaatio">
            <p>Minua motivoi hyvä palkka, uuden oppiminen ja selkeä palaute. Arvojani ovat rehellisyys ja oikeudenmukaisuus.</p>
        </div>
        
        <h2 onclick="toggleSection('unelmatyo')">Unelmatyöni ja työympäristö</h2>
        <div class="content" id="unelmatyo">
            <p>Haluaisin työskennellä kehittämässä uutta teknologiaa, joka vie maailmaa eteenpäin.</p>
        </div>
        
        <h2 onclick="toggleSection('tyonhaku')">Työllistyminen ja työnhaku</h2>
        <div class="content" id="tyonhaku">
            <p>Verkostoituminen on tärkeää, mutta minulle haastavampaa. Käytän LinkedInia ja Academic Workia työnhaussa.</p>
        </div>
        
        <h2 onclick="toggleSection('koulutus')">Jatkokoulutussuunnitelmat</h2>
        <div class="content" id="koulutus">
            <p>Minulla on jo kaasualan ja öljyalan pätevyydet, mutta haluan opiskella diplomi-insinööriksi.</p>
        </div>
    </div>
    
    <footer>
        <p>&copy; 2024 Portfolio. Kaikki oikeudet pidätetään.</p>
    </footer>
</body>
</html>
