- **Funktion:** Übersetzt Domainnamen in IP-Adressen.
- Definition: Domain Name System
    
- **Beispiel:** `google.com → 142.250.185.206`

- Records
	- A Record - IPv4
	- AAA Record - IPv6
	- MX Record - Email Server
	- CNAME Record - Alias (domainname)
	- TXT Record - Text
    
- **DNS-Server:** `8.8.8.8` (Google), `1.1.1.1` (Cloudflare).

### **Grundlegende DNS-Struktur**

Das DNS ist wie eine Baumstruktur aufgebaut:

- **Root-Zone (`.`)** → Ganz oben in der Hierarchie
    
- **Top-Level-Domain (TLD) (`.com`, `.de`)** → Erste Ebene nach der Root
    
- **Second-Level-Domain (`example.com`)** → Vom Domaininhaber registrierte Adresse
    
- **Subdomains (`shop.example.com`)** → Untergeordnete Domains

### **Ablauf einer DNS-Anfrage**

### **1. Cache-Prüfung**

Der Client (z. B. Browser) prüft zuerst, ob er die IP-Adresse bereits im **lokalen Cache** hat. Falls ja, wird diese verwendet, ohne eine neue Anfrage zu senden.

### **2. Anfrage an den DNS-Resolver (meist vom Internetanbieter)**

Falls die IP-Adresse nicht im Cache ist, fragt der Client den **DNS-Resolver** (z. B. von Google `8.8.8.8` oder Cloudflare `1.1.1.1`).

### **3. Root-Nameserver (`.`) wird kontaktiert**

Falls der Resolver die IP nicht kennt, fragt er einen **Root-Nameserver** (es gibt 13 Root-Server-Gruppen weltweit).

### **4. Weiterleitung zur TLD-Nameserver (`.com`, `.de`, etc.)**

Der Root-Server antwortet mit einer Verweisung zum entsprechenden **Top-Level-Domain (TLD) Nameserver** (z. B. `.com`).

### **5. Weiterleitung zum autoritativen Nameserver**

Der TLD-Server verweist auf den **autoritativen Nameserver** der Domain (`example.com`). Dieser hält die endgültige IP-Adresse der Website.

### **6. Antwort an den Client**

Der Resolver speichert die IP-Adresse im Cache und gibt sie an den Client weiter. Der Client kann jetzt die Website aufrufen.

### **Caching und TTL (Time to Live)**

Damit das DNS-System schnell arbeitet, speichern verschiedene Systeme die IP-Adressen für eine bestimmte Zeit. Die **TTL (Time to Live)** gibt an, wie lange ein DNS-Eintrag zwischengespeichert wird, bevor er erneut abgefragt werden muss.