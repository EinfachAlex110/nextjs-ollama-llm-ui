# Vollständig ausgestattete & schöne Web-Oberfläche für Ollama LLMs

<div align="center">
  <img src="ollama-nextjs-ui.gif">
</div>

<div align="center">
  
![GitHub Repo stars](https://img.shields.io/github/stars/jakobhoeg/nextjs-ollama-llm-ui)
  
</div>

Erhalten Sie **schnell**, **lokal** und sogar **offline** Zugang zu großen Sprachmodellen (LLMs). Dieses Projekt zielt darauf ab, der einfachste Weg für Sie zu sein, um mit LLMs zu starten. Keine mühsame und nervige Einrichtung erforderlich!

# Funktionen ✨

- **Schöne & intuitive Benutzeroberfläche**: Inspiriert von ChatGPT, um die Benutzererfahrung zu verbessern.
- **Vollständig lokal**: Speichert Chats zur Bequemlichkeit im lokalen Speicher. Keine Datenbank erforderlich.
- **Vollständig responsiv**: Nutzen Sie Ihr Telefon zum Chatten, mit der gleichen Leichtigkeit wie auf dem Desktop.
- **Einfache Einrichtung**: Keine mühsame und nervige Einrichtung erforderlich. Klonen Sie einfach das Repo und Sie sind startklar!
- **Code-Syntax-Hervorhebung**: Nachrichten, die Code enthalten, werden zur einfachen Nutzung hervorgehoben.
- **Einfaches Kopieren von Codeblöcken**: Kopieren Sie den hervorgehobenen Code mit einem Klick.
- **Modelle herunterladen/pullen & löschen**: Laden Sie Modelle direkt über die Oberfläche herunter und löschen Sie sie.
- **Schneller Wechsel zwischen Modellen**: Wechseln Sie schnell zwischen Modellen mit einem Klick.
- **Chatverlauf**: Chats werden gespeichert und sind leicht zugänglich.
- **Heller & Dunkler Modus**: Wechseln Sie zwischen hellem und dunklem Modus.

# Vorschau

https://github.com/jakobhoeg/nextjs-ollama-llm-ui/assets/114422072/08eaed4f-9deb-4e1b-b87a-ba17d81b9a02

# Voraussetzungen ⚙️

Um die Web-Oberfläche zu nutzen, müssen folgende Voraussetzungen erfüllt sein:

1. Laden Sie [Ollama](https://ollama.com/download) herunter und starten Sie es. Oder führen Sie es in einem Docker-Container aus. Schauen Sie in die [Dokumentation](https://github.com/ollama/ollama) für Anweisungen.
2. Node.js (18+) und npm sind erforderlich. [Download](https://nodejs.org/en/download)

# Eigene Instanz auf Vercel oder Netlify mit einem Klick bereitstellen ✨

[![Mit Vercel bereitstellen](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fjakobhoeg%2Fnextjs-ollama-llm-ui&env=NEXT_PUBLIC_OLLAMA_URL&envDescription=Your%20Ollama%20URL) [![Mit Netlify bereitstellen](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/jakobhoeg/nextjs-ollama-llm-ui)

Sie müssen die Umgebungsvariable [OLLAMA_ORIGINS](https://github.com/ollama/ollama/blob/main/docs/faq.md) auf Ihrem Rechner setzen, der Ollama ausführt:

```
OLLAMA_ORIGINS="https://your-app.vercel.app/"
```

# Installation 📖

[![Packaging status](https://repology.org/badge/vertical-allrepos/nextjs-ollama-llm-ui.svg?columns=3)](https://repology.org/project/nextjs-ollama-llm-ui/versions)

Verwenden Sie ein vorgefertigtes Paket von einem der unterstützten Paketmanager, um eine lokale Umgebung der Web-Oberfläche auszuführen. Alternativ können Sie aus dem Quellcode installieren, indem Sie den untenstehenden Anweisungen folgen.

> **Hinweis**  
> Wenn Ihr Frontend auf etwas anderem als `http://localhost` oder `http://127.0.0.1` läuft, müssen Sie die OLLAMA_ORIGINS auf Ihre Frontend-URL setzen.
>
> Dies wird auch in der [Dokumentation](https://github.com/ollama/ollama/blob/main/docs/faq.md#how-do-i-configure-ollama-server) angegeben:
>
> `Ollama erlaubt Cross-Origin-Anfragen von 127.0.0.1 und 0.0.0.0 standardmäßig. Zusätzliche Ursprünge können mit OLLAMA_ORIGINS konfiguriert werden`

## Installation aus dem Quellcode

**1. Klonen Sie das Repository in ein Verzeichnis auf Ihrem PC über die Eingabeaufforderung:**

```
git clone https://github.com/jakobhoeg/nextjs-ollama-llm-ui
```

**2. Öffnen Sie den Ordner:**

```
cd nextjs-ollama-llm-ui
```

**3. Benennen Sie die Datei `.example.env` in `.env` um:**

- Unter Windows:

  ```
  ren .example.env .env
  ```

- Unter Unix/Linux/MacOS:

  ```
  mv .example.env .env
  ```

**4. Wenn Ihre Ollama-Instanz NICHT auf der Standard-IP-Adresse und dem Standard-Port läuft, ändern Sie die Variable in der `.env`-Datei entsprechend Ihrem Anwendungsfall:**

```
NEXT_PUBLIC_OLLAMA_URL="http://localhost:11434"
```

**5. Installieren Sie die Abhängigkeiten:**

```
npm install
```

**6. Starten Sie den Entwicklungsserver:**

```
npm run dev
```

**7. Gehen Sie zu [localhost:3000](http://localhost:3000) und beginnen Sie mit Ihrem Lieblingsmodell zu chatten!**

# Kommende Funktionen

Diese Funktionen sind in Planung:

- ✅ Unterstützung für Spracheingabe
- ✅ Code-Syntax-Hervorhebung
- ⬜️ Möglichkeit, ein Bild im Prompt zu senden, um Vision-Sprachmodelle zu nutzen
- ⬜️ Möglichkeit, Antworten zu regenerieren
- ⬜️ Import und Export von Chats

# Technologie-Stack

- **Next.js**: React-Framework für das Web
- **Tailwind CSS**: Utility-First CSS-Framework
- **shadcn-ui**: UI-Komponenten basierend auf Radix UI und Tailwind CSS
- **shadcn-chat**: Chat-Komponenten für Next.js/React-Projekte
- **Framer Motion**: Animationsbibliothek für React
- **Lucide Icons**: Icon-Bibliothek

# Hilfreiche Links

[Medium-Artikel](https://medium.com/@bartek.lewicz/launch-your-own-chatgpt-clone-for-free-on-colab-shareable-and-online-in-less-than-10-minutes-da19e44be5eb) - Wie Sie Ihren eigenen ChatGPT-Klon kostenlos auf Colab starten können. Von Bartek Lewicz.

---

## Ausführliche Schritt-für-Schritt-Anleitung

Folgen Sie dieser ausführlichen Anleitung, um die Web-Oberfläche für Ollama LLMs auf Ihrem lokalen Rechner einzurichten.

### Voraussetzungen

- **Ollama** installiert und läuft auf Ihrem System.
- **Node.js (Version 18 oder höher)** und **npm** sind installiert.

### Schritt 1: Repository klonen

Öffnen Sie Ihr Terminal oder die Eingabeaufforderung und führen Sie den folgenden Befehl aus:

```
git clone https://github.com/jakobhoeg/nextjs-ollama-llm-ui
```

Dieser Befehl klont das Repository in ein Verzeichnis namens `nextjs-ollama-llm-ui`.

### Schritt 2: In das Projektverzeichnis wechseln

Navigieren Sie in das neu erstellte Verzeichnis:

```
cd nextjs-ollama-llm-ui
```

### Schritt 3: Umgebungsdatei konfigurieren

Bennen Sie die Datei `.example.env` in `.env` um:

- **Unter Windows:**

  ```
  ren .example.env .env
  ```

- **Unter Unix/Linux/MacOS:**

  ```
  mv .example.env .env
  ```

### Schritt 4: Umgebungsvariable anpassen (falls erforderlich)

Wenn Ihre Ollama-Instanz nicht auf der Standardadresse `http://localhost:11434` läuft, öffnen Sie die `.env`-Datei mit einem Texteditor und passen Sie die `NEXT_PUBLIC_OLLAMA_URL` entsprechend an:

```
NEXT_PUBLIC_OLLAMA_URL="http://Ihre-IP-Adresse:Ihr-Port"
```

### Schritt 5: Abhängigkeiten installieren

Installieren Sie die benötigten Pakete mit npm:

```
npm install
```

Dieser Befehl installiert alle erforderlichen Pakete, die im `package.json` definiert sind.

### Schritt 6: Entwicklungsserver starten

Starten Sie den Entwicklungsserver:

```
npm run dev
```

Nach dem Start sollte eine Meldung angezeigt werden, dass der Server auf `http://localhost:3000` läuft.

### Schritt 7: Web-Oberfläche aufrufen

Öffnen Sie Ihren Browser und navigieren Sie zu [http://localhost:3000](http://localhost:3000). Sie sollten die Web-Oberfläche sehen und können beginnen, mit Ihrem bevorzugten Modell zu chatten.

### Schritt 8: Ollama Origins einstellen (falls erforderlich)

Wenn Ihre Anwendung nicht auf `localhost` läuft, müssen Sie die Umgebungsvariable `OLLAMA_ORIGINS` auf Ihrem Rechner, der Ollama ausführt, einstellen:

- **Unter Unix/Linux/MacOS:**

  ```
  export OLLAMA_ORIGINS="http://Ihre-Frontend-URL"
  ```

- **Unter Windows (PowerShell):**

  ```
  $env:OLLAMA_ORIGINS="http://Ihre-Frontend-URL"
  ```

### Schritt 9: Modelle verwalten

Über die Web-Oberfläche können Sie Modelle herunterladen, löschen und zwischen ihnen wechseln:

- **Modelle herunterladen:** Navigieren Sie zum Abschnitt "Modelle" und klicken Sie auf "Herunterladen" oder "Pull" neben dem gewünschten Modell.
- **Modelle löschen:** Klicken Sie auf "Löschen" neben dem Modell, das Sie entfernen möchten.
- **Zwischen Modellen wechseln:** Verwenden Sie das Dropdown-Menü, um das aktive Modell zu ändern.

### Zusätzliche Hinweise

- **Code-Syntax-Hervorhebung:** Wenn das Modell Code in seinen Antworten bereitstellt, wird dieser automatisch hervorgehoben.
- **Kopieren von Codeblöcken:** Sie können Codeblöcke einfach kopieren, indem Sie auf das Kopiersymbol klicken.
- **Chatverlauf:** Ihre Chats werden im lokalen Speicher Ihres Browsers gespeichert und sind leicht zugänglich.

### Fehlersuche

- **Problem:** **Fehler beim Starten des Entwicklungsservers.**
  - **Lösung:** Stellen Sie sicher, dass alle Abhängigkeiten korrekt installiert sind und dass Sie Node.js Version 18 oder höher verwenden.
- **Problem:** **Die Anwendung kann keine Verbindung zu Ollama herstellen.**
  - **Lösung:** Überprüfen Sie, ob Ollama läuft und dass die `NEXT_PUBLIC_OLLAMA_URL` korrekt in der `.env`-Datei eingestellt ist.
- **Problem:** **CORS-Fehler beim Zugriff auf Ollama.**
  - **Lösung:** Stellen Sie sicher, dass die Umgebungsvariable `OLLAMA_ORIGINS` auf die URL Ihrer Web-Oberfläche gesetzt ist.

### Deployment auf Vercel oder Netlify

Sie können die Anwendung auch online bereitstellen:

- **Vercel:**

  Klicken Sie auf den "Mit Vercel bereitstellen"-Button und folgen Sie den Anweisungen. Stellen Sie sicher, dass Sie die Umgebungsvariable `NEXT_PUBLIC_OLLAMA_URL` einstellen.

- **Netlify:**

  Klicken Sie auf den "Mit Netlify bereitstellen"-Button und folgen Sie den Anweisungen.

**Hinweis:** Bei Online-Deployments muss Ollama öffentlich zugänglich sein, was Sicherheitsrisiken mit sich bringen kann. Stellen Sie sicher, dass Sie geeignete Sicherheitsmaßnahmen ergreifen.

### Kommende Funktionen

Bleiben Sie gespannt auf zukünftige Updates, die weitere Funktionen hinzufügen, wie z.B.:

- Unterstützung für Vision-Sprachmodelle durch Senden von Bildern.
- Möglichkeit, Antworten zu regenerieren.
- Import und Export von Chats für eine bessere Verwaltung.

### Unterstützende Ressourcen

- **Ollama Dokumentation:** [https://github.com/ollama/ollama](https://github.com/ollama/ollama)
- **Medium-Artikel für weitere Einblicke:** [Wie Sie Ihren eigenen ChatGPT-Klon kostenlos starten](https://medium.com/@bartek.lewicz/launch-your-own-chatgpt-clone-for-free-on-colab-shareable-and-online-in-less-than-10-minutes-da19e44be5eb)

---

**Viel Erfolg bei der Einrichtung!** Wenn Sie auf Probleme stoßen oder Fragen haben, zögern Sie nicht, die Dokumentation zu konsultieren oder Unterstützung zu suchen.

[Lobehub mention](https://lobehub.com/blog/5-ollama-web-ui-recommendation#5-next-js-ollama-llm-ui) - Five Excellent Free Ollama WebUI Client Recommendations
