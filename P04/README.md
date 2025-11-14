# P04: Documentació servidor DNS

## Breu descripció

Molt benvinguts a la vostra nova tasca, consultors!

Com a membres de l'equip de sistemes d'EverPia, us heu enfrontat al repte de configurar un servidor de noms com a prova de concepte pel nostre client Digicore, però ara mateix el resultat de la vostra feina es troba en una màquina virtual.

L’objectiu és poder **publicar aquestes configuracions a GitHub**, de manera que qualsevol tècnic pugui replicar el servidor simplement descarregant els arxius i reiniciant el servei al servidor Linux triat.

---

# Fase 1: Preparació de la Connectivitat i Extracció dels Arxius

## Pas 1.1: Configuració de la Interfície Host-Only

- Afegir una **segona interfície de xarxa** a la màquina virtual Ubuntu Server en mode **Host-Only**.
- Configurar i activar la interfície.
- Comprovar la connectivitat entre la màquina virtual i la màquina física.

---

## Pas 1.2: Còpia Segura dels Fitxers Clau amb SCP

Un cop establerta la connectivitat Host-Only, utilitzareu el protocol **SCP (Secure Copy Protocol)**, inclòs amb SSH, per transferir els fitxers de configuració a la màquina física.

Fitxers a copiar:

- `/etc/bind/named.conf.options`
- `/etc/bind/named.cof.local`
- Arxius de zones de `/etc/bind/zones`

Per copiar els arxius al PC, obriu un terminal i executeu la comanda `scp`.

*(El punt al final de la comanda indica que es copiaran al directori actual de la màquina física.)*

---

# Fase 2: Integració a GitHub

## Pas 2.1: Crear carpeta i arxiu `README.md`

- Crear la carpeta:


