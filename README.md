# Ollama Learning App

Die Ollama Learning App ist eine webbasierte Anwendung, die mithilfe der Ollama API KI-basierte Bewertungen für Lernfragen ermöglicht. Du kannst Fragen und Antworten per CSV importieren, über die KI bewerten lassen und deinen Lernfortschritt verfolgen – alles in einer modernen, responsiven Oberfläche.

## Voraussetzungen

- **Python 3.9+** (oder höher)  
  [Python herunterladen](https://www.python.org/downloads/)

- **Flask** – Ein leichtgewichtiges Webframework für Python  
- **Requests** – Zum Senden von HTTP-Anfragen an die Ollama API

- Eine laufende **Ollama API**-Instanz (z. B. mit dem Modell `gemma:27B`)  
  *Stelle sicher, dass die API unter der Standard-URL `http://localhost:11434` erreichbar ist oder passe die URL in den Einstellungen der App an.*

- Einen modernen Webbrowser (Chrome, Firefox, Edge etc.)

## Projektstruktur

Die Ordnerstruktur des Projekts sieht beispielsweise so aus:

ollama-learning-app/ ├── server.py # Flask-Backend zur Auslieferung des Frontends └── templates/ └── index.html # Das komplette Frontend (HTML, CSS, JavaScript)


## Installation

1. **Repository klonen oder Projektordner herunterladen**

   Falls das Projekt auf GitHub liegt:
   ```bash
   git clone https://github.com/dein-benutzername/ollama-learning-app.git
   cd ollama-learning-app


pip install flask requests
    Stelle sicher, dass die Ollama API läuft und über die URL erreichbar ist (Standard: http://localhost:11434).

    Über den Einstellungen-Tab im Frontend kannst du die API-URL, das gewünschte Modell und die Anzahl korrekter Antworten festlegen.

Ausführung der App

    Flask-Server starten:

python server.py

Der Server läuft standardmäßig unter http://127.0.0.1:5000.

Webbrowser öffnen: Navigiere in deinem Browser zu http://127.0.0.1:5000.

App nutzen:

    Einstellungen:
    Lege hier die Ollama API URL fest, wähle ein Modell aus und bestimme, wie viele korrekte Antworten nötig sind, um eine Frage abzuschließen.

    Import:
    Importiere Fragen und Antworten entweder per CSV-Datei oder manuell. Das CSV-Format sollte folgendermaßen aussehen:

        Frage,Richtige Antwort

        Lernen:
        Im Lern-Modul werden die Fragen angezeigt. Gib deine Antwort ein, lasse sie von der KI bewerten und verfolge deinen Fortschritt.

        Statistiken:
        Verfolge deinen Lernfortschritt und erkenne, welche Fragen noch Schwierigkeiten bereiten.

Fehlersuche

    Kein Modell ausgewählt:
    Achte darauf, dass du nach dem Aktualisieren der Modelle im Einstellungs-Tab ein Modell auswählst und anschließend auf „Einstellungen speichern“ klickst.

    Ollama API nicht erreichbar:
    Überprüfe, ob die API unter der eingestellten URL läuft. Bei CORS-Problemen oder Netzwerkfehlern sieh in der Browser-Konsole oder in den Server-Logs nach.