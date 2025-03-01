<!DOCTYPE html>
<!-- saved from url=(0044)https://carnifexe.github.io/bussgeldrechner/ -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">


    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta name="google" content="notranslate">
    <title>SAHP Bußgeldrechner</title>
    <script src="./Bußgeldrechner_files/index.js.Download"></script>
    <link rel="stylesheet" href="./Bußgeldrechner_files/fonts.css">
    <link rel="stylesheet" href="./Bußgeldrechner_files/style.css">
    <link rel="stylesheet" href="./Bußgeldrechner_files/style_sahp_overwrite.html">
    <link rel="icon" type="x-icon" href="https://carnifexe.github.io/bussgeldrechner/DOJ_logo.png">
    <meta content="Bußgeldrechner DE 01" property="og:title">
    <meta content="Bußgeldrechner für GrandRP DE 01 &lt;br&gt; Weitergeführt von Maik Bosa für das SAHP" property="og:description">
    <meta content="https://carnifexe.github.io/bussgeldrechner/" property="og:url">
	<meta property="og:image" content="https://carnifexe.github.io/bussgeldrechner/DOJ_logo.png">
    <meta content="#65d3ff" data-react-helmet="true" name="theme-color">
    <link rel="stylesheet" href="./Bußgeldrechner_files/pro.min.css">
    <link rel="stylesheet" href="./Bußgeldrechner_files/notifications.css">
    <script src="./Bußgeldrechner_files/notifications.js.Download"></script>
	    <style>
        /* CSS für das Video */
        #video_container {
            text-align: center; /* Zentriert das Video */
            margin: 10px 0; /* Fügt oben und unten einen Abstand hinzu */
        }
        #disclaimer_video {
            width: 80%; /* Setzt die Breite des Videos auf 80% */
            max-width: 600px; /* Maximale Breite für große Bildschirme */
        }
        #doj_link {
            text-align: center; /* Zentriert den Link */
            margin: 10px 0; /* Fügt oben und unten einen Abstand hinzu */
        }
        #doj_logo {
            width: 30%; /* Setzt die Breite des DOJ-Logos auf 30% */
            max-width: 150px; /* Maximale Breite für das Logo */
        }
        /* Style für das Notizfeld und den Lösch-Button */
/* Style für das Notizfeld und die Buttons */
#notepadArea {
    position: relative;
    margin-bottom: 10px; /* Abstand zum nächsten Element */
}

#notepadArea_input {
    width: 300px; /* Feste Breite für die Textarea */
    height: 100px; /* Feste Höhe für die Textarea */
    resize: none; /* Verhindert, dass der Benutzer die Größe ändern kann */
}
#clearButton {
    cursor: pointer;
    color: red; /* Textfarbe für den Löschen-Button */
    font-weight: bold;
    position: relative;
    right: 20px; /* Abstand vom rechten Rand der Textarea */
    top: -90px; /* Abstand vom oberen Rand der Textarea */
    background: none;
    border: none;
    font-size: 16px;
    z-index: 1; /* Stellt sicher, dass der Button über der Textarea liegt */
}
/* Stil für die Benachrichtigung */
#notification {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #f44336;
    color: white;
    padding: 15px 30px;
    border-radius: 5px;
    font-size: 16px;
    display: none; /* Standardmäßig unsichtbar */
    z-index: 9999; /* Damit es oben auf allen anderen Elementen liegt */
    opacity: 0; /* Startet unsichtbar */
    transition: opacity 0.5s ease-in-out; /* Sanfte Einblendung */
}

    </style>
<script>
document.addEventListener('contextmenu',function(e){e.preventDefault();e.stopPropagation();});
//document.addEventListener('copy',function(e){e.preventDefault();e.stopPropagation();});
//document.addEventListener('cut',function(e){e.preventDefault();e.stopPropagation();});
</script>
<style>
.jw-album-image img, .jw-element-image img { pointer-events: none; -webkit-touch-callout: none; }
.pswp__share-tooltip .pswp__share--download { display: none; }
</style>
</head>
<body>
        <div id="disclaimerBackgroundBlocker" style="display: none;"></div>
	<div id="disclaimer" style="opacity: 1; box-shadow: rgba(0, 0, 0, 0.22) 0px 0px 70px 30vw; display: none;">
		<div id="disclaimer_title">
			<i id="disclaimer_title_warning" class="fa-regular fa-triangle-exclamation" style="color: rgb(255, 255, 255);"></i> Disclaimer
		</div>
		<br>
		<div id="disclaimer_text">
			Dieser Bußgeldrechner wird von Maik Bosa und Moritz Yane weitergeführt. <br>Wir übernehmen keine Haftung für falsch ausgestellte Akten!
			<br><br>
			<span id="countdown_text">Der Button wird in <span id="countdown">1</span> Sekunden automatisch gedrückt.</span>
			<br>
			<br>
		</div>
            <div id="video_container">
                <video id="disclaimer_video" controls="" autoplay="" muted="">
                    <source src="SAHP_2.mp4" type="video/mp4"> <!-- Hier den Pfad zu deinem Video angeben -->
                    Ihr Browser unterstützt das Video-Tag.
                </video>
            </div>
<script language="JavaScript" src="./Bußgeldrechner_files/counter.js.php"></script><div style="display: inline-block;*display: inline;zoom: 1;font-family: Helvetica, Verdana, Arial, Sans Serif;font-weight: normal;font-size: 12px; color: #666; padding: 3px;text-align: center;border: 1pt solid #eee;-webkit-border-radius: 5px 5px 5px 5px;border-radius: 5px 5px 5px 5px;"><b>2.742 Besucher</b> seit <b>02.02.2025</b></div><br><br>
            <table>
                <tbody><tr id="StandDate">
                    <th style="width: 15%;">Der Bußgeldrechner wurde zuletzt am 07.02.2025 aktualisiert.</th>
                </tr>
			</tbody></table>
		<br>
		<button id="disclaimer_button" onclick="JavaScript:disclaimerAccepted()">Verstanden</button>
		<button id="discord_button" onclick="window.open(&#39;https://discord.gg/ebshMAD3FF&#39;)">Bewerber Discord</button>
	</div>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            let countdownValue = 15; // Startwert des Countdowns in Sekunden
            let countdownInterval; // Intervall für den Countdown

            // Funktion zum Aktualisieren des Countdowns <br><i>Gilt nicht für Cannabis</i>
            function updateCountdown() {
                if (countdownValue > 0) {
                    document.getElementById("countdown").textContent = countdownValue; // Countdown-Text aktualisieren
                    countdownValue--;
                } else {
                    disclaimerAccepted(); // Button automatisch klicken
                    clearInterval(countdownInterval); // Countdown stoppen
                }
            }

            // Countdown-Intervall alle 1 Sekunde starten
            countdownInterval = setInterval(updateCountdown, 1000);

            // Funktion, die beim Klick auf "Verstanden" ausgeführt wird
            window.disclaimerAccepted = function() {
                if (document.getElementById("disclaimer")) { // Überprüfen, ob das Element noch existiert
                    document.getElementById("disclaimer").style.display = "none"; // Disclaimer verstecken
                    document.getElementById("disclaimerBackgroundBlocker").style.display = "none"; // Hintergrundblocker verstecken
                }
            };
        });
    </script>
    <div id="header">

        <div id="credits">
		Weitergeführt von Maik Bosa und Moritz Yane vom SAHP
		</div>
        <div id="sahp">San Andreas Highway Patrol</div>
        <div id="searchbar"><input id="searchbar_input" oninput="JavaScript:searchFine()" type="text" placeholder="Nach einer Straftat suchen"></div>
    </div>

	<div id="contentbox">


<audio id="clickSound" src="KlickSound.mp3"></audio>
        <div id="fineslist">
            <div id="notification"></div><table>
                <tbody><tr id="finesHeader">
                    <th style="width: 15%;">Paragraph</th>
                    <th style="width: 55%;">Strafbestand</th>
                    <th style="width: 15%;">Haftstrafe</th>  
                    <th style="width: 15%;">Bußgeld</th>
                </tr>
<!-- Benachrichtigungs-Box -->


                <tr class="categoryHeader">
                    <th></th>
                    <th>Straßenverkehrsordnung (StVO)</th>
                </tr>
				<tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §2</td>
                    <td class="fineText">Gefährdung anderer Verkehrsteilnehmer</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §4</td>
                    <td class="fineText">Missachten von Rechtsfahrgebot</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="8000">$8.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §5</td>
                    <td class="fineText">Überschreiten der Fahrzeugkapazitäten</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §6</td>
                    <td class="fineText">Fahren mit demoliertem Fahrzeug</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="2000">$2.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §7</td>
                    <td class="fineText">Fahren ohne Licht (Dunkelheit, Wetterverhältnissen)</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 10 - 20 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 21 - 40 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 41 - 60 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 61 - 100 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung ab 101 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §9 Art. 3</td>
                    <td class="fineText">Fahren ohne gültige Zulassung</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 1</td>
                    <td class="fineText">Missachten von Rechts vor Links</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="1000">$1.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 2</td>
                    <td class="fineText">Missachten von Verkehrsschildern</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="2000">$2.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 4</td>
                    <td class="fineText">Fahren ohne genügend Tankkapazität</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 6</td>
                    <td class="fineText">Nutzung eines Mobilgeräts am Steuer</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="3000">$3.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 7</td>
                    <td class="fineText">Lärmbelästigung / Unnötiges Hupen</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 9(1)</td>
                    <td class="fineText">Überholen auf der rechten Fahrbahn</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 12</td>
                    <td class="fineText">Fahren abseits von gekennzeichneten Wegen</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="8000">$8.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 16</td>
                    <td class="fineText">Fahren auf der entgengesetzten Fahrtrichtung</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §12.1</td>
                    <td class="fineText">Falsch Parken / Halten</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §12.3</td>
                    <td class="fineText">Bergung aus nicht befahrbarem Gelände<br><i>Bergung aus schwer zugänglichem Gelände, wie zum Beispiel Gebirge, Strand oder Wasser.</i></td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §17 Art. 1+2</td>
                    <td class="fineText">Fahren im berauschten Zustand</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §19</td>
                    <td class="fineText">Fahren ohne Erste-Hilfe-Kit (Kofferrraum)</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §20</td>
                    <td class="fineText">Fahren ohne Gurt (nicht angeschnallt)</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
              <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §24</td>
                    <td class="fineText">Fahrerflucht / Entziehung einer Verkehrskontrolle</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §24</td>
                    <td class="fineText">Fahrerflucht / Entziehung einer Verkehrskontrolle mit integriertem Anti Radar / Flucht mit integriertem Anti Radar</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <!-- <tr class="showing fine" onclick="(function() { document.getElementById('clickSound').play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §28</td>
                    <td class="fineText">Sharing-Cars mit Anti-Radar wurde nicht aus dem Verkehr gezogen</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr> -->
                <tr class="categoryHeader">
                    <th></th>
                    <th>Psychische &amp; Physische Integrität (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §3.1</td>
                    <td class="fineText">Beleidigung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §3.2</td>
                    <td class="fineText">Belästigung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §3.3</td>
                    <td class="fineText">Öffentliche Defamierung / Mobbing</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.1</td>
                    <td class="fineText">Versuchter Mord / Mord</td>
                    <td class="wantedAmount" data-wantedamount="4">⭐⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.2</td>
                    <td class="fineText">Körperverletzung</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.3</td>
                    <td class="fineText">Körperverletzung mit Todesfolge</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.4</td>
                    <td class="fineText">Gewaltsame Drohung</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.5</td>
                    <td class="fineText">Fahrlässige Tötung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §5</td>
                    <td class="fineText">Sexuelle Belästigung</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §20</td>
                    <td class="fineText">Sachbeschädigung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 + $5.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §21</td>
                    <td class="fineText">Unterlassene Hilfeleistung</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §26</td>
                    <td class="fineText">Prostitution</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §27</td>
                    <td class="fineText">Freiheitsberaubung / Geiselnahmen / Entführung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §28</td>
                    <td class="fineText">Errichtung von Straßenbarrikaden</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000 + $10.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §31</td>
                    <td class="fineText">Verhalten in der Öffentlichkeit</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §32</td>
                    <td class="fineText">Rassismus / Nachstellung (Stalking)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §38</td>
                    <td class="fineText">Fischwilderei</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §39</td>
                    <td class="fineText">Verleumdung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §42</td>
                    <td class="fineText">Erpressung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="45000">$45.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §43</td>
                    <td class="fineText">Androhung einer Straftat</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000 + pro ⭐ $5.000 </td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Wirtschaftskriminalität (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §6 / §9</td>
                    <td class="fineText">Diebstahl / Betrug</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 + $5.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §7</td>
                    <td class="fineText">Fahrzeug Diebstahl</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §10.1</td>
                    <td class="fineText">Besitz illegaler Gegenstände</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §11</td>
                    <td class="fineText">Raub</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
				<tr class="showing fine" data-fine="ammuRob" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
					<td class="paragraph">StGB §12.1</td>
					<td class="fineText">Geschäfts Raub / Ammu Rob (Deckt alle Strafen ab)</td>
					<td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
					<td class="fineAmount" data-fineamount="25000">$25.000</td>
				</tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §12.3</td>
                    <td class="fineText">ATM Raub</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §13</td>
                    <td class="fineText">Einbruch</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §14</td>
                    <td class="fineText">Steuerhinterziehung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §30</td>
                    <td class="fineText">Hausfriedensbruch</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §41.1</td>
                    <td class="fineText">Besitz staatliches Eigentum (Waffen)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §41.2</td>
                    <td class="fineText">Besitz staatliches Eigentum (Gegenstände)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Umgang mit Beamten (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.1</td>
                    <td class="fineText">Nichtbeachten einer amtlichen Anweisung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.2</td>
                    <td class="fineText">Entziehung polizeilicher Maßnahmen</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.3</td>
                    <td class="fineText">Behinderung eines Beamten bei der Arbeit</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.5</td>
                    <td class="fineText">Bestechung von Beamten</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.6</td>
                    <td class="fineText">Widerstand gegen Vollstreckungsbeamte</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.7</td>
                    <td class="fineText">Nicht ausweisen bei einer polizeilichen / Medizinischen Maßnahme</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §16</td>
                    <td class="fineText">Befreiung von Gefangenen</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §19</td>
                    <td class="fineText">Falsche Namensangabe</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §23</td>
                    <td class="fineText">Missbrauch von Notruf</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §24</td>
                    <td class="fineText">Amtsanmaßung</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §29</td>
                    <td class="fineText">Missachtung eines Platzverweises</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Waffengesetz (WaffG)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">WaffG §1</td>
                    <td class="fineText">Besitz legaler Waffen ohne Waffenschein</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §5.1</td>
                    <td class="fineText">Besitz illegaler Waffen </td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §8.1</td>
                    <td class="fineText">Offenes Tragen einer Waffe</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 + $5.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §8.2</td>
                    <td class="fineText">Tragen einer Waffe in staatl. Einrichtungen</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §11</td>
                    <td class="fineText">Ungesetzlicher Waffenhandel (An- &amp; Verkauf)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Sperrzonen / Absperrungen / Kapitalverbrechen (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §17</td>
                    <td class="fineText">Durchbrechen von Absperrungen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18</td>
                    <td class="fineText">Unerlaubtes Betreten von Sperrzonen</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18</td>
                    <td class="fineText">Unerlaubtes Betreten eines millitärischen Geländes</td>
                    <td class="wantedAmount" data-wantedamount="5">⭐⭐⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18.1</td>
                    <td class="fineText">Unerlaubtes Betreten von Militärischen-Sperrzone</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18.1</td>
                    <td class="fineText">Unerlaubtes Befahren von Sperrzonen</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" data-fine="terror" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §25</td>
                    <td class="fineText">Terrorismus (Deckt alle Strafen ab)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Betäubungsmittelgesetz (BtMG)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz (Kokain) Klein ab 11 - 30</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz (Marihuana) Klein ab 21 - 30</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz Mittel ab 31 - 50</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz Groß 50+</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenhandel (An- &amp; Verkauf)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogen Herstellung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §3</td>
                    <td class="fineText">Verkauf von Medizinprodukten bis 20 Medizinischen Gegenständen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §3</td>
                    <td class="fineText">Verkauf von Medizinprodukten bis 50 Medizinischen Gegenständen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §3</td>
                    <td class="fineText">Verkauf von Medizinprodukten ab 51 Medizinischen Gegenständen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Beamtendienstgesetzbuch (Nicht für den Streifendienst) (BDG)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §2</td>
                    <td class="fineText">Verhaltenskodex</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §3</td>
                    <td class="fineText">Dienstpflichten des Beamten</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §7</td>
                    <td class="fineText">Bestechung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §8</td>
                    <td class="fineText">Vorteilsnahme &amp; Vorteilsgewährung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §9</td>
                    <td class="fineText">Verleitung eines Untergebenen/Kollegen zur Straftat</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §10</td>
                    <td class="fineText">Unterlassen der Diensthandlung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §11</td>
                    <td class="fineText">Falschbeurkundung im Amt</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §40</td>
                    <td class="fineText">Weitergabe von Staatseigentum</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §44</td>
                    <td class="fineText">Urkundenfälschung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §13</td>
                    <td class="fineText">Hochverrat im öffentlichen Dienst</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §14</td>
                    <td class="fineText">Umgehung von Strafprozessen</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §15</td>
                    <td class="fineText">Verschwörung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §16</td>
                    <td class="fineText">Schmuggel</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Strafprozessordnung (StPO)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StPO §6</td>
                    <td class="fineText">Bußgelder nicht bezahlt (500k voll)</td>
                    <td class="wantedAmount" data-wantedamount="5">⭐⭐⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="0"></td>
                </tr>
            </tbody></table>
        </div>
        <div id="results">
            <div id="resultsTitle">Ergebnis</div>
            <div id="infoTitle">Bei den grauen Wanteds ist dem Officer das Strafmaß Freigestellt. Durch anklicken können diese ausgewählt werden. Bei gelben Wanteds ist dieses Festgelegt<b></b></div><b>
            <hr color="#121212">
            <div class="result" id="fineResult"><b>Geldstrafe:</b> <font style="user-select: all;">$0</font></div>
            <div class="result" id="wantedsResult"><b>Wanteds:</b> <font style="user-select: all;">0</font></div>
            <div class="result" id="reasonResult"><b>Grund:</b> <font style="user-select: all;" onclick="JavaScript:copyText(event)"></font></div>
            <div class="result" id="charactersResult"><b>Zeichen:</b> 0/150</div>
            <div class="result" id="infoResult"><b>Information:</b> </div>

            <div id="checkbox">
                <input id="checkbox_box" onchange="JavaScript:startCalculating()" type="checkbox" name="" checked="">
                <label style="line-height: 25px;" for="checkbox_box">Kurzer Grund</label>
            </div>

            <div id="plateInput"><input id="plateInput_input" type="text" maxlength="8" placeholder="Kennzeichen" oninput="JavaScript:startCalculating()"></div>
            <div id="blitzerInput"><input id="blitzerInput_input" type="text" maxlength="64" placeholder="Blitzerort" oninput="JavaScript:startCalculating()"></div>
            <div id="systemwantedsInput"><input id="systemwantedsInput_input" type="text" maxlength="1" placeholder="Systemwanteds" oninput="JavaScript:startCalculating()"></div>
            
            <div id="übergabeInput">
                <select name="" id="übergabeInput_select" onchange="JavaScript:startCalculating()">
                    <option value="none">TV-Abtransport auswählen</option>
                    <option value="lspd">Los Santos Police Department</option>
                    <option value="sahp">San Andreas Highway Patrol</option>
                    <option value="ng">National Guard</option>
                    <option value="usss">United States Secret Service</option>
                    <option value="fib">Federal Investigation Bureau</option>
                    <option value="gov">Goverment</option>
                </select>
                    <input id="übergabeInput_input" type="text" oninput="JavaScript:startCalculating()" placeholder="TV-Abtransport Beauftrager" maxlength="64">
                </div>
				<div id="notepadArea" contenteditable="false">
						<textarea id="notepadArea_input" placeholder="Schreibe deine Notizen hier..." rows="3"></textarea>
						<button id="clearButton" contenteditable="false" onclick="clearNotepad()">x</button> <!-- Löschen-Button hinzufügen -->
				</div>
                <div id="reue">
                    <input id="reue_box" onchange="JavaScript:startCalculating()" type="checkbox" name="">
                    <label for="reue_box">
                        <font id="checkboxfont1" style="line-height: 25px;">Reue</font>
                        <br>
                        <font style="font-size: 15px; font-weight: 400;">(Entfernt 2 Wanteds, 1 Wanted muss verbleiben gemäß StBG §35 - Reue)</font>
                    </label>
                </div>
                <div id="systemfehler">
                    <input id="systemfehler_box" onchange="JavaScript:startCalculating()" type="checkbox" name="">
                    <label style="line-height: 25px;" for="systemfehler_box">Systemfehler</label>
                </div>
                <button id="showAttorneysButton" onclick="JavaScript:showAttorneys()">Anwaltsregister anzeigen</button>
                <button id="showRightsButton" onclick="showRightsContainer()">Rechte Anzeigen</button>
                <button id="resetButton" onclick="JavaScript:resetButton()">Zurücksetzen</button>

    <!-- Logo Container -->
	                <table id="finTable">
                    <tbody><tr>
                        <th style="width: 80%;">	<div id="logoContainer" style="text-align: center; margin-top: 20px; margin-left: -120px;">
							<img src="./Bußgeldrechner_files/logosahp.png" alt="Logo" id="logo" style="width: 22%; height: auto;"></div></th>

                    </tr>
                </tbody></table>
            </b></div><b>
            <div id="finesListContainer" style="pointer-events: none;">
                <div id="finesListContainer_title">Auflistung der zu vergebenen Geldstrafen</div>
                <table id="finesListTable"><tbody><tr>
                    <th style="width: 80%;">Grund für die Geldstrafe</th>
                    <th style="width: 20%;">Bußgeld</th>
                </tr></tbody></table>
            </div>

<!-- Hintergrund für Modal -->
<div id="rightsContainer_backdrop" onclick="hideRightsContainer()"></div>

<!-- Modal für Rechte -->
<div id="rightsContainer">
    <div id="rightsContainer_title">
        <span>Rechte Anzeigen</span>
        <button id="rightsContainer_close" onclick="hideRightsContainer()">✖</button>
    </div>
    
    <div id="rightsContainer_content">
        <h2>Die Rechte des TVs:</h2>
        <p>Sie haben das Recht zu schweigen, alles was Sie sagen, kann gegen Sie verwendet werden.<br> 
           Ab 3 Wanteds haben Sie das Recht auf einen Anwalt, den Sie selbst benennen müssen. <br>
           Wenn kein Anwalt verfügbar ist, wird Ihnen keiner gestellt. <br>
           Die Judikative übernimmt der Exekutivbeamte.</p>
        <p>Haben Sie Ihre Rechte verstanden?</p>
    
        <h2>Wenn ein Anwalt gewünscht:</h2>
        <p>Wenn ein Anwalt hinzugezogen wird, kann es länger als 25 Minuten dauern. <br>
           Haben Sie dies verstanden?</p>
    </div>
</div>     
            <div id="attorneyContainer_backdrop" onclick="hideAttorneys()"></div>
            <div id="attorneyContainer" style="opacity: 0; pointer-events: none;">
                <div id="attorneyContainer_title">
                    Anwaltsregister
                    <button id="attorneyContainer_close" onclick="hideAttorneys()">✖</button>
                </div>
                <div id="attorneyContainer_iframe">
                    <iframe src="./Bußgeldrechner_files/pubhtml.html"></iframe>

                </div>
            </div>
    

            
           <div id="standartNotifications">
        </div>
    </b></div><b>
    <button class="help-button" onclick="window.open(&#39;https://github.com/Carnifexe/Carnifexe.github.io/blob/main/README.md&#39;)">
        ?<span> Lizenzvereinbarung</span>
    </button>
    


</b></body></html><!DOCTYPE html>
<!-- saved from url=(0044)https://carnifexe.github.io/bussgeldrechner/ -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">


    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta name="google" content="notranslate">
    <title>SAHP Bußgeldrechner</title>
    <script src="./Bußgeldrechner_files/index.js.Download"></script>
    <link rel="stylesheet" href="./Bußgeldrechner_files/fonts.css">
    <link rel="stylesheet" href="./Bußgeldrechner_files/style.css">
    <link rel="stylesheet" href="./Bußgeldrechner_files/style_sahp_overwrite.html">
    <link rel="icon" type="x-icon" href="https://carnifexe.github.io/bussgeldrechner/DOJ_logo.png">
    <meta content="Bußgeldrechner DE 01" property="og:title">
    <meta content="Bußgeldrechner für GrandRP DE 01 &lt;br&gt; Weitergeführt von Maik Bosa für das SAHP" property="og:description">
    <meta content="https://carnifexe.github.io/bussgeldrechner/" property="og:url">
	<meta property="og:image" content="https://carnifexe.github.io/bussgeldrechner/DOJ_logo.png">
    <meta content="#65d3ff" data-react-helmet="true" name="theme-color">
    <link rel="stylesheet" href="./Bußgeldrechner_files/pro.min.css">
    <link rel="stylesheet" href="./Bußgeldrechner_files/notifications.css">
    <script src="./Bußgeldrechner_files/notifications.js.Download"></script>
	    <style>
        /* CSS für das Video */
        #video_container {
            text-align: center; /* Zentriert das Video */
            margin: 10px 0; /* Fügt oben und unten einen Abstand hinzu */
        }
        #disclaimer_video {
            width: 80%; /* Setzt die Breite des Videos auf 80% */
            max-width: 600px; /* Maximale Breite für große Bildschirme */
        }
        #doj_link {
            text-align: center; /* Zentriert den Link */
            margin: 10px 0; /* Fügt oben und unten einen Abstand hinzu */
        }
        #doj_logo {
            width: 30%; /* Setzt die Breite des DOJ-Logos auf 30% */
            max-width: 150px; /* Maximale Breite für das Logo */
        }
        /* Style für das Notizfeld und den Lösch-Button */
/* Style für das Notizfeld und die Buttons */
#notepadArea {
    position: relative;
    margin-bottom: 10px; /* Abstand zum nächsten Element */
}

#notepadArea_input {
    width: 300px; /* Feste Breite für die Textarea */
    height: 100px; /* Feste Höhe für die Textarea */
    resize: none; /* Verhindert, dass der Benutzer die Größe ändern kann */
}
#clearButton {
    cursor: pointer;
    color: red; /* Textfarbe für den Löschen-Button */
    font-weight: bold;
    position: relative;
    right: 20px; /* Abstand vom rechten Rand der Textarea */
    top: -90px; /* Abstand vom oberen Rand der Textarea */
    background: none;
    border: none;
    font-size: 16px;
    z-index: 1; /* Stellt sicher, dass der Button über der Textarea liegt */
}
/* Stil für die Benachrichtigung */
#notification {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #f44336;
    color: white;
    padding: 15px 30px;
    border-radius: 5px;
    font-size: 16px;
    display: none; /* Standardmäßig unsichtbar */
    z-index: 9999; /* Damit es oben auf allen anderen Elementen liegt */
    opacity: 0; /* Startet unsichtbar */
    transition: opacity 0.5s ease-in-out; /* Sanfte Einblendung */
}

    </style>
<script>
document.addEventListener('contextmenu',function(e){e.preventDefault();e.stopPropagation();});
//document.addEventListener('copy',function(e){e.preventDefault();e.stopPropagation();});
//document.addEventListener('cut',function(e){e.preventDefault();e.stopPropagation();});
</script>
<style>
.jw-album-image img, .jw-element-image img { pointer-events: none; -webkit-touch-callout: none; }
.pswp__share-tooltip .pswp__share--download { display: none; }
</style>
</head>
<body>
        <div id="disclaimerBackgroundBlocker" style="display: none;"></div>
	<div id="disclaimer" style="opacity: 1; box-shadow: rgba(0, 0, 0, 0.22) 0px 0px 70px 30vw; display: none;">
		<div id="disclaimer_title">
			<i id="disclaimer_title_warning" class="fa-regular fa-triangle-exclamation" style="color: rgb(255, 255, 255);"></i> Disclaimer
		</div>
		<br>
		<div id="disclaimer_text">
			Dieser Bußgeldrechner wird von Maik Bosa und Moritz Yane weitergeführt. <br>Wir übernehmen keine Haftung für falsch ausgestellte Akten!
			<br><br>
			<span id="countdown_text">Der Button wird in <span id="countdown">1</span> Sekunden automatisch gedrückt.</span>
			<br>
			<br>
		</div>
            <div id="video_container">
                <video id="disclaimer_video" controls="" autoplay="" muted="">
                    <source src="SAHP_2.mp4" type="video/mp4"> <!-- Hier den Pfad zu deinem Video angeben -->
                    Ihr Browser unterstützt das Video-Tag.
                </video>
            </div>
<script language="JavaScript" src="./Bußgeldrechner_files/counter.js.php"></script><div style="display: inline-block;*display: inline;zoom: 1;font-family: Helvetica, Verdana, Arial, Sans Serif;font-weight: normal;font-size: 12px; color: #666; padding: 3px;text-align: center;border: 1pt solid #eee;-webkit-border-radius: 5px 5px 5px 5px;border-radius: 5px 5px 5px 5px;"><b>2.742 Besucher</b> seit <b>02.02.2025</b></div><br><br>
            <table>
                <tbody><tr id="StandDate">
                    <th style="width: 15%;">Der Bußgeldrechner wurde zuletzt am 07.02.2025 aktualisiert.</th>
                </tr>
			</tbody></table>
		<br>
		<button id="disclaimer_button" onclick="JavaScript:disclaimerAccepted()">Verstanden</button>
		<button id="discord_button" onclick="window.open(&#39;https://discord.gg/ebshMAD3FF&#39;)">Bewerber Discord</button>
	</div>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            let countdownValue = 15; // Startwert des Countdowns in Sekunden
            let countdownInterval; // Intervall für den Countdown

            // Funktion zum Aktualisieren des Countdowns <br><i>Gilt nicht für Cannabis</i>
            function updateCountdown() {
                if (countdownValue > 0) {
                    document.getElementById("countdown").textContent = countdownValue; // Countdown-Text aktualisieren
                    countdownValue--;
                } else {
                    disclaimerAccepted(); // Button automatisch klicken
                    clearInterval(countdownInterval); // Countdown stoppen
                }
            }

            // Countdown-Intervall alle 1 Sekunde starten
            countdownInterval = setInterval(updateCountdown, 1000);

            // Funktion, die beim Klick auf "Verstanden" ausgeführt wird
            window.disclaimerAccepted = function() {
                if (document.getElementById("disclaimer")) { // Überprüfen, ob das Element noch existiert
                    document.getElementById("disclaimer").style.display = "none"; // Disclaimer verstecken
                    document.getElementById("disclaimerBackgroundBlocker").style.display = "none"; // Hintergrundblocker verstecken
                }
            };
        });
    </script>
    <div id="header">

        <div id="credits">
		Weitergeführt von Maik Bosa und Moritz Yane vom SAHP
		</div>
        <div id="sahp">San Andreas Highway Patrol</div>
        <div id="searchbar"><input id="searchbar_input" oninput="JavaScript:searchFine()" type="text" placeholder="Nach einer Straftat suchen"></div>
    </div>

	<div id="contentbox">


<audio id="clickSound" src="KlickSound.mp3"></audio>
        <div id="fineslist">
            <div id="notification"></div><table>
                <tbody><tr id="finesHeader">
                    <th style="width: 15%;">Paragraph</th>
                    <th style="width: 55%;">Strafbestand</th>
                    <th style="width: 15%;">Haftstrafe</th>  
                    <th style="width: 15%;">Bußgeld</th>
                </tr>
<!-- Benachrichtigungs-Box -->


                <tr class="categoryHeader">
                    <th></th>
                    <th>Straßenverkehrsordnung (StVO)</th>
                </tr>
				<tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §2</td>
                    <td class="fineText">Gefährdung anderer Verkehrsteilnehmer</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §4</td>
                    <td class="fineText">Missachten von Rechtsfahrgebot</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="8000">$8.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §5</td>
                    <td class="fineText">Überschreiten der Fahrzeugkapazitäten</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §6</td>
                    <td class="fineText">Fahren mit demoliertem Fahrzeug</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="2000">$2.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §7</td>
                    <td class="fineText">Fahren ohne Licht (Dunkelheit, Wetterverhältnissen)</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 10 - 20 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 21 - 40 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 41 - 60 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung 61 - 100 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §8</td>
                    <td class="fineText">Geschwindigkeitsüberschreitung ab 101 km/h</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §9 Art. 3</td>
                    <td class="fineText">Fahren ohne gültige Zulassung</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 1</td>
                    <td class="fineText">Missachten von Rechts vor Links</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="1000">$1.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 2</td>
                    <td class="fineText">Missachten von Verkehrsschildern</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="2000">$2.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 4</td>
                    <td class="fineText">Fahren ohne genügend Tankkapazität</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 6</td>
                    <td class="fineText">Nutzung eines Mobilgeräts am Steuer</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="3000">$3.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 7</td>
                    <td class="fineText">Lärmbelästigung / Unnötiges Hupen</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 9(1)</td>
                    <td class="fineText">Überholen auf der rechten Fahrbahn</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 12</td>
                    <td class="fineText">Fahren abseits von gekennzeichneten Wegen</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="8000">$8.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §10 Art. 16</td>
                    <td class="fineText">Fahren auf der entgengesetzten Fahrtrichtung</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §12.1</td>
                    <td class="fineText">Falsch Parken / Halten</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine addPlateInList" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §12.3</td>
                    <td class="fineText">Bergung aus nicht befahrbarem Gelände<br><i>Bergung aus schwer zugänglichem Gelände, wie zum Beispiel Gebirge, Strand oder Wasser.</i></td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §17 Art. 1+2</td>
                    <td class="fineText">Fahren im berauschten Zustand</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §19</td>
                    <td class="fineText">Fahren ohne Erste-Hilfe-Kit (Kofferrraum)</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §20</td>
                    <td class="fineText">Fahren ohne Gurt (nicht angeschnallt)</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
              <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §24</td>
                    <td class="fineText">Fahrerflucht / Entziehung einer Verkehrskontrolle</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §24</td>
                    <td class="fineText">Fahrerflucht / Entziehung einer Verkehrskontrolle mit integriertem Anti Radar / Flucht mit integriertem Anti Radar</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <!-- <tr class="showing fine" onclick="(function() { document.getElementById('clickSound').play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StVO §28</td>
                    <td class="fineText">Sharing-Cars mit Anti-Radar wurde nicht aus dem Verkehr gezogen</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr> -->
                <tr class="categoryHeader">
                    <th></th>
                    <th>Psychische &amp; Physische Integrität (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §3.1</td>
                    <td class="fineText">Beleidigung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §3.2</td>
                    <td class="fineText">Belästigung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §3.3</td>
                    <td class="fineText">Öffentliche Defamierung / Mobbing</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.1</td>
                    <td class="fineText">Versuchter Mord / Mord</td>
                    <td class="wantedAmount" data-wantedamount="4">⭐⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.2</td>
                    <td class="fineText">Körperverletzung</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.3</td>
                    <td class="fineText">Körperverletzung mit Todesfolge</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.4</td>
                    <td class="fineText">Gewaltsame Drohung</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §4.5</td>
                    <td class="fineText">Fahrlässige Tötung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §5</td>
                    <td class="fineText">Sexuelle Belästigung</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §20</td>
                    <td class="fineText">Sachbeschädigung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 + $5.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §21</td>
                    <td class="fineText">Unterlassene Hilfeleistung</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §26</td>
                    <td class="fineText">Prostitution</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §27</td>
                    <td class="fineText">Freiheitsberaubung / Geiselnahmen / Entführung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §28</td>
                    <td class="fineText">Errichtung von Straßenbarrikaden</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000 + $10.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §31</td>
                    <td class="fineText">Verhalten in der Öffentlichkeit</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §32</td>
                    <td class="fineText">Rassismus / Nachstellung (Stalking)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §38</td>
                    <td class="fineText">Fischwilderei</td>
                    <td class="wantedAmount" data-wantedamount="0"></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §39</td>
                    <td class="fineText">Verleumdung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §42</td>
                    <td class="fineText">Erpressung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="45000">$45.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §43</td>
                    <td class="fineText">Androhung einer Straftat</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000 + pro ⭐ $5.000 </td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Wirtschaftskriminalität (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §6 / §9</td>
                    <td class="fineText">Diebstahl / Betrug</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 + $5.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §7</td>
                    <td class="fineText">Fahrzeug Diebstahl</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §10.1</td>
                    <td class="fineText">Besitz illegaler Gegenstände</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §11</td>
                    <td class="fineText">Raub</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
				<tr class="showing fine" data-fine="ammuRob" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
					<td class="paragraph">StGB §12.1</td>
					<td class="fineText">Geschäfts Raub / Ammu Rob (Deckt alle Strafen ab)</td>
					<td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
					<td class="fineAmount" data-fineamount="25000">$25.000</td>
				</tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §12.3</td>
                    <td class="fineText">ATM Raub</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §13</td>
                    <td class="fineText">Einbruch</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §14</td>
                    <td class="fineText">Steuerhinterziehung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §30</td>
                    <td class="fineText">Hausfriedensbruch</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §41.1</td>
                    <td class="fineText">Besitz staatliches Eigentum (Waffen)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §41.2</td>
                    <td class="fineText">Besitz staatliches Eigentum (Gegenstände)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Umgang mit Beamten (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.1</td>
                    <td class="fineText">Nichtbeachten einer amtlichen Anweisung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.2</td>
                    <td class="fineText">Entziehung polizeilicher Maßnahmen</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.3</td>
                    <td class="fineText">Behinderung eines Beamten bei der Arbeit</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.5</td>
                    <td class="fineText">Bestechung von Beamten</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.6</td>
                    <td class="fineText">Widerstand gegen Vollstreckungsbeamte</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §15.7</td>
                    <td class="fineText">Nicht ausweisen bei einer polizeilichen / Medizinischen Maßnahme</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §16</td>
                    <td class="fineText">Befreiung von Gefangenen</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §19</td>
                    <td class="fineText">Falsche Namensangabe</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §23</td>
                    <td class="fineText">Missbrauch von Notruf</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §24</td>
                    <td class="fineText">Amtsanmaßung</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §29</td>
                    <td class="fineText">Missachtung eines Platzverweises</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Waffengesetz (WaffG)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">WaffG §1</td>
                    <td class="fineText">Besitz legaler Waffen ohne Waffenschein</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="10000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §5.1</td>
                    <td class="fineText">Besitz illegaler Waffen </td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$10.000 pro ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §8.1</td>
                    <td class="fineText">Offenes Tragen einer Waffe</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="5000">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000 + $5.000 pro weiteren ⭐</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §8.2</td>
                    <td class="fineText">Tragen einer Waffe in staatl. Einrichtungen</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="5000">$5.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="true">
                    <td class="paragraph">WaffG §11</td>
                    <td class="fineText">Ungesetzlicher Waffenhandel (An- &amp; Verkauf)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Sperrzonen / Absperrungen / Kapitalverbrechen (StGB)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §17</td>
                    <td class="fineText">Durchbrechen von Absperrungen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18</td>
                    <td class="fineText">Unerlaubtes Betreten von Sperrzonen</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18</td>
                    <td class="fineText">Unerlaubtes Betreten eines millitärischen Geländes</td>
                    <td class="wantedAmount" data-wantedamount="5">⭐⭐⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="50000">$50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18.1</td>
                    <td class="fineText">Unerlaubtes Betreten von Militärischen-Sperrzone</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="true" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §18.1</td>
                    <td class="fineText">Unerlaubtes Befahren von Sperrzonen</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="showing fine" data-fine="terror" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §25</td>
                    <td class="fineText">Terrorismus (Deckt alle Strafen ab)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Betäubungsmittelgesetz (BtMG)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz (Kokain) Klein ab 11 - 30</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz (Marihuana) Klein ab 21 - 30</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="15000">$15.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz Mittel ab 31 - 50</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenbesitz Groß 50+</td>
                    <td class="wantedAmount" data-wantedamount="2">⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogenhandel (An- &amp; Verkauf)</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §2.1</td>
                    <td class="fineText">Drogen Herstellung</td>
                    <td class="wantedAmount" data-wantedamount="3">⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="30000">$30.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §3</td>
                    <td class="fineText">Verkauf von Medizinprodukten bis 20 Medizinischen Gegenständen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐</td>
                    <td class="fineAmount" data-fineamount="10000">$10.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §3</td>
                    <td class="fineText">Verkauf von Medizinprodukten bis 50 Medizinischen Gegenständen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="20000">$20.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BtMG §3</td>
                    <td class="fineText">Verkauf von Medizinprodukten ab 51 Medizinischen Gegenständen</td>
                    <td class="wantedAmount" data-wantedamount="1">⭐<font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="0">☆</font></td>
                    <td class="fineAmount" data-fineamount="25000">$25.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Beamtendienstgesetzbuch (Nicht für den Streifendienst) (BDG)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §2</td>
                    <td class="fineText">Verhaltenskodex</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §3</td>
                    <td class="fineText">Dienstpflichten des Beamten</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §7</td>
                    <td class="fineText">Bestechung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §8</td>
                    <td class="fineText">Vorteilsnahme &amp; Vorteilsgewährung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §9</td>
                    <td class="fineText">Verleitung eines Untergebenen/Kollegen zur Straftat</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §10</td>
                    <td class="fineText">Unterlassen der Diensthandlung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §11</td>
                    <td class="fineText">Falschbeurkundung im Amt</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StGB §40</td>
                    <td class="fineText">Weitergabe von Staatseigentum</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();">
                    <td class="paragraph">StGB §44</td>
                    <td class="fineText">Urkundenfälschung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §13</td>
                    <td class="fineText">Hochverrat im öffentlichen Dienst</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §14</td>
                    <td class="fineText">Umgehung von Strafprozessen</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §15</td>
                    <td class="fineText">Verschwörung</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">BDG §16</td>
                    <td class="fineText">Schmuggel</td>
                    <td class="wantedAmount" data-wantedamount="0"><font class="extrawanted1 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted2 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted3 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted4 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font><font class="extrawanted5 extrawanted" onclick="JavaScript:toggleExtraWanted(event)" data-addedfine="10000">☆</font></td>
                    <td class="fineAmount" data-fineamount="0">max. $50.000</td>
                </tr>
                <tr class="categoryHeader">
                    <th></th>
                    <th>Strafprozessordnung (StPO)</th>
                </tr>
                <tr class="showing fine" onclick="(function() { document.getElementById(&#39;clickSound&#39;).play(); selectFine(event); })();" data-removedriverlicence="false" data-removeweaponlicence="false">
                    <td class="paragraph">StPO §6</td>
                    <td class="fineText">Bußgelder nicht bezahlt (500k voll)</td>
                    <td class="wantedAmount" data-wantedamount="5">⭐⭐⭐⭐⭐</td>
                    <td class="fineAmount" data-fineamount="0"></td>
                </tr>
            </tbody></table>
        </div>
        <div id="results">
            <div id="resultsTitle">Ergebnis</div>
            <div id="infoTitle">Bei den grauen Wanteds ist dem Officer das Strafmaß Freigestellt. Durch anklicken können diese ausgewählt werden. Bei gelben Wanteds ist dieses Festgelegt<b></b></div><b>
            <hr color="#121212">
            <div class="result" id="fineResult"><b>Geldstrafe:</b> <font style="user-select: all;">$0</font></div>
            <div class="result" id="wantedsResult"><b>Wanteds:</b> <font style="user-select: all;">0</font></div>
            <div class="result" id="reasonResult"><b>Grund:</b> <font style="user-select: all;" onclick="JavaScript:copyText(event)"></font></div>
            <div class="result" id="charactersResult"><b>Zeichen:</b> 0/150</div>
            <div class="result" id="infoResult"><b>Information:</b> </div>

            <div id="checkbox">
                <input id="checkbox_box" onchange="JavaScript:startCalculating()" type="checkbox" name="" checked="">
                <label style="line-height: 25px;" for="checkbox_box">Kurzer Grund</label>
            </div>

            <div id="plateInput"><input id="plateInput_input" type="text" maxlength="8" placeholder="Kennzeichen" oninput="JavaScript:startCalculating()"></div>
            <div id="blitzerInput"><input id="blitzerInput_input" type="text" maxlength="64" placeholder="Blitzerort" oninput="JavaScript:startCalculating()"></div>
            <div id="systemwantedsInput"><input id="systemwantedsInput_input" type="text" maxlength="1" placeholder="Systemwanteds" oninput="JavaScript:startCalculating()"></div>
            
            <div id="übergabeInput">
                <select name="" id="übergabeInput_select" onchange="JavaScript:startCalculating()">
                    <option value="none">TV-Abtransport auswählen</option>
                    <option value="lspd">Los Santos Police Department</option>
                    <option value="sahp">San Andreas Highway Patrol</option>
                    <option value="ng">National Guard</option>
                    <option value="usss">United States Secret Service</option>
                    <option value="fib">Federal Investigation Bureau</option>
                    <option value="gov">Goverment</option>
                </select>
                    <input id="übergabeInput_input" type="text" oninput="JavaScript:startCalculating()" placeholder="TV-Abtransport Beauftrager" maxlength="64">
                </div>
				<div id="notepadArea" contenteditable="false">
						<textarea id="notepadArea_input" placeholder="Schreibe deine Notizen hier..." rows="3"></textarea>
						<button id="clearButton" contenteditable="false" onclick="clearNotepad()">x</button> <!-- Löschen-Button hinzufügen -->
				</div>
                <div id="reue">
                    <input id="reue_box" onchange="JavaScript:startCalculating()" type="checkbox" name="">
                    <label for="reue_box">
                        <font id="checkboxfont1" style="line-height: 25px;">Reue</font>
                        <br>
                        <font style="font-size: 15px; font-weight: 400;">(Entfernt 2 Wanteds, 1 Wanted muss verbleiben gemäß StBG §35 - Reue)</font>
                    </label>
                </div>
                <div id="systemfehler">
                    <input id="systemfehler_box" onchange="JavaScript:startCalculating()" type="checkbox" name="">
                    <label style="line-height: 25px;" for="systemfehler_box">Systemfehler</label>
                </div>
                <button id="showAttorneysButton" onclick="JavaScript:showAttorneys()">Anwaltsregister anzeigen</button>
                <button id="showRightsButton" onclick="showRightsContainer()">Rechte Anzeigen</button>
                <button id="resetButton" onclick="JavaScript:resetButton()">Zurücksetzen</button>

    <!-- Logo Container -->
	                <table id="finTable">
                    <tbody><tr>
                        <th style="width: 80%;">	<div id="logoContainer" style="text-align: center; margin-top: 20px; margin-left: -120px;">
							<img src="./Bußgeldrechner_files/logosahp.png" alt="Logo" id="logo" style="width: 22%; height: auto;"></div></th>

                    </tr>
                </tbody></table>
            </b></div><b>
            <div id="finesListContainer" style="pointer-events: none;">
                <div id="finesListContainer_title">Auflistung der zu vergebenen Geldstrafen</div>
                <table id="finesListTable"><tbody><tr>
                    <th style="width: 80%;">Grund für die Geldstrafe</th>
                    <th style="width: 20%;">Bußgeld</th>
                </tr></tbody></table>
            </div>

<!-- Hintergrund für Modal -->
<div id="rightsContainer_backdrop" onclick="hideRightsContainer()"></div>

<!-- Modal für Rechte -->
<div id="rightsContainer">
    <div id="rightsContainer_title">
        <span>Rechte Anzeigen</span>
        <button id="rightsContainer_close" onclick="hideRightsContainer()">✖</button>
    </div>
    
    <div id="rightsContainer_content">
        <h2>Die Rechte des TVs:</h2>
        <p>Sie haben das Recht zu schweigen, alles was Sie sagen, kann gegen Sie verwendet werden.<br> 
           Ab 3 Wanteds haben Sie das Recht auf einen Anwalt, den Sie selbst benennen müssen. <br>
           Wenn kein Anwalt verfügbar ist, wird Ihnen keiner gestellt. <br>
           Die Judikative übernimmt der Exekutivbeamte.</p>
        <p>Haben Sie Ihre Rechte verstanden?</p>
    
        <h2>Wenn ein Anwalt gewünscht:</h2>
        <p>Wenn ein Anwalt hinzugezogen wird, kann es länger als 25 Minuten dauern. <br>
           Haben Sie dies verstanden?</p>
    </div>
</div>     
            <div id="attorneyContainer_backdrop" onclick="hideAttorneys()"></div>
            <div id="attorneyContainer" style="opacity: 0; pointer-events: none;">
                <div id="attorneyContainer_title">
                    Anwaltsregister
                    <button id="attorneyContainer_close" onclick="hideAttorneys()">✖</button>
                </div>
                <div id="attorneyContainer_iframe">
                    <iframe src="./Bußgeldrechner_files/pubhtml.html"></iframe>

                </div>
            </div>
    

            
           <div id="standartNotifications">
        </div>
    </b></div><b>
    <button class="help-button" onclick="window.open(&#39;https://github.com/Carnifexe/Carnifexe.github.io/blob/main/README.md&#39;)">
        ?<span> Lizenzvereinbarung</span>
    </button>
    


</b></body></html>
