# smart-grid-asset-inspector

# EGS Grid Insights Dashboard

Dieses Projekt ist ein interaktives Energie-Dashboard, das verschiedene Kennzahlen aus einem Stromnetz (Grid) visuell darstellt.  
Die Idee dahinter: Ein übersichtliches Interface, das Live-Änderungen simuliert und typische KPI-Bereiche eines Netzbetreibers abdeckt – ohne externe Datenquellen.

Ich habe das Dashboard als eigenes Projekt umgesetzt, um Erfahrungen mit React, Recharts und komplexeren UI-Layouts zu sammeln.

## Ziel des Projekts
Der Fokus liegt darauf, ein realistisches Energie/Netz-Dashboard zu bauen, wie man es aus Control-Center-Umgebungen kennt:

- Live-Kennzahlen (Stabilität, Flexibilität, Spannung etc.)
- Wöchentliche Trendgrafiken
- Standort-Risikobewertung (EGS Locations)
- Health-Monitoring (System Zustand)
- Batterie-Status & Energie-Mix
- Alerts / Event Feed
- Light/Dark Mode inkl. Auto-Theme (nach Uhrzeit)

Das Ganze soll technisch verständlich bleiben und gleichzeitig optisch wie eine „echte“ Dashboard-Lösung aussehen.

## Tech Stack
- **React (Vite + TypeScript)**
- **Recharts** für Diagramme
- **CSS Grid & Flexbox** für das Layout
- **Poppins** als Hauptschrift
- Keine zusätzlichen UI-Libraries – alles „handgebaut“

## Features im Überblick

### Live-KPIs  
Alle KPI-Werte werden alle paar Sekunden aktualisiert.  
Das simuliert das Verhalten echter Netz-Telemetrie.

### Trendcharts (Mo–So)
Mehrere Diagramme:

- Grid Stability  
- Flexibility  
- Connectivity  
- Voltage Variance  
- Energy Forecast  
- CO₂-Trend  
- 24h Load Forecast  
- Energy Mix (Bar Chart)

Alle mit schwarzen Achsen für gute Lesbarkeit.

###  EGS Locations (Standorte)
Jeder Standort zeigt:

- Auslastung in %  
- Risiko-Stufe (Low → Critical)

Ideal, um Netzgebiete zu vergleichen.

### System Health
Zeigt Grid-Stabilität, Spannungsschwankungen und Gesamtstatus.

### Battery Storage Modul
Ein kleiner Speicher-Monitor:

- Ladezustand  
- Lade-/Entladeleistung  
- Zyklen des Tages

### Renewable Index
Anteil erneuerbare Energien  
-> visuell über einen Fortschrittsbalken.

### Alerts & Activity Feed
Echtzeit-Benachrichtigungen über:

- Spannungssprünge  
- Prognoseänderungen  
- Simulationsereignisse  

### Light/Dark Mode
Wechselt automatisch nach Zeit  
---
EGS-Grid-App/
│
├── public/ # statische Dateien (Favicon usw.)
│
├── src/
│ ├── App.tsx # Hauptkomponente (Dashboard)
│ ├── App.css # komplettes Styling
│ ├── main.tsx # React Einstiegspunkt
│ └── assets/ # (optional) Bilder/Icons
│
├── index.html
├── vite.config.ts
├── package.json
└── README.md


Ich habe alles in einer Datei (`App.tsx`) gehalten, um es übersichtlich und einfach nachvollziehbar zu halten.  
In einer größeren Anwendung würde man Panels und Komponenten natürlich aufsplitten.

## Lokales Starten

1. Abhängigkeiten installieren
2. Dev-Server starten  
-> zusätzlich manuell schaltbar.
   
3. App öffnen  
http://localhost:5173


## 🌐 Deployment
Das Projekt ist Vite-basiert und kann problemlos über **Vercel**, **Netlify** oder **GitHub Pages** deployed werden.

## 📌 Warum ich das gebaut habe
Ich wollte ein Dashboard entwickeln, das:

- visuell überzeugt  
- technisch sauber aufgebaut ist  
- klar strukturiert bleibt  
- reale Energie-Themen widerspiegelt  
- und später erweiterbar ist (z. B. Live-APIs, WebSockets, PowerApps Integration)

Das Projekt eignet sich gut als Portfolio-Eintrag, weil man dabei mehrere Bereiche kombiniert:  
UI, State-Management, Charts, Live-Simulation und ein durchdachtes Layout.

## Ausblick
Geplant sind:

- Optional echte Live-Daten (z. B. ENTSO-E API)
- Export-Funktion (Report)
- Rechteverwaltung / Login
- Einbindung als Custom Page in PowerApps

---

Wenn du Feedback oder Erweiterungen hast, freue ich mich.



## 📁 Projektstruktur

