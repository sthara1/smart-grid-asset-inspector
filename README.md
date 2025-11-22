# EGS Grid Insights Dashboard  
*Smart-Grid Asset Inspector*

Ein interaktives Energiemanagement-Dashboard, das typische Kennzahlen eines Stromnetzes (Grid) visualisiert und simuliert.  
Der Fokus liegt auf einer klaren UI, Live-Änderungen und einem realistischen Control-Center-Feeling.

---

## Features

### **Live-KPIs**
- Grid Stability  
- Flexibility Index  
- Connectivity Quality  
- Voltage Variance  
- Energy Forecast  
- CO₂-Emissions

Alle Werte werden alle paar Sekunden automatisch angepasst, um Live-Daten zu simulieren.

---

### **Wöchentliche Trendgrafiken**
Für jeden KPI existiert ein eigener Trendchart (Recharts):

- Grid Stability (Week)
- Flexibility Index
- Connectivity Quality
- Voltage Variance
- Energy Forecast (7 Days)
- CO₂ Emission Trend

---

### **Standort-Monitoring (EGS Locations)**
Darstellung mehrerer Standorte mit:

- Live Load (%)
- Risikostatus (Low, Medium, High, Critical)
- Farb-Badges für schnelle Kontrolle

---

### **System Health**
Zusammenfassung wichtiger Gesamtwerte:

- Grid Stability
- Voltage Variance
- Overall Status

---

### **Battery Storage**
Informationen wie:

- State of Charge
- Ladeleistung
- Zyklen pro Tag

---

### **Renewable Mix**
Balken-Visualisierung des erneuerbaren Anteils des aktuellen Energiemixes.

---

### **Alerts & Event Feed**
Live-Simulation von Warnmeldungen:

- Spannungsschwankungen  
- Prognoseabweichungen  
- Standortüberlastung  

Incl. CO₂-Einsparung des Tages.

---

### **Weather Impact**
Einfache Darstellung der Wettereinflüsse:

- Solar Output  
- Wind Potential  
- Temperatur

---

### **Light- & Dark-Mode**
Manuelles Umschalten — Code ist vorbereitet für automatische Zeitsteuerung.

---

## **Tech Stack**

| Bereich | Technologie |
|--------|-------------|
| Framework | **React + TypeScript** |
| Build Tool | **Vite** |
| Charts | **Recharts** |
| Styling | CSS (Poppins, Custom Layout) |
| State | React Hooks |
| Deployment | GitHub Pages, Netlify, Vercel oder PowerApps |

---

## 📁 Projektstruktur
src/
│
├─ assets/ → Icons, Logos, Bilder

├─ components/

│ ├─ charts/ → ChartPanel, EnergyMixChart, ForecastChart

│ ├─ layout/ → Header, GridContainer

│ ├─ panels/ → SystemHealthPanel, BatteryPanel, WeatherPanel

│ └─ widgets/ → KPI Cards, LocationTable, AlertsFeed
│
├─ data/ → Statische Testdaten / Seeds

├─ hooks/ → useLiveUpdate, useTheme, etc.

├─ styles/ → globale und modulare Stylesheets

├─ utils/ → Helper/Formatter (z. B. adjustValue)
│
├─ App.tsx → Hauptlayout

├─ main.tsx → Einstiegspunkt (ReactDOM)

└─ index.css → globale Basis-Styles




---

## Installation

### Abhängigkeiten installieren
```bash
npm install

npm run dev

Dashboard öffnen

➡ http://localhost:5173

Deployment

Das Dashboard kann deployed werden über:

GitHub Pages
npm run build


Output liegt in /dist.

Netlify / Vercel

Einfach das Repository verbinden – Build-Command:

npm run build

Output-Ordner:

dist

PowerApps (Custom Page)

✔ Deployment auf Netlify/Vercel
✔ URL in PowerApps über Iframe Control einbetten
✔ Funktioniert ohne Anpassungen

Warum dieses Projekt?

Ich wollte ein Dashboard entwickeln, das:

realistische Energiedaten simuliert

visuell stark ist

technisch klar strukturiert bleibt

mit echten Systemen erweiterbar ist (APIs, WebSockets)

sich als Portfolio-Projekt eignet

Es verbindet UI-Design, State-Management, Echtzeit-Simulation und komplexes Layout in einer kompakten Demo.

 Ausblick (geplante Erweiterungen)

Einbindung echter Live-Grid-Daten (ENTSO-E API)

Benutzerrechte / Login

Export-Funktion (PDF/CSV)

Erweiterte Standortkarte (Leaflet/Mapbox)

Automatischer Theme-Switch per Uhrzeit

KI-Prognosen (Weather-Based Forecasting)

 Screenshots
<img width="1392" height="917" alt="image" src="https://github.com/user-attachments/assets/d3e5c754-78d2-467e-8295-6cd33530a31a" />
<img width="1472" height="605" alt="image" src="https://github.com/user-attachments/assets/74bdfa8b-9cd6-43fc-a222-2c3525d76f89" />
<img width="978" height="837" alt="image" src="https://github.com/user-attachments/assets/44d103bd-dedb-4132-96f5-66eca7cac70e" />
<img width="1036" height="919" alt="image" src="https://github.com/user-attachments/assets/9534c457-e162-4828-a6ad-0f6d7744728e" />
<img width="1380" height="910" alt="image" src="https://github.com/user-attachments/assets/192b4136-2c1d-418b-b870-63c2842ded7f" />









Lizenz

MIT — frei für eigene Projekte und Weiterentwicklung.

Feedback

Wenn du Ideen oder Verbesserungsvorschläge hast – gerne melden!


---









## 📁 Projektstruktur

