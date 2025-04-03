- **Funktion:** Trennt Netzwerk- und Host-Teil einer IP-Adresse.
    
- **Beispiel:**
    
    - `192.168.1.5` mit `255.255.255.0` bedeutet:
        
        - **Netzwerkanteil:** `192.168.1`
            
        - **Hostanteil:** `5`
            
    - `192.168.1.5/26` (Subnetzmaske `255.255.255.192`) bedeutet:
        
        - 64 Hosts pro Subnetz (`2^6 - 2`).