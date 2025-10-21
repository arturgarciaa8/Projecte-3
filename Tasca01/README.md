# 🧩 T01: Gestor de contrasenyes

## 🔎 Breu descripció

⚠️ **Alerta!!** EverPia ha estat atacada per ciberdelinqüents. La consultora on esteu de becaris ha patit una **fuita d’informació (data breach)** i informació confidencial sobre un projecte en desenvolupament està ara en mans de delinqüents que amenacen amb publicar-la si no es paga un rescat.

Aquesta situació ha generat una **gran alarma dins la companyia**, i s’ha creat un **comitè de crisi** per gestionar-la.  
La investigació interna ha revelat que **un dels comptes tècnics va ser compromès** a causa de l’ús d’una **contrasenya feble o reutilitzada**.

Com a resposta, la **Direcció Tècnica** ha emès una directriu:  
> Tot el personal tècnic ha de començar a utilitzar un **gestor de contrasenyes validat** per garantir l’ús de credencials úniques i robustes.

Se us encarrega la tasca d’avaluar les opcions i crear la documentació necessària per a la formació del personal.

---

## 🧠 Fase 1: Anàlisi i Justificació (Document d'Informe)

Heu de redactar un **informe tècnic** que justifiqui la decisió de la Direcció i compari les opcions disponibles.

### Contingut de l’informe:

#### 🔹 Introducció i Justificació
- Explicar per què les **contrasenyes febles o reutilitzades** són un risc crític per a l’empresa (atacs de diccionari, *credential stuffing*, etc.).
- Explicar la **funció d’un gestor de contrasenyes** per mitigar aquests riscos.

#### 🔹 Comparativa Tècnica
Realitzeu una taula comparativa entre les següents opcions:

| Eina | Tipus | Característiques principals |
|------|--------|-----------------------------|
| **Bitwarden** | Online / Núvol | Sincronització multi-dispositiu, xifratge *end-to-end*, accés fàcil i model freemium. |
| **KeePassX / KeePassXC** | Offline / Escriptori | Emmagatzematge local (fitxer `.kdbx`), independència del núvol, codi obert i portabilitat. |

#### 🔹 Avantatges i Inconvenients
Resumeix els **pros i contres** de cada model (online vs. offline) segons:
- Seguretat  
- Usabilitat  
- Continuïtat del negoci

#### 🔹 Recomanació
Concloeu l’informe escollint **l’eina més adequada** per al personal tècnic i **justifiqueu** la vostra elecció.

---

## 🧩 Fase 2: Guia d'Ús Tècnica (Manual Operatiu)

A partir de l’eina seleccionada (Bitwarden, KeePassX, etc.), creeu una **guia d’ús clara i visual**, amb captures de pantalla i instruccions pas a pas.

### Punts obligatoris:

#### ⚙️ Instal·lació i Configuració Inicial
- Descàrrega i instal·lació del programari.
- Creació de la **BBDD principal o compte mestre**.

#### 🔐 Generació de Contrasenyes Segures
- Com utilitzar el **generador de contrasenyes**.
- Paràmetres recomanats: longitud, caràcters especials, etc.

#### 💾 Exemples d'Ús i Emplenament Automàtic
- Desar credencials d’un compte de correu electrònic.
- Desar credencials d’una aplicació o servei web.
- Ús de l’**extensió del navegador** per emplenar automàticament les dades.

#### 🧱 Gestió de Còpies de Seguretat (Backup)
- Com fer una còpia de seguretat (`.kdbx` o exportació Bitwarden).
- Recomanacions: emmagatzemar la còpia **en una clau USB xifrada** o **al núvol de forma segura**.

---

## 📁 Lliurament

Aquesta és una **tasca individual**.  
Dins el repositori del projecte-3, creeu la carpeta:

