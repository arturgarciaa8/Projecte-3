# T04: Serveis de directori — LDAP

## Breu descripció

Innovatech, una start-up tecnològica emergent, està creixent molt ràpidament i pateix un **caos en la gestió d’usuaris i accessos**.

Actualment:

- Cada servei intern (servidor de fitxers, wiki, etc.) té la seva **pròpia base de dades** d’usuaris i contrasenyes.  
- Els ordinadors clients utilitzen **autenticació local**.

Això provoca problemes crítics:

### **1. Ineficiència Operativa**
Crear o eliminar un empleat implica fer canvis en múltiples sistemes.

### **2. Risc de Seguretat**
Els usuaris sovint **reutilitzen contrasenyes** entre serveis per no oblidar-les.

### **3. Manca d’Escalabilitat**
A mesura que l'empresa creix i incorpora nous serveis, el model actual és totalment insostenible.

---

## Solució proposada

El CEO d’Innovatech ha contactat EverPia per implementar una solució d’autenticació **centralitzada**.

La proposta és desplegar **OpenLDAP** (*Lightweight Directory Access Protocol*), ja que és:

- Robust  
- De codi obert  
- Perfecte per entorns amb ordinadors GNU/Linux (com Innovatech)  

---

## Objectiu de la tasca

La vostra missió és **implementar i configurar un servidor OpenLDAP** en un sistema Linux.

Això inclou:

### **1. Instal·lar el servei**
Desplegar el servidor OpenLDAP i eines relacionades.

### **2. Configurar el domini base**
Definir:
- `dc=empresa`
- `dc=local`  
o el domini indicat al plec tècnic.

### **3. Crear la jerarquia del directori**
Afegir les unitats organitzatives (OU):
- `ou=Users`
- `ou=Groups`
- (Les que especifiqui el document tècnic)

### **4. Integrar usuaris i grups**
Afegir-los al directori amb:
- Atributs LDAP correctes  
- Estructura ben definida (UID, GID, SN, CN...)

### **5. Configurar un equip client**
El client GNU-Linux ha d’autenticar usuaris **a través del directori LDAP**.  
S’anirà configurant:
- `sssd` o `nslcd`
- PAM  
- NSS  
Segons el procediment especificat.

---

## Documentació i plec tècnic

Tota la feina exacta a desenvolupar està detallada al:

➡️ **Plec de condicions tècniques**  
(Disponible al Moodle)

És imprescindible seguir-lo punt per punt.

---

## Material de classe (Moodle)

- **UD04.AA1** — Serveis de Directori  
- **UD04.AA2** — Instal·lació OpenLDAP  
- **UD04.AA3** — Configuració del directori  
- **UD04.AA5** — Afegir un client al directori

