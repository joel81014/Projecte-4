# Introducció
Molt bé, equip de consultors júniors, en el nostre projecte, ens trobem ara amb un requisit tècnic molt habitual per part dels nostres clients: la **centralització de dades en entorns Linux**.

---

## El Cas Client: DevOptimize Solutions
El nostre client, **DevOptimize Solutions**, és una petita *startup* de desenvolupament de programari que treballa exclusivament amb Linux. Tenen un problema crític: el seu codi font i els seus actius (documents de disseny, scripts) estan descontrolats. Cada desenvolupador té còpies locals, cosa que provoca errors de versió constants i una pèrdua d'eficiència brutal.

Ens han contractat per implementar un **servidor de fitxers centralitzat**. Atès que tot l'entorn és Linux, la solució nativa, més ràpida i eficient del sector és **NFS (Network File System)**.

> ⚠️ **Restricció clau:** El client ha insistit en que treballa sense un entorn d’autenticació centralitzada i que, de moment, no té previst fer aquest pas.

---

## Descripció de la tasca
Per mostrar al client com quedarà la solució proposada a partir de les seves demandes i poder mostrar també les limitacions, se t’encarrega fer una demostració del sistema.

* **Infraestructura:** Crearàs un servidor NFS (NFSv3) i un client Linux que consumeixi els recursos compartits.
* **Simulació d'entorn:** Hauràs de crear usuaris i grups per simular l'entorn del client.
* **Control d'accés:** Demostrar el control d'accés utilitzant les opcions d'exportació (`/etc/exports`) i els permisos del sistema de fitxers (`chmod`, `chown`).

🔗 **Repositori de la tasca a realitzar:** [https://github.com/SMX2n/Projecte04-NFS](https://github.com/SMX2n/Projecte04-NFS)

---

## Materials i links de suport
* **Material propi:** UD5. AA1. NFS. Disponible al Moodle del mòdul de *Sistemes Operatius en Xarxa*.
* **Ruiz, P. (2021, novembre 22).** *NFS (parte 1): Instalación en un servidor Ubuntu 20.04 LTS.* SomeBooks.es.  
  [https://somebooks.es/nfs-parte-1-instalacion-en-un-servidor-ubuntu-20-04-lts/](https://somebooks.es/nfs-parte-1-instalacion-en-un-servidor-ubuntu-20-04-lts/)
* **Ruiz, P. (2021, desembre 2).** *NFS (parte 2): Instalación en un cliente Ubuntu 20.04 LTS.* SomeBooks.es.  
  [https://somebooks.es/nfs-parte-2-instalacion-en-un-cliente-ubuntu-20-04-lts/](https://somebooks.es/nfs-parte-2-instalacion-en-un-cliente-ubuntu-20-04-lts/)
* **Network File System (NFS). (s. f.).** *Ubuntu Server.* [https://documentation.ubuntu.com/server/how-to/networking/install-nfs/](https://documentation.ubuntu.com/server/how-to/networking/install-nfs/)
