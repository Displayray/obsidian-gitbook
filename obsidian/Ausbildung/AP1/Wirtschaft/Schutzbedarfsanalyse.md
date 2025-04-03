- **Wofür?** Bestimmt, wie schützenswert Daten oder Prozesse sind.
    
- **Drei Schutzklassen:**
    
    1. **Normal**: Keine großen Folgen (z. B. öffentliche Infos auf einer Webseite).
        
    2. **Hoch**: Schäden für das Unternehmen möglich (z. B. Kundenlisten).
        
    3. **Sehr hoch**: Existenzbedrohend (z. B. Finanzdaten, Passwörter).
        

### **Praxisbeispiel:**

Ein Online-Shop speichert **Kundendaten**. Diese müssen sicher gespeichert und gegen Hacker geschützt werden.

## Beispiele: Sommer 2023
![[Pasted image 20250403092056.png]]

Vertraulichkeit - sehr hoch -> Enthält sensible Daten der Kunden
Integrität - hoch -> Fehlerhafte bzw Manipulierte Daten führen zu falschen Bestellungen/Aufträgen wodurch es zu finanziellen Verlusten kommen kann
Verfügbarkeit - normal -> Ein Ausfall über 24h kann geduldet werden, außerdem, ist die Schadenshöhe gering.

### Noch eins
![[Pasted image 20250403093637.png]]
### **Prinzip der Schutzbedarfsanalyse**

Die Schutzbedarfsanalyse bewertet **Vertraulichkeit, Integrität und Verfügbarkeit** anhand möglicher Schäden bei Sicherheitsverletzungen.

### **Vorgehen:**

1. **Bestimmung der Schutzbedarfskategorien** für **Vertraulichkeit, Integrität und Verfügbarkeit**:
    
    - **Normal** 🟢 → Keine schwerwiegenden Schäden
        
    - **Hoch** 🟠 → Erhebliche Schäden für Unternehmen oder Betroffene
        
    - **Sehr hoch** 🔴 → Existenzbedrohende Schäden
        
2. **Analyse der möglichen Auswirkungen** eines Angriffs oder Ausfalls:
    
    - **Vertraulichkeit:** Wer darf die Daten sehen?
        
    - **Integrität:** Sind die Daten unverändert und korrekt?
        
    - **Verfügbarkeit:** Muss das System stets verfügbar sein?
        
3. **Zusammenfassung & Maßnahmenableitung**
    
    - Falls ein Bereich „hoch“ oder „sehr hoch“ eingestuft wird, sind **stärkere Sicherheitsmaßnahmen** erforderlich.
        

### **Beispiel für den Laptop mit Auftrags- und Kundenverwaltung**

- **Vertraulichkeit:** **Hoch bis sehr hoch**, da Kundendaten enthalten sind.
    
- **Integrität:** **Hoch**, da fehlerhafte Daten zu falschen Bestellungen führen könnten.
    
- **Verfügbarkeit:** **Hoch**, da Vertriebsmitarbeiter ständig darauf zugreifen müssen.
    

🔹 **Ergebnis:** Ein **hoher Schutzbedarf** ist wahrscheinlich. Maßnahmen wie Verschlüsselung, regelmäßige Backups und Zugriffsbeschränkungen sind wichtig.