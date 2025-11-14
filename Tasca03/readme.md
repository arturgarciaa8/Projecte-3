# T03: Gestió flexible de discos (LVM i Espais d’emmagatzematge)

## Breu descripció

Un cop superada la fase de formació, ja esteu preparats per afrontar el repte dels nostres clients.  
El bufet d’advocats **Garriga i Associats**, un dels més prestigiosos de la ciutat, ha requerit els serveis de la nostra consultora. Gestionen una gran quantitat d’informació legal sensible, de manera que la **integritat**, la **disponibilitat** i la **facilitat de gestió** del seu emmagatzematge són essencials.

La direcció ha expressat la necessitat urgent de renovar els seus sistemes de servidors per garantir:
- Protecció davant fallades de disc  
- Possibilitat d’ampliar l’espai sense interrupcions  

Com a tècnics d’EverPia, heu de **dissenyar i documentar dues solucions d’emmagatzematge**:
- Una per servidors **Linux**  
- Una per servidors **Windows**

Aquestes solucions han de complir amb:
- Alta disponibilitat  
- Redundància  
- Escalabilitat  

Com que és una prova de concepte, la demostració es farà en **màquines virtuals** utilitzant sistemes operatius clients.

---

## 1. Part Linux: LVM amb Zorin OS

S’utilitzarà Zorin OS (o alternativa Linux) per demostrar **Logical Volume Manager (LVM)**.

### Requisits de la Implementació i Demostració

#### **Configuració inicial**
- Crear un **grup de volums (VG)** i un **volum lògic (LV)** amb un mínim de *dos discos de 10 GB*.  
- Formatar i muntar automàticament mitjançant `/etc/fstab`.

#### **Alta disponibilitat**
- Implementar un **mirall LVM (lvm_mirror)** per protegir davant fallada d’un disc.

#### **Instantànies (snapshots)**
1. Afegir **dos discos de 10 GB** al VG.  
2. Crear un volum `lvm_dades` amb el primer disc:  
   - Formatar-lo  
   - Muntar-lo  
3. Afegir arxius al volum (per exemple, imatges).  
4. Usar el segon disc per crear un snapshot (`lv_snapshot`).  
5. Documentar com **restaurar** el snapshot en cas de corrupció de dades.

#### **Escalabilitat**
- Ampliar el volum `lv_dades` utilitzant l’espai lliure del VG.

---

## 2. Part Windows: Espais d’emmagatzematge (Storage Spaces)

S’utilitzarà **Windows 11** per demostrar les configuracions d’Espais d’Emmagatzematge.

### Requisits de la Implementació i Demostració

#### **Configuració inicial**
- Crear un **Storage Pool** amb *tres discos de 10 GB*.

#### **Estudi de configuracions**
1. **Mirroring** (alta disponibilitat)  
   - Ús de dos discos  
   - Verificar redundància

2. **Parity**  
   - Ús dels tres discos  
   - Explicar eficiència de l’espai

3. **Mirall triple (triple mirror)**  
   - Afegir tants discos de 10 GB com calguin

#### **Demostració de la gestió**
- Mostrar l'estat dels discos i del pool  
- Documentar la gestió des de la consola de Windows (Storage Spaces Management)

---

## Com treballareu i què lliurareu?

- El treball es fa **en grup**.  
- Us dividireu en dos equips:
  - Equip Linux → LVM  
  - Equip Windows → Storage Spaces

### Procediment de treball

1. **Individual**:  
   - Preparar un *guió de la tasca*: comandes, documentació, passos.

2. **En parelles**:  
   - Realitzar la demostració pràctica de la vostra part.

3. **En grup**:  
   - Revisar la documentació final.  
   - Cada membre puja la documentació al seu repositori.

### Format del lliurament

Dins el projecte, crear la carpeta:




