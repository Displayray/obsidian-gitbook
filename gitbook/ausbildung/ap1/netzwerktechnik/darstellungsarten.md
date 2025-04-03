### **Logische vs. Physikalische Netzwerktopologie**

Ein **Netzwerk** kann auf zwei Arten dargestellt werden:

1. **Logische Topologie** → Datenfluss und Kommunikation
    
2. **Physikalische Topologie** → Physische Verkabelung und Geräteanordnung
    

---

### **1. Logische Netzwerktopologie**

📌 **Definition:**

- Beschreibt, **wie Daten im Netzwerk fließen**, unabhängig von der realen Verkabelung.
    
- Bestimmt **Kommunikationswege, Protokolle und Datenweiterleitung**.
    
- Wichtig für das **Routing und Switching**.
    

📌 **Beispiele:**

- **Bus-Topologie (logisch)** → Alle Geräte empfangen das gleiche Signal, aber nur das Zielgerät verarbeitet es.
    
- **Stern-Topologie (logisch)** → Daten laufen zentral über einen Switch, auch wenn physisch mehrere Kabel vorhanden sind.
    
- **Virtuelle Netzwerke (VLANs)** → Geräte können logisch verbunden sein, obwohl sie physisch getrennt sind.
    

---

### **2. Physikalische Netzwerktopologie**

📌 **Definition:**

- Beschreibt die **tatsächliche Anordnung der Geräte und Kabel** im Netzwerk.
    
- Wichtig für **Installation, Wartung und Fehlersuche**.
    
- Bezieht sich auf **physische Verbindungen (LAN-Kabel, Funkverbindungen, Router, Switches, Server etc.).**
    

📌 **Beispiele:**

- **Stern-Topologie (physikalisch)** → Alle Geräte sind direkt mit einem zentralen Switch verbunden.
    
- **Ring-Topologie (physikalisch)** → Geräte sind kreisförmig verkabelt.
    
- **Mesh-Topologie (physikalisch)** → Jedes Gerät ist mit mehreren anderen Geräten verbunden.
    

---

### **Zusammenhang:**

Ein Netzwerk kann **physikalisch als Stern, aber logisch als Bus** aufgebaut sein.  
➡ Beispiel: Ein **Ethernet-Switch-Netzwerk** sieht physikalisch aus wie ein Stern, aber die Daten fließen logisch wie ein Bus.

💡 **Wichtige Erkenntnis:**

- **Logische Topologie** ist entscheidend für **Datenübertragung und Netzwerktechnik**.
    
- **Physikalische Topologie** bestimmt die **tatsächliche Verkabelung und Hardwarestruktur**.