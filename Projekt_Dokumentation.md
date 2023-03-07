# Projekt-Dokumentation

Gruppenname: Gardenia

Gruppenmitglieder: Atputharasa, Bächli, Kritzner, Manser 

| Datum    | Version | Zusammenfassung                                                           |
| -------- | ------- | ------------------------------------------------------------------------- |
| 21.02.23 | 0.0.1   | Dokumentation angefangen und Schritte 1.1, 1.2 und 1.4 ausgefüllt.        |
| 28.02.23 | 0.0.2   | Realisieren angefangen und Arbeitspakete eingeteilt 1.3 und 2 ausgefüllt. |
| 07.03.23 | 0.0.2   | Realisieren angefangen und Arbeitspakete eingeteilt 1.3 und 2 ausgefüllt. |

## 1 Informieren

### 1.1 Ihr Projekt

Allen hat das Programmieren mit Windows Forms am besten gefallen und wollen zusätzlich unsere Kenntnise darin vertiefen. Deswegen haben wir uns dazu entschlossen ein Flappy Bird Game zu programmieren. Das Game soll viele neue, einzigartige Level haben, die man mit Schlüsseln freischalten kann. Die Schlüssel kann man kaufen, wenn man einen genug hohen Score hat. Wir möchten am Schluss ein funktionales Spiel haben und dabei noch einiges über Windows Forms lernen. 

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ        | Beschreibung                                                                                  |
| ---- | --------------- | ---------- | --------------------------------------------------------------------------------------------- |
| 1    | Muss            | Funktional | Als ein Spieler möchte ich den Vogel steuern, damit ich den Pipes Ausweichen kann.            |
| 2    | Muss            | Funktional | Als ein Spieler möchte ich eine Form von Belohnung erhalten, damit ich motivierend weiterspiele.  |
| 3    | Kann            | Qualität   | Als ein Spieler möchte ich verschiedene Level spielen können, damit es abwechslungsreich ist.                                 |
| 4    | Kann            | Qualität   | Als ein Spieler möchte ich verschiedene Easter Eggs im Spiel finden können, damit ich Spass habe.                   |
| 5    | Muss            | Funktional | Als ein Spieler möchte ich, eine neue Runde starten können, damit ich weiterspielen kann.                                   |
| 6    | Muss            | Funktional | Als ein Spieler möchte ich, dass die Pipes unterschiedlich positioniert sind, damit es herausfordernd ist.                        |
| 7    | Muss            | Funktional | Als ein Spieler möchte ich wissen, wie weit ich gekommen bin und wie lange ich überlebt habe, damit ich weiss, wenn ich meinen Highscore biete. |
| 8    | Muss            | Funktional | Als ein Programmierer möchte ich, dass das Spiel absturzsicher ist, damit ich ohne Probleme spielen kann.                           |
| 9    | Muss            | Funktional | Als ein Spieler möchte ich mein Highscore im Menu sehen, damit ich weiss, ab wann ich meinen Highscore biete.                                      |
| 10   | Kann            | Qualität   | Als Spieler möchte ich verschiedene Skins verwenden können, damit ich mehr Freude habe.                                |
| 11   | Muss            | Rand       | Das Programm soll in C# geschrieben werden.                                                   |

### 1.3 Testfälle

| TC-№ | Ausgangslage                                                                      | Eingabe                                   | Erwartete Ausgabe                                                       |
| ---- | --------------------------------------------------------------------------------- | ----------------------------------------- | ----------------------------------------------------------------------- |
| 1.1  | Das Spiel ist gestartet und der Vogel ist auf der Mitte des Bildschirms zu sehen. | –                                         | Der Vogel stürzt ab                                                     |
| 1.2  | Das Spiel ist gestartet                                                           | Spacebar drücken                          | Der Vogel ändert seine Flughöhe entsprechend der Eingabe.               |
| 2.1  | Das Spiel ist gestartet                                                           | Erfolgreiches Durchfliegen von Pipes      | Der Spieler erhält eine Belohnung, z.B. ein neues Outfit für den Vogel. |
| 2.2  | Das Spiel ist gestartet                                                           | Kollision mit Pipe                        | Der Spieler erhält keine Belohnung.                                     |
| 3.1  | Spiel gestartet                                                                   | nichts                                    | Welches Level wollen sie spielen?                                       |
| 3.2  | Spiel gestartet                                                                   | Level wird ausgewählt                     | das Level startet                                                       |
| 4.1  | Level wird gestartet                                                              | Easter Egg gefunden                       | Glückwunsch sie haben eine Münze erhalten                               |
| 5.1  | Spieler hat verloren                                                              | Level neustarten                          | Level startet neu                                                       |
| 6.1  | Spiel gestartet                                                                   | Level auswählen und starten               | Hindernisse haben sich entsprechend dem Level angepasst                 |
| 7.1  | Spiel gestartet                                                                   | Spiel wird für eine gewisse Zeit gespielt | Zeit wie lange man überlebt hat wird angezeigt                          |
| 8.1  | Spiel gestartet                                                                   | alles mögliche                            | Das Programm läuft weiter                                               |
| 9.1  | Spieler öffnet das Menü                                                           | -                                         | Der Spieler sieht seinen aktuellen Highscore.                           |
| 9.2  | Spiel läuft, Spieler erzielt einen neuen Highscore                                | -                                         | Der Spieler sieht seinen neuen Highscore im Menü.                       |
| 10.1 | Shop geöffnet                                                                     | Skin kaufen                               | Skin wurde erfolgreich gekauft und wurde der Garderobe hinzugefügt      |
| 10.2 | Garderobe geöffnet                                                                | Skin auswählen                            | Skin wurde erfolgreich ausgewählt                                       |

### 1.4 Diagramme

![image](https://user-images.githubusercontent.com/110893260/220314499-43efbc8b-20fd-414d-9a49-928b7b0b1a45.png)
![Hauptprogramm 1](https://user-images.githubusercontent.com/110892683/220312679-2a105031-0689-45fe-8ebc-e986ed8d7211.png)
![Level auswählen](https://user-images.githubusercontent.com/110892683/220312706-61c6b973-f979-4f91-912c-ae0ad61e6b57.png)

## 2 Planen

| AP-№ | Frist      | Zuständig   | Beschreibung                                                                                                       | geplante Zeit |
| ---- | ---------- | ----------- | ------------------------------------------------------------------------------------------------------------------ | ------------- |
| 1.A  | 07.03.23   | Atputharasa | Implementierung der Vogel-Steuerung                                                                                | 35'           |
| 2.B  | 07.03.23   | Kritzner    | Der Spieler erhält am Schluss vom Level extra Münzen (Für jede Pipe 1 Münze extra)                                 | 60min         |
| 2.C  | 07.03.23   | Kritzner    | Wenn der Spieler einen Highscore macht kann er am Ende der Runde eine Truhe für Münzen kaufen (enthält Skins)      | 60min         |
| 3.A  | 07.03.2023 | Manser      | Implementierung der Levelauswahl                                                                                   | 60            |
| 3.B  | 07.03.2023 | Manser      | Design der Benutzeroberfäche für die Levelauswahl                                                                  | 60            |
| 3.C  | 07.03.2023 | Manser      | Highscore für die verschiedene Levelauswahl zu speichern                                                           | 60            |
| 3.D  | 07.03.2023 | Manser      | Implementierung der Überprüfung, ob der Spieler das ausgewählte Level freigeschaltet hat                           | 60            |
| 4.A  | 14.03.2023 | Manser      | Implementierung verschiedener Easter Eggs                                                                          | 2 x 45        |
| 4.B  | 14.03.2023 | Manser      | Festlegen der Easter-Egg-Regeln und deren Platzierung im Spiel                                                     | 60            |
| 4.C  | 14.03.2023 | Manser      | Implementierung der Easter-Egg-Suche-Logik                                                                         | 60            |
| 5.A  | 07.03.23   | Atputharasa | Implementierung der Neustart-Funktion                                                                              | 15'           |
| 5.B  | 07.03.2023 | Atputharasa | Implementierung der Benutzeroberfläche, um den Neustart-Button anzuzeigen                                          | 60            |
| 5.D  | 07.03.2023 | Atputharasa | Implementierung der Funktionalität, um das Spiel zurückzusetzen und eine neue Runde zu starten                     | 60            |
| 5.E  | 07.03.2023 | Atputharasa | Implementierung der Bestätigungsfunktion, um zu verhindern, dass der Spieler versehentlich ein neues Spiel startet | 60            |
| 6.A  | 07.03.23   | Atputharasa | Planung der unterschiedlichen Pipes                                                                                | 15'           |
| 6.B  | 07.03.23   | Atputharasa | Implementierung der Pipestypen                                                                                     | 45'           |
| 6.C  | 07.03.2023 | Atputharasa | Implementierung der Logik zur Generierung von zufälligen Platzierung von Pipes                                     | 60            |
| 6.D  | 07.03.2023 | Atputharasa | implementierung der Levelauswahl                                                                                   | 60            |
| 7.A  | 07.03.23   | Bächli      | Implementierung des Highscores                                                                                     | 20'           |
| 7.B  | 07.03.23   | Bächli      | Implementierung der Überlebenszeit                                                                                 | 20'           |
| 7.C  | 07.03.23   | Bächli      | Design der Benutzeroberfläche für die Anzeige des Highscores und der Überlebensdauer                               | 20'           |
| 7.D  | 07.03.23   | Bächli      | Implementierung einer Funktion, um die Anzeige zu aktualisieren, wenn der Spieler voranschreitet oder stirbt       | 20'           |
| 7.E  | 07.03.23   | Bächli      | Implementierung einer Anzeige für den aktuellen Score.                                                             | 25'           |
| 8.A  | 14.3.23    | Bächli      | Identifizierung möglicher Absturzursachen im Code.                                                                 | 20'           |
| 8.B  | 14.3.23    | Bächli      | Beseitigen der potenziellen Absturzursachen                                                                        | 20'           |
| 9.A  | 07.03.23   | Manseer     | Implementierung eines Menu                                                                                         | 20'           |
| 9.B  | 07.03.23   | Bächli      | Implementierung einer Funktion, um den Highscore im Menü anzuzeigen.                                               | 15'           |
| 10.A | 07.03.2023 | Manser      | Skins designen                                                                                                     | 60            |
| 10.B | 14.03.23   | Kritzner    | Einen Shop erstellen wo man Skins kaufen kann                                                                      | 3 x 45min     |
| 10.C | 14.03.23   | Kritzner    | Im Shop gibt es mehrere Skins                                                                                      | 2 x 45min     |
| 10.D | 21.03.23   | Kritzner    | Überprüfen ob der Spieler genügend Münzen hat um einen Skin zu kaufen                                              | 20min         |
| 10.E | 21.03.23   | Kritzner    | Der Spieler kann die gekauften Skins in einer Garderobe anziehen                                                   | 2 x 45min     |

Total: 

## 3 Entscheiden

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 2.B  | 07.03.2023 | Filip Kritzner | 60min | 50min |
| 2.C  | 07.03.2023 | Filip Kritzner | 60min | 90min |
| 10.B  | 07.03.2023 | Filip Kritzner | 45min | 40min |

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


