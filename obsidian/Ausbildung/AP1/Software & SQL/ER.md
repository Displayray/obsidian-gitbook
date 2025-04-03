Entitäten: Rechtecke
Beziehungen: Raute
Attribute: Oval

![[airport-chen-er-diagram-example.png]]

Wichtig hierbei sind die Kardinalitäten & Primärschlüssel Kennzeichnung

Beispiel

Entität: Kunde
Beziehung: erteilt
Entität: Auftrag
oder
Entität: Hersteller
Beziehung: stellt her
Entität: Reifen

Wichtig (Attribute nicht vergessen)

Kardinalitäten:
1:1 - 1 zu 1 beziehung
1:n - 1 zu vielzahl beziehung
n:m - vielzahl zu vialzahl beziehung


Und hier noch kurz die hässliche Min-Max-Notation

### Bedeutung der Notation:

- **MIN (Minimum)**: Gibt an, wie viele Entitäten einer Entität an einer Beziehung beteiligt sein müssen. Dies kann entweder 0 oder 1 sein.
    
- **MAX (Maximum)**: Gibt an, wie viele Entitäten einer Entität maximal an einer Beziehung beteiligt sein können. Dies kann eine Zahl wie 1 oder "N" (für viele) sein.
    

### Beispiel:

Stellen wir uns eine Datenbank vor, die **Personen** und **Bestellungen** enthält, und wir möchten die Beziehung zwischen ihnen beschreiben.

- Eine Person kann **keine oder viele Bestellungen** aufgeben.
    
- Eine Bestellung muss **genau einer Person** zugeordnet sein.
    

Die Beziehung zwischen **Personen** und **Bestellungen** wäre dann in der **MIN-MAX-Notation** folgendermaßen dargestellt:

- **Personen** → **Bestellungen**:  
    MIN = 0, MAX = N für **Personen** (eine Person kann 0 oder mehr Bestellungen haben)  
    MIN = 1, MAX = 1 für **Bestellungen** (eine Bestellung muss genau einer Person zugeordnet sein)
    

### Zusammenfassung der gängigen Kardinalitäten:

1. **1:1-Beziehung** (z.B., Ein Mitarbeiter hat genau einen Arbeitsplatz):
    
    - MIN = 1, MAX = 1 auf beiden Seiten.
        
2. **1:n-Beziehung** (z.B., Ein Kunde kann viele Bestellungen haben, aber jede Bestellung gehört nur zu einem Kunden):
    
    - MIN = 0, MAX = N auf der Seite der "vielen" Entität (z.B., Bestellungen)
        
    - MIN = 1, MAX = 1 auf der Seite der "einzelnen" Entität (z.B., Kunde).
        
3. **m:n-Beziehung** (z.B., Ein Schüler kann viele Kurse belegen und ein Kurs kann viele Schüler haben):
    
    - MIN = 0, MAX = N auf beiden Seiten der Beziehung.