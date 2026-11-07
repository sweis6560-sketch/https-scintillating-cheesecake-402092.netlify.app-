# Livewave — Livestream-App

Eine responsive, deutschsprachige Livestream-Discovery-Web-App als vollständige Überarbeitung des bisherigen leeren Repositorys.

## Enthalten
- Live-Entdecken-Seite mit Suche und Kategorie-Filtern
- Stream-Karten mit Creator-, Kategorie- und Zuschauerinformationen
- Demo-Watchroom mit Player-Platzhalter, Follow-Schaltfläche und lokalem Chat
- Stream-Planungsformular für Creator
- Responsive Layout für Desktop und Mobilgeräte
- Sicherheits-Header über Netlify `_headers`

## Lokal starten
Die App ist eine statische Website. Öffne `index.html` direkt im Browser oder starte einen beliebigen lokalen Static-File-Server.

## Netlify
Das Repository kann direkt als Netlify-Site verbunden werden. Build command leer lassen; Publish directory auf `.` setzen. Die Datei `netlify.toml` enthält diese Einstellungen.

## Wichtige Grenzen der Demo
Die Oberfläche enthält bewusst Demo-Daten. Der Player überträgt noch kein echtes Video; Chat, Follow und Stream-Planung sind lokal und nicht persistent. Für produktive Livestreams müssen ein Streaming-Anbieter (z. B. LiveKit oder Mux), ein Backend, echte Authentifizierung, persistente Datenhaltung, Moderation/Reporting und Datenschutz-/Impressumsseiten eingerichtet werden. API-Schlüssel niemals im Frontend hinterlegen.

## Sicherheit
Netlify-Header setzen unter anderem Content-Security-Policy, Referrer-Policy, X-Content-Type-Options und Permissions-Policy. Vor produktivem Betrieb die CSP bei Einbindung externer Streaming-/Auth-Dienste gezielt anpassen.
