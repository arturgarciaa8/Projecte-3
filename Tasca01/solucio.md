# T01: Gestor de contrasenyes — Artur Garcia

## Fase 1: Anàlisi i Justificació

### Introducció i Justificació
Les contrasenyes febles o reutilitzades són una amenaça greu per a la seguretat de les empreses.  
Permeten atacs com:

- **Diccionari:** provar combinacions comunes  
- **Credential stuffing:** usar contrasenyes filtrades d’altres webs  

Aquests atacs poden donar accés no autoritzat a dades crítiques, com ha passat a EverPia.

Per evitar-ho, cal usar un **gestor de contrasenyes**, que crea i guarda credencials úniques i segures de forma xifrada, reduint el risc d’errors humans i fuites d’informació.

---

### Comparativa Tècnica

| Característica | Bitwarden (Online) | KeePassXC (Offline) |
|----------------|--------------------|----------------------|
| **Seguretat** | Xifratge end-to-end (AES-256). | Xifratge fort (AES-256). |
| **Emmagatzematge** | Núvol segur o servidor propi. | Local (fitxer KDBX). |
| **Sincronització** | Automàtica entre dispositius. | Manual. |
| **Plataformes** | Web, app i extensions. | Windows, macOS, Linux. |
| **Codi i cost** | Open source, versió freemium. | 100% open source i gratuït. |
| **Facilitat d’ús** | Molt intuïtiu. | Més tècnic. |

---

### Avantatges i Inconvenients

#### **Bitwarden (Online)**  
**Avantatges:**  
- Sincronització automàtica i ús fàcil.  
- Compartició segura de contrasenyes.  

**Inconvenients:**  
- Depèn d’Internet i d’un servei extern.  

---

#### **KeePassXC (Offline)**  
**Avantatges:**  
- Privadesa total i sense dependències.  
- Gratuït i de codi obert.  

**Inconvenients:**  
- Sense sincronització automàtica.  
- Menys intuïtiu.  

---

### Recomanació
Es recomana utilitzar **Bitwarden** per la seva seguretat, facilitat d’ús i sincronització entre dispositius, ideals per al treball tècnic diari.

**KeePassXC** pot servir com a opció complementària en entorns desconnectats o d’alta privadesa.

Adoptar Bitwarden millorarà notablement la seguretat interna i evitarà futurs incidents de fuita d’informació.

---

## Fase 2: Guia d'Ús Tècnica (Manual Operatiu)
