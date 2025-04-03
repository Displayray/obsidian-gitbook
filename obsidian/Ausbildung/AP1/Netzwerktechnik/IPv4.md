- **Aufbau:** 32-Bit-Adresse, aufgeteilt in 4 Oktette (z. B. `192.168.1.1`).
    
- **Öffentliche vs. private IPs:**
    
    - Private IPs: **Nicht direkt über das Internet erreichbar**
        
        - `192.168.x.x`
            
        - `10.x.x.x`
            
        - `172.16.x.x – 172.31.x.x`
            
    - Öffentliche IPs: **Im Internet sichtbar**
        
        - Werden von deinem Provider vergeben.
            
- **Subnetzmaske (Praxisbeispiel):**
    
    - IP-Adresse: `192.168.1.100`
        
    - Subnetzmaske: `255.255.255.0`
        
    - Netzwerkadresse: `192.168.1.0`
        
    - Host-Bereich: `192.168.1.1 – 192.168.1.254`