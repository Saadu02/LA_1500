# Projekt-Dokumentation


## Tower Defence. 
Gruppe Heliotrope
Sathana Suganthasri, Joel Simon Juan. Haldimann und Kilian Adil. Staeuble


| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|23.02.2023| 0.0.1     |Entscheidung getroffen, wie unsere Thema lautet. |
|02.03.2023| 0.0.2  |Kapitel 1 bis 3 abgeschlossen.|
|30.03.2023| 0.0.3  | Projekt fertig erstellt und rest der Kapitel fertig ausgefüllt.|

## 1 Informieren

### 1.1 Ihr Projekt

Tower Defence: Stellverteidigung, um deine Basis zu schützen. 


Die Spieler muss seine Base beschützen. Die Gegner versucht die Base von den Spieler zu kommen und zu zerstören. Um das zu verhindern muss die Spieler sein Base verteidigen und im dem selben Zeit den Gegner töten. Die Spieler kann auswählen, wo er sein Tower platzieren kann. Er kann so viel Türme platzieren, wie er kann. Danach kann er bei dem Gegner zielen und abschiessen. Das alles Programmieren wir im Unity.


### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    |muss|Qualität| Als ein Spieler möchte ich dass das Spiel sauber läuft, damit die Erfahrung besser ist.|
| 2  |muss|Funktional|Als ein Spieler möchte ich dass das Spiel wenig Bugs hat, damit das Spiel spielbar ist.|
| 3  |muss|Funktional|Als ein Spieler möchte ich Towers funktional platzieren können, damit das Spiel nicht zu einfach oder zu schwer wird.|
| 4  |muss|Funktional|Als ein Spieler möchte ich herausgefordert werden, damit das Spiel Spass macht.|
| 5  |muss|Funktional|Als ein Spieler möchte ich interessantes Gameplay, damit ich ein Grund habe, das Spiel zu spielen.|
| 6  |muss|Qualität|Als ein Spieler möchte ich, dass meine Türme unterschiedlich aussehen, sodass ich sie unterscheiden kann.|
| 7  |muss|Funktional|Als ein Spieler möchte ich das meine Tower präzise die Gegner treffen, damit das Spiel nicht unfair wird.|
| 8  |kann|Qualität|Als ein Spieler möchte ich dass das Spiel visuell schön aussieht, damit die Erfahrung besser ist.|
| 9  |kann|Qualität|Als ein Spieler möchte ich das Spiel pausieren können, damit ich nicht gezwungen bin das Spiel früh zu beenden.|
| 10  |kann|Qualität|Als ein Spieler möchte ich am Ende meines Spieles mein High-Score sehen, damit ich weiss wie gut ich war.|
| 11 |kann|Fukional| Als ein Spieler möchte ich verschiedene Schwierigkeiten aussuchen, damit das Spiel interessanter wirkt.|
| 12 |kann|Qualität| Als Spieler möchte ich verschiedene Skins kaufen können, sodass es mehr Abwechslung bei den Türmen gibt.|
| 13 |kann|Qualität| Als Spieler möchte ich am Ende des Spiels mit einer Ingame-Währung Belohnt werden|
| 14 |kann|Qualität| Als Spieler möchte ich verschiedene Maps auswählen, weil so das Spiel vielseitiger ist.|
| 15 |kann|Funktional| Als Spieler möchte ich, dass meine Türme langsam an Leben verlieren, sodass das Spiel interaktiver ist.|


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1 |Das Spiel wird gestartet| Spieler spielt |Das Spiel funktioniert einwandfrei|
| 1.1  |Spiel startet|Ein Menü taucht auf| Schönen Ausblick in das Spiel|
| 1.2  |Das Spiel wird gestartet| Spieler wählt Niveau aus| Das gewählte Niveau wird angezeigt und gespielt|
| 2 |Spieler spielt weiter| Spieler platziert ein Turm| Spieler kann den Turm platzieren ohne Probleme|
| 3  |Spieler spielt weiter| Spieler legt viele Türme |Die Türme müssen platziert sein.|
| 4  |Spieler spielt weiter| Spieler platziert türme abhängig von seiner Energie|spieler kann nicht weiter platzieren ohne genug Energie.|
| 5  | Spiel ist bereit| Spieler ist jetzt bereit für die Gegner |das Spiel zeigt an, dass die Gegner jetzt angreifen werden. |
| 6  | Gegner kommen| Die Türmer fixieren sich auf den Gegner und schiesst | Gegner sind Tot|
| 7 | Spieler spielt weiter| Spieler drückt Stopp taste/Symbol| Das Spiel wird gestoppt|
| 8  |  Spieler spielt weiter |Spieler/ Türme schiesst Gegner |Zählt Punkte/Highscore|
| 8.1|Kommt ans Ende des Spiels| Spieler spielt fertig |Highscore wird angezeigt|
| 8.2|Kommt ans Ende des Spiels| Spieler erhält Punkte |Spieler kann jetzt in den Shop gehen.| $
| 9 | Das Spiel Shop wird angezeigt| Spieler kauft verschiede Skins | Spieler kann die neuen Skins ausprobieren. |
| 9.1  |Spieler ist im shop|Spieler wählt Skins aus, die er sich leisten kann| Spieler kann jetzt Skins im Spiel benutzen|
| 10  |Spieler spiel neue Runde|Spieler hat Skins gekauft|Die Skins werden korrekt angezeigt.|

### 1.4 Diagramme

![image](https://user-images.githubusercontent.com/111046257/220876770-4f72536c-3310-44da-9a93-72f0e3d8db4d.png)



<img width="750" alt="image" src="https://user-images.githubusercontent.com/111045600/220882164-ed35f0b2-8945-441f-9bf6-09a9e7359acf.png">




## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1  | 16.03.2023 | Alle | Schauen das es einwandfrei funktioniert|50 min|
| 1.A | 09.03.2023 | Sathana | Menü programmieren | 30 min| 	
| 1.B  | 16.03.2023| Joel | Niveaus programmieren| 30min |
| 2  | 09.03.2023 | Joel | nur ein Turm Platzierung programmieren | 20 min|
| 3  | 09.03.2023 | Joel | viele Türme Platzierung programmieren|20 min|
| 4  | 09.03.2023| Alle | so programmieren das der Spieler nur Türme platzieren kann wenn er Energie hat.| 30 min|
| 5   | 09.03.2023 | Alle | So Programmieren das es angezeigt wird, wenn Gegner kommen. | 40 min|
| 6  | 16.03.2023 | Alle | Programmieren das die Türmer auf den Gegner fixiert sind| 35 min|
| 6.A | 16.03.2023 | Joel |So Programmieren damit die Gegner auch sterben, wenn sie abgestossen werden| 25 min|
| 7  | 23.03.2023 | Alle | Stopp/pause Symbol programmieren| 20 min|
| 8  | 23.03.2023| Sathana | Anzahl Punkte Zählen  |25 min|
| 8.A  | 23.03.2023| Sathana | Highscore soll angezeigt werden | 20 min|
| 8.C | 09.03.2023 | Joel | Map erstellen | 40 min|
| 9  | 23.03.2023| Kilian |Verschiedene Skins programmieren | 30 min|
| 9.A  | 23.03.2023| Kilian| Diese Skins auch im Spiel verwendbar machen  |20 min|
| 10  | 23.03.2023| Alle | Neue Runde programmieren | 25 min|




Total: 440

## 3 Entscheiden

Wir haben entschieden das wir im Unity programmieren. Der Spieler kann verschiedene Türme auswählen und platzieren. Wir haben auch entschieden das wir einen Shop erstellen. So dass der Spieler seine Sachen kaufen kann, die er im Spiel mit Punkten erreicht hatte. Wir haben auch entschieden das der Spieler auch mehrere Schwierigkeiten wählen kann. 

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  | 09.03.2023 | Sathana | 30 min | 90 min|
| 2  | 09.03.2023 | Joel | 20 min | 90 min|
| 8.C | 09.03.2023 | Joel | 40 min | 80 min|
| 3  | 16.03.2023 | Kilian/Joel | 20 min | 65 min|
| 6 | 16.03.2023 | Joel | 35 min | 70 min |
| 7 | 16.03.2023 | Sathana | 20 min | 60 min | 
| 1 | 17.03.2023 | Alle | 50 | 135 min |
|1.B| - | Joel | 30 min | - |
| 4 | 17.03.2023 | Alle | 30 min | - |
| 5 | 17.03.2023 | Alle| 40 min| - |
| 6.A | 17.03.2023 | Joel | 25 min| 40 min |
| 8 | 17.03.2023 | Sathana | 25 min | - |
| 8.A | 17.03,2023| Sathana | 20 min | - |
| 9 | 17.03.2023 | Kilian | 30 min | - |
| 9.A | 17.03.2023 | Kilian | 20 min | - |
| 10  | 17.03.2023| Alle | 25 min| - |




## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| 1   | 05.04.2023 |OK  | Sathana |
| 1.1| 05.04.2023 |OK |  Sathana |
| 1.2| 05.04.2023 |  -    | Sathana |
| 2  |   05.04.2023 |OK  | Sathana |
| 3  |  05.04.2023  |OK  | Sathana |
| 4  |  05.04.2023  |   -   | Sathana |
| 5  |  05.04.2023  |OK  | Sathana |
| 6  |  05.04.2023  |OK  | Sathana |
| 7  |  05.04.2023  |OK  | Sathana |
| 8  |  05.04.2023  |  -    | Sathana |
| 8.1| 05.04.2023  |  -    | Sathana |
| 8.2| 05.04.2023  |   -   | Sathana |
| 9  |   05.04.2023  |OK  | Sathana |
| 9.1|  05.04.2023  |OK  | Sathana |
| 10 |  05.04.2023  |OK  | Sathana |

Bei dem Resultat (-) heisst es, dass wir sie nicht programmiert haben. Aber man kann das Spiel trotzdem spielen, auch wenn das nicht verfügbar ist. Zeitlich reichten für uns die Erweiterungen zu programmieren. 


✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.


## 6 Auswerten

https://github.com/Saadu02/LA_1500/blob/main/Lern-Bericht.md
