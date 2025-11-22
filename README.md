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




## 📁 Projektstruktur

