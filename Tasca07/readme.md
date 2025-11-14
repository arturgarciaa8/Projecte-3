# T07: Instal·lant un servidor de noms

## Breu descripció

Després de l’exitosa experiència a nivell de formació, els nostres clients de Digicore estan tan satisfets amb la nostra feina que ens encarreguen la implantació des de zero dels seus serveis de DNS interns.

Actualment, l'agència fa servir adreces IP per accedir als seus servidors de desenvolupament, bases de dades i eines de gestió interna. Aquest mètode és ineficient i propens a errors:

- **Usabilitat deficient:** Els empleats han de memoritzar o buscar constantment adreces IP complexes (p. ex., 192.168.10.25).
- **Manteniment feixuc:** Si un servidor canvia la seva IP, cal notificar i actualitzar manualment la configuració a tots els equips i aplicacions que s'hi connecten.
- **Manca de professionalitat:** En un entorn professional, tots els serveis haurien de ser accessibles mitjançant noms fàcils de recordar.

Per tant, la nostra missió és implementar un Sistema de Noms de Domini (DNS) intern robust.  
L'objectiu és que els servidors i aplicacions de l'agència es puguin accedir utilitzant noms de domini amigables (p. ex., `bbdd.digicore.lan` o `wiki.digicore.lan`).

---

## El vostre repte

La recomanació com a consultora és utilitzar **BIND9**, l'estàndard de facto de servidor de noms a Linux, per la seva fiabilitat i flexibilitat.

La vostra missió serà **instal·lar i configurar un servidor DNS primari (màster)** amb BIND9 en un sistema Linux.  
Haureu de crear una **Zona Directa (Forward Zone)** i una **Zona Inversa (Reverse Zone)** per al domini privat de DigiCore, garantint que tant els noms es resolguin a IPs com les IPs es resolguin a noms.

Per fer una prova de concepte, usareu el domini:


