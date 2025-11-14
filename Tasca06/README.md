# T06: Fonaments del servei DNS

## Breu descripció

Com a membres cada cop més integrats de l’equip tècnic d’EverPia, se us presenta un nou repte.  
El vostre client, **DigiCore**, una empresa de màrqueting digital, està experimentant errors de connectivitat en certes aplicacions.  
L’equip tècnic sospita que la causa pot ser una **resolució de noms (DNS)** incorrecta o lenta.

La vostra missió és realitzar una **auditoria teòrica i pràctica del servei DNS**, amb l’objectiu de formar el personal del client i oferir eines de diagnosi ràpides.

---

# FASE TEÒRICA — Sessió formativa

Com a part de la formació, haureu d’elaborar material formatiu sobre els conceptes fonamentals del DNS.  
Les sessions prèvies proporcionades pels directors tècnics són la base obligatòria.

## Conceptes que haureu d’explicar

### **1. Jerarquia i estructura del DNS**
- Estructura en arbre  
- Nivells: **Root > TLDs > Domini de segon nivell**

### **2. Procés de resolució**
- Consulta **iterativa**  
- Consulta **recursiva**  
- Funció d’un **Root Server**  
- Funció d’un **servidor autoritatiu**

### **3. Tipus de zones**
- **Zona directa**  
- **Zona inversa**  
- **Zona primària**  
- **Zona secundària**

### **4. Tipus de registres DNS (Records)**
- **A**  
- **CNAME**  
- **MX**  
- **NS**  
- **SRV**

### **5. Conceptes essencials**
- **Resposta autoritativa**  
- **Time To Live (TTL)**  
- **Start of Authority (SOA):** informació crítica (correo de l’admin, número de sèrie…)  
- **Reenviadors:** condicionals i incondicionals  
- **Resolució local:** mecanismes sense servidor  
- **mDNS (Multicast DNS)**  

---

## Activitat teòrica
Un cop dominats els conceptes, cal preparar una:

🎥 **Píndola formativa (vídeo de 10–15 minuts)**  
Explicant de manera breu i clara tots aquests punts.

---

# FASE PRÀCTICA — Diagnosi de Noms (Auditoria amb CLI)

Heu de demostrar l’ús de les principals eines de diagnosi DNS en:

- **Linux / macOS** → `dig`  
- **Windows** → `nslookup`  

La pràctica es realitzarà en un equip **Zorin OS** amb dues interfícies:

- NAT  
- Adaptador pont (amb IP configurada segons indicacions)

---

# A. Diagnosi Avançada amb *dig* (Linux / macOS)

### **Comanda 1: Consulta bàsica de registre A**

