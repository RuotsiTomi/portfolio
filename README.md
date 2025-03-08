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
        .content.active {
            display: block;
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
        .info-box {
            background: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 10px;
            margin: 20px;
            font-size: 18px;
        }
    </style>
    <script>
        function toggleSection(id) {
            document.querySelectorAll('.content').forEach(el => el.classList.remove('active'));
            var section = document.getElementById(id);
            if (section) {
                section.classList.add('active');
            }
        }
        
        document.addEventListener("DOMContentLoaded", function () {
            document.getElementById('vahvuudet').classList.add('active');
        });
    </script>
</head>
<body>
    <header>
        <h1>Portfolio – Oppimispäiväkirja</h1>
        <div class="info-box">
            <p>Tämä sivusto on luotu vain koulutehtävää varten. Katso oikea portfolio tästä: 
                <a href="https://parempiportfolio.com" target="_blank" style="color: #00aaff;">parempiportfolio.com</a>
            </p>
        </div>
        <img src="WhatsApp-Kuva 2025-01-25 klo 13.37.13_d7cc6feb.jpg" alt="Kuva minusta" class="profile">
    </header>
    
    <nav>
        <a onclick="toggleSection('vahvuudet')">Persoonallisuus ja vahvuudet</a>
        <a onclick="toggleSection('motivaatio')">Motivaatio ja arvot</a>
        <a onclick="toggleSection('unelmatyo')">Unelmatyö</a>
        <a onclick="toggleSection('tyonhaku')">Työllistyminen</a>
        <a onclick="toggleSection('koulutus')">Jatkokoulutus</a>
        <a onclick="toggleSection('kiinnostus')">Kiinnostus</a>
    </nav>
    
    <div class="container active">
        <div class="content active" id="vahvuudet">
            <h2>Persoonallisuus ja vahvuudet</h2>
            <li>✔ Matemaattinen osaaminen – looginen ajattelu ja laskennalliset taidot</li>
                <li>✔ Tarkkaavaisuus – huolellisuus työtehtävissä</li>
                <li>✔ Tehokkuus – kyky saada asiat nopeasti ja laadukkaasti valmiiksi</li>
            </ul>
            <p><strong>Kehityskohteeni:</strong></p>
            <ul>
                <li>✖ Kielellinen osaaminen – haluan kehittää itseäni erityisesti viestinnässä</li>
                <li>✖ Kommunikointi – verkostoituminen ja vuorovaikutus vaativat itseltäni enemmän panostusta</li>
            </ul>
            <p><strong>Ajanhallinta:</strong></p>
            <p>🕒 Olen hyvä aikatauluttamaan työni ja olen aina ajoissa.</p>
        </div>
        <div class="content" id="motivaatio">
            <h2>Motivaatio ja arvot</h2>
            <p>Minua motivoi::</strong></p>
                <li>💰 Hyvä palkka – haluan taloudellista vakautta
                <li>📚 Uuden oppiminen – haluan kehittää itseäni jatkuvasti
                <li>🔄 Palaute – arvostan selkeää palautetta kehittyäkseni
                <li>🔒 Vakaus – arvostan varmaa ja pitkäjänteistä työuraa
                <li>Tärkeimmät arvoni:
                <li>✅ Rehellisyys – pyrin aina toimimaan avoimesti ja oikeudenmukaisesti
                <li>✅ Oikeudenmukaisuus – pidän tärkeänä, että jokainen saa ansaitsemansa kohtelun
</p>
        </div>
        <div class="content" id="unelmatyo">
            <h2>Unelmatyö</h2>
            <p>Haluaisin työskennellä kehittämässä uutta teknologiaa, joka vie maailmaa eteenpäin. Samalla haluan ansaita hyvin ja kehittyä asiantuntijana.
                <li>Työympäristöni:
                    <li>🔹 Pidän sekä selkeistä ohjeista että vapaudesta kehittää ratkaisuja
                    <li>🔹 Sopii parhaiten muuttuva ja monipuolinen ympäristö
                <li>🌟 Esikuvani alalla: Elon Musk – innovatiivinen ajattelija, joka vie teknologiaa rohkeasti eteenpäin.
</p>
        </div>
        <div class="content" id="tyonhaku">
            <h2>Työllistyminen</h2>
            <p>Työllistymisen kehittäminen ja työnhaku
            <li>Haluan jatkuvasti kehittää omaa osaamistani ja oppia lisää. Tiedostan, että verkostoitumi-nen on tärkeää urakehityksen kannalta, mutta se on minulle luontaisesti haastavampaa.
                <li>Käyttämäni työnhakukanavat:
                    <li>•	🔗 LinkedIn – aktiivinen profiili ja verkostoituminen
                    <li>•	🏢 Academic Work – nykyinen työpaikkani
                    <li>•	📑 Yritysten omat rekrytointikanavat – tärkeä tapa löytää uusia mahdollisuuksia
                <li>👥 Tärkeimmät verkostot: opiskelijakaverit ja nykyiset kollegat
</p>
        </div>
        <div class="content" id="koulutus">
            <h2>Jatkokoulutus</h2>
            <p>🎓 Minulla on jo kaasualan, öljyalan ja lämmityslaiteasentajan sähköpätevyydet, mutta haluan kehittää osaamistani edelleen.
                <li>🔹 Tavoitteeni: 
                    <li>✅ Opiskella itseni diplomi-insinööriksi insinööriopintojen jälkeen
                    <li>✅ Hankkia lisää sertifikaatteja alani erikoisosaamisalueilta
                    <li>✅ Oppia uusia teknologioita, jotka tukevat uratavoitteitani
</p>
        </div>
        <div class="content" id="kiinnostus">
            <h2>Kiinnostus</h2>
            <p>Olen erittäin kiinnostunut tekoälyn hyödyntämisestä tulevaisuudessa ja siksi yrittänyt saa-da siitä mahdollisimman paljon oppia ja hyötyä koulutuksessa, sekä työelämässä. 
Sijoittaminen on toinen intohimoni ja tavoitteeni on olla taloudellisesti riippumaton ennen, kun täytän 40 ja tähän suunnitelmaan uskon sijoittamisen olevan parasvaihtoehto, tai ai-nakin tällä hetkellä.
</p>
        </div>
    </div>
    
    <footer>
        <p>&copy; 2024 Portfolio. Kaikki oikeudet pidätetään.</p>
        <p>📧 Ota yhteyttä: <a href="mailto:tomi_r@hotmail.com" style="color: #00aaff;">tomi_r@hotmail.com</a></p>
    </footer>
</body>
</html>
