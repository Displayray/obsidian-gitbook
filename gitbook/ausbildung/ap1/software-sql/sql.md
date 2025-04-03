Ja Datenbanken und so nh

### 1. **Datenbanken und Tabellen verwalten**

- **Datenbank erstellen**:  
    `CREATE DATABASE meine_datenbank;`
    
- **Datenbank auswählen**:  
    `USE meine_datenbank;`
    
- **Tabelle erstellen**:  
    `CREATE TABLE personen ( id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(100), alter INT, email VARCHAR(100) );`
    
- **Tabelle löschen**:  
    `DROP TABLE personen;`
    
- **Datenbank löschen**:  
    `DROP DATABASE meine_datenbank;`
    

---

### 2. **Daten manipulieren**

- **Daten einfügen**:  
    `INSERT INTO personen (name, alter, email) VALUES ('Max Mustermann', 30, 'max@example.com');`
    
- **Daten aktualisieren**:  
    `UPDATE personen SET alter = 31 WHERE name = 'Max Mustermann';`
    
- **Daten löschen**:  
    `DELETE FROM personen WHERE name = 'Max Mustermann';`
    

---

### 3. **Daten abfragen**

- **Daten auswählen**:  
    `SELECT * FROM personen;`  
    (Das `*` bedeutet, dass alle Spalten zurückgegeben werden.)
    
- **Daten mit bestimmten Spalten auswählen**:  
    `SELECT name, email FROM personen;`
    
- **Daten mit Bedingungen auswählen**:  
    `SELECT * FROM personen WHERE alter > 25;`
    
- **Daten sortieren**:  
    `SELECT * FROM personen ORDER BY name ASC;`  
    (Für absteigende Reihenfolge: `DESC`)
    
- **Daten gruppieren**:  
    `SELECT alter, COUNT(*) FROM personen GROUP BY alter;`  
    (Zählt, wie viele Personen jedes Alter haben.)
    
- **Daten mit Bedingungen und LIMIT**:  
    `SELECT * FROM personen WHERE alter < 30 LIMIT 5;`  
    (Zeigt nur die ersten 5 Datensätze an, die die Bedingung erfüllen.)
    

---

### 4. **Verknüpfung von Tabellen (JOIN)**

- **INNER JOIN** (nur übereinstimmende Datensätze):  
    `SELECT personen.name, bestellungen.bestell_id FROM personen INNER JOIN bestellungen ON personen.id = bestellungen.personen_id;`
    
- **LEFT JOIN** (alle Datensätze aus der linken Tabelle, auch wenn keine Übereinstimmung in der rechten Tabelle existiert):  
    `SELECT personen.name, bestellungen.bestell_id FROM personen LEFT JOIN bestellungen ON personen.id = bestellungen.personen_id;`
    

---

### 5. **Daten aggregieren**

- **COUNT**: Gibt die Anzahl der Datensätze zurück. Beispiel:  
    `SELECT COUNT(*) FROM personen;`
    
- **SUM**: Berechnet die Summe einer bestimmten Spalte. Beispiel:  
    `SELECT SUM(umsatz) FROM bestellungen;`
    
- **AVG**: Berechnet den Durchschnitt einer Spalte. Beispiel:  
    `SELECT AVG(alter) FROM personen;`
    
- **MAX / MIN**: Gibt den maximalen oder minimalen Wert einer Spalte zurück. Beispiel:  
    `SELECT MAX(alter) FROM personen;`  
    `SELECT MIN(alter) FROM personen;`
    

---

### 6. **String-Filtermethoden**

- **LIKE**: Wird verwendet, um nach einem Muster in einer Spalte zu suchen. Beispiel:  
    `SELECT * FROM personen WHERE name LIKE 'Max%';`  
    (Findet alle Namen, die mit "Max" beginnen.)
    
- **CONCAT**: Verbindet mehrere Strings zu einem. Beispiel:  
    `SELECT CONCAT(name, ' ', email) AS kontakt FROM personen;`  
    (Verbindet den Namen und die E-Mail-Adresse zu einer neuen Spalte „kontakt“.)
    
- **UPPER / LOWER**: Wandelt einen String in Groß- bzw. Kleinbuchstaben um. Beispiel:  
    `SELECT UPPER(name) FROM personen;`  
    (Gibt den Namen in Großbuchstaben zurück.)
    
- **SUBSTRING**: Gibt einen Teilstring eines Strings zurück. Beispiel:  
    `SELECT SUBSTRING(name, 1, 3) FROM personen;`  
    (Gibt die ersten drei Buchstaben des Namens zurück.)
    
- **TRIM**: Entfernt führende und nachfolgende Leerzeichen eines Strings. Beispiel:  
    `SELECT TRIM(name) FROM personen;`  
    (Entfernt Leerzeichen vor und nach dem Namen.)