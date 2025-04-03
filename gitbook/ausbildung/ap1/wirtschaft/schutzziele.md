Die **Schutzziele der IT-Sicherheit** sind grundlegende Prinzipien, die den Schutz von Informationen und Systemen gewährleisten sollen. Sie sind essenziell für Unternehmen, Behörden und Privatpersonen, um Datenverluste, Manipulation oder unberechtigten Zugriff zu verhindern.

### **Die drei klassischen Schutzziele** (CIA-Triade):

1. **Vertraulichkeit (Confidentiality)**
    
    - Informationen dürfen nur von autorisierten Personen oder Systemen eingesehen werden.
        
    - Maßnahmen: Verschlüsselung, Zugriffskontrollen, VPNs, Firewalls.
        
2. **Integrität (Integrity)**
    
    - Daten dürfen nicht unbemerkt verändert oder manipuliert werden.
        
    - Maßnahmen: Hashing, digitale Signaturen, Prüfsummen, Backups.
        
3. **Verfügbarkeit (Availability)**
    
    - Systeme und Daten müssen für berechtigte Nutzer jederzeit zugänglich sein.
        
    - Maßnahmen: Redundanz, Lastverteilung, DDoS-Schutz, Notfallpläne.


## Beispiele

### **1. Vertraulichkeit (Confidentiality)**

📌 **Beispiel:** Online-Banking

- Beim Online-Banking müssen die Kontodaten und Transaktionen vor unbefugtem Zugriff geschützt werden.
    
- **Maßnahmen:** Verschlüsselung (z. B. TLS für HTTPS-Verbindungen), sichere Passwörter, Zwei-Faktor-Authentifizierung (2FA).
    

📌 **Beispiel:** Personalakten in Unternehmen

- Personalakten enthalten sensible Daten, die nur Personalabteilung und Geschäftsführung einsehen dürfen.
    
- **Maßnahmen:** Zugriffsrechte in der IT, verschlüsselte Datenbanken, sichere Speichersysteme.
    

---

### **2. Integrität (Integrity)**

📌 **Beispiel:** Software-Updates

- Eine Software-Aktualisierung darf während des Downloads oder der Installation nicht manipuliert werden.
    
- **Maßnahmen:** Hash-Werte zur Überprüfung, digitale Signaturen, kryptografische Prüfsummen.
    

📌 **Beispiel:** Datenbanken in Onlineshops

- Die Preisinformationen eines Produkts dürfen nicht von unbefugten Personen geändert werden, um z. B. aus einem 500€-Produkt ein 5€-Produkt zu machen.
    
- **Maßnahmen:** Transaktionsprotokolle, Zugriffskontrollen, regelmäßige Backups.
    

---

### **3. Verfügbarkeit (Availability)**

📌 **Beispiel:** Webshops während des Black Friday

- Ein Onlineshop muss auch bei hohem Traffic (z. B. Black Friday) erreichbar bleiben.
    
- **Maßnahmen:** Lastverteilung (Load Balancer), Server-Cluster, DDoS-Schutz.
    

📌 **Beispiel:** Notrufsysteme

- Ein Notrufsystem (z. B. 112) darf niemals ausfallen, da Menschenleben davon abhängen.
    
- **Maßnahmen:** Redundante Netzwerke, Notstromversorgung, Hochverfügbarkeits-Server.


## Maßnahmen: Beispiel Datei-Server

### **1. Maßnahmen zur Erhöhung der Vertraulichkeit:**

🔒 **Zugriffskontrollen:**

- **Benutzer- und Gruppenrechte** (Least Privilege-Prinzip: Jeder bekommt nur so viele Rechte wie nötig).
    
- **Multi-Faktor-Authentifizierung (MFA)** für Administratoren und sensible Daten.
    
- **IP-Adressfilter** für externe Zugriffe.
    

🔒 **Datenverschlüsselung:**

- **Verschlüsselte Übertragung** (z. B. SMB mit TLS, SFTP statt FTP).
    
- **Verschlüsselte Speicherung** (BitLocker, VeraCrypt oder EFS unter Windows).
    

🔒 **Logging & Überwachung:**

- **Protokollierung von Zugriffen** (Wer hat welche Datei geöffnet, bearbeitet oder gelöscht?).
    
- **SIEM-Systeme** (Security Information and Event Management) zur Anomalieerkennung.
    

---

### **2. Maßnahmen zur Erhöhung der Integrität:**

✔ **Schreibschutz & Versionskontrolle:**

- Aktivieren von **Read-Only-Modus** für kritische Dateien.
    
- **Versionierung aktivieren** (z. B. Snapshots, um unerwünschte Änderungen rückgängig zu machen).
    

✔ **Digitale Signaturen & Prüfsummen:**

- **Hash-Werte** für kritische Dateien generieren und regelmäßig überprüfen.
    
- **Signierte Dokumente** zur Sicherstellung der Echtheit und Unverfälschtheit.
    

✔ **Malware- & Ransomware-Schutz:**

- **Echtzeit-Scanner** für hochgeladene Dateien.
    
- **Schreibschutz für Systemdateien**, um Manipulation durch Schadsoftware zu verhindern.
    

---

### **3. Maßnahmen zur Erhöhung der Verfügbarkeit:**

⚡ **Redundanz & Backups:**

- **RAID-Systeme** für Ausfallsicherheit der Festplatten.
    
- **Regelmäßige Backups** (z. B. inkrementell, täglich, extern gespeichert).
    
- **Offsite-Backups** (Speicherung an einem anderen Standort für Notfälle).
    

⚡ **DDoS- & Netzwerkschutz:**

- **Firewalls & IDS/IPS** (Intrusion Detection & Prevention Systeme).
    
- **Lastverteilung (Load Balancer)** bei vielen Zugriffen.
    

⚡ **Notfall- & Wiederherstellungspläne:**

- **Disaster Recovery Plan** für den Ernstfall (z. B. nach Cyberangriffen).
    
- **USV (Unterbrechungsfreie Stromversorgung)** zum Schutz vor Stromausfällen.