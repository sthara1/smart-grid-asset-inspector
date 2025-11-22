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
-> zusätzlich manuell schaltbar.

## 📁 Projektstruktur

