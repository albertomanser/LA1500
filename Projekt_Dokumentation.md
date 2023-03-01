# Projekt-Dokumentation

Gruppenname: Gardenia

Gruppenmitglieder: Atputharasa, Bächli, Kritzner, Manser 

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|  21.02.23     | 0.0.1   | Dokumentation angefangen und Schritte 1.1, 1.2 und 1.4 ausgefüllt. |


## 1 Informieren

### 1.1 Ihr Projekt

Allen hat das Programmieren mit Windows Forms am besten gefallen und wollen zusätzlich unsere Kenntnise darin vertiefen. Deswegen haben wir uns dazu entschlossen ein Flappy Bird Game zu programmieren. Das Game soll viele neue, einzigartige Level haben, die man mit Schlüsseln freischalten kann. Die Schlüssel kann man kaufen, wenn man einen genug hohen Score hat. Wir möchten am Schluss ein funktionales Spiel haben und dabei noch einiges über Windows Forms lernen. 

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1 | Muss | Funktional | Als ein Spieler möchte ich den Vogel steuern, damit ich den Pipes Ausweichen kann. |
| 2 | Muss | Funktional | Als ein Spieler möchte ich eine Form von Behlohnung erhalten, indem ich Leistungen erbringe. | 
| 3 | Kann | Qualität | Als ein Spieler möchte ich verschiedene Level spielen können. |
| 4 | Kann | Qualität | Als ein Spieler möchte ich verschiedene Easter Eggs im Spiel finden können.|
| 5 | Muss | Funktional | Als ein Spieler möchte ich, eine neue Runde starten können. |
| 6 | Muss | Funktional | Als ein Spieler möchte ich, dass die Hindernisse unterschiedlich sind. |
| 7 | Muss | Funktional | Als ein Spieler möchte ich wissen, wie weit ich gekommen bin und wie lange ich überlebt habe. |
| 8 | Muss | Funktional | Als ein Programmierer möchte ich, dass das Spiel absturzsicher ist. |
| 9 | Muss | Funktional |Als ein Spieler möchte ich mein Highscore im Menu sehen. |
| 10 | Kann | Qualität | Als Spieler möchte ich verschiedene Skins verwenden können |
| 11 | Muss | Rand | Das Programm soll in C# geschrieben werden. |

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |  Das Spiel ist gestartet und der Vogel ist auf der Mitte des Bildschirms zu sehen. | – |   Der Vogel stürzt ab |
| 1.2  |  Das Spiel ist gestartet            |  Spacebar drücken       | Der Vogel ändert seine Flughöhe entsprechend der Eingabe.                   |
| 2.1  |   Das Spiel ist gestartet            |   Erfolgreiches Durchfliegen von Pipes      | Der Spieler erhält eine Belohnung, z.B. ein neues Outfit für den Vogel.                   |
| 2.2  |  Das Spiel ist gestartet             |  Kollision mit Pipe       | Der Spieler erhält keine Belohnung.                 |
| 3.1  |Spiel gestartet|nichts|Welches Level wollen sie spielen?|
| 3.2  | Spiel gestartet | Level wird ausgewählt | das Level startet |
| 4.1  |Level wird gestartet|Easter Egg gefunden|Glückwunsch sie haben eine Münze erhalten|
| 5.1  | Spieler hat verloren | Level neustarten | Level startet neu |
| 6.1  | Spiel gestartet | Level auswählen und starten | Hindernisse haben sich entsprechend dem Level angepasst |
| 7.1  | Spiel gestartet | Spiel wird für eine gewisse Zeit gespielt | Zeit wie lange man überlebt hat wird angezeigt |
| 8.1  | Spiel gestartet | alles mögliche | Das Programm läuft weiter|
| 9.1  |  Spieler öffnet das Menü            | -        |  Der Spieler sieht seinen aktuellen Highscore.                 |
| 9.2  |  Spiel läuft, Spieler erzielt einen neuen Highscore            |   -      | Der Spieler sieht seinen neuen Highscore im Menü.                  |
| 10.1  | Shop geöffnet | Skin kaufen | Skin wurde erfolgreich gekauft und wurde der Garderobe hinzugefügt |
| 10.2  | Garderobe geöffnet | Skin auswählen | Skin wurde erfolgreich ausgewählt |

### 1.4 Diagramme

![image](https://user-images.githubusercontent.com/110893260/220314499-43efbc8b-20fd-414d-9a49-928b7b0b1a45.png)
![Hauptprogramm 1](https://user-images.githubusercontent.com/110892683/220312679-2a105031-0689-45fe-8ebc-e986ed8d7211.png)
![Level auswählen](https://user-images.githubusercontent.com/110892683/220312706-61c6b973-f979-4f91-912c-ae0ad61e6b57.png)


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 07.03.23       | Atputharasa          |    Implementierung der Vogel-Steuerung          |  35'             |
| 1.B  |  07.03.23      | Atputharasa           |  Testen der Vogel-Steuerung            |        5'       |
| 1.C  |  07.03.23      | Atputharasa           |  Anpassung der Steuerungsempfindlichkeit            |   10'            |
| 2.A  | 07.03.23 | Kritzner | Der Spieler kann Münzen aufsammeln | 45min |
| 2.B  | 07.03.23 | Kritzner | Der Spieler erhält am Schluss vom Level extra Münzen (Für jede Pipe 1 Münze extra) | 60min |
| 2.C  | 07.03.23 | Kritzner | Wenn der Spieler einen Highscore macht kann er am Ende der Runde eine Truhe für Münzen kaufen (enthält Skins) | 60min |
| 3.A  | 7.3.2023|Manser|implementierung der Levelauswahl| 60|
| 4.A  | 14.3.2023|Manser| Implementierung verschiedener Easter Eggs| 2 x 45|
| 5.A  | 07.03.23         |  Atputharasa            | Implementierung der Neustart-Funktion             |    15'           |
| 5.B  | 07.03.23        |  Atputharasa            |  Testen der Neustart-Funktion            |           5'    |
| 6.A  |   07.03.23      | Atputharasa             | Planung der unterschiedlichen Hindernistypen             |     15'          |
| 6.B  |   07.03.23      |  Atputharasa            | Implementierung der Hindernistypen             |     45'          |
| 6.C  | 07.03.23        |   Atputharasa           |  Testing der Hindernistypen            |          5'     |
| 7.A  |       |           |              |               |
| 7.B  |       |           |              |               |
| 7.C  |       |           |              |               |
| 7.D  |       |           |              |               |
| 8.A  |       |           |              |               |
| 8.B  |       |           |              |               |
| 8.C  |       |           |              |               |
| 8.D  |       |           |              |               |
| 9.A  |    07.03.23     |        Atputharasa      |  Implementierung einer Anzeige für den aktuellen Highscore.            |   25'            |
| 9.B  |    07.03.23     |       Atputharasa       | Implementierung einer Funktion, um den Highscore im Menü anzuzeigen.             | 15'              |
| 9.C  |     07.03.23    |       Atputharasa       | Testen der Anzeige auf Richtigkeit.             |       5'        |
| 10.A  | 14.03.23 | Kritzner | Einen Shop erstellen wo man Skins kaufen kann | 3 x 45min |
| 10.B  | 14.03.23 | Kritzner | Im Shop gibt es mehrere Skins | 2 x 45min |
| 10.C  | 21.03.23 | Kritzner | Überprüfen ob der Spieler genügend Münzen hat um einen Skin zu kaufen | 20min |
| 10.D | 21.03.23 | Kritzner | Der Spieler kann die gekauften Skins in einer Garderobe anziehen | 2 x 45min |




Total: 

## 3 Entscheiden

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

## 6 Auswerten
