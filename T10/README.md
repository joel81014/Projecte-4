# Introducció
Molt bé, equip. A la nostra consultora, **EverPia**, busquem constantment optimitzar els recursos dels nostres clients per reduir costos i simplificar la gestió. Un dels punts més caòtics en qualsevol oficina és la gestió d'impressores: drivers incompatibles, costos de tòner descontrolats i equips que no saben a quina impressora estan enviant la feina.

La solució professional és implementar un **Servidor d'Impressió Centralitzat**.

### El Cas Client: DevOptimize Solutions
DevOptimize Solutions ens ha demanat una proposta per centralitzar la impressió en tots els seus departaments, els quals utilitzen una barreja de clients Linux (**Zorin OS**) i servidors (**Ubuntu Server**).

---

## La Vostra Missió: La Prova de Concepte (PoC)
Abans de comprar impressores de xarxa cares, el client vol veure una **Prova de Concepte (PoC)** que demostri que un servidor Linux pot gestionar una impressora i compartir-la de manera transparent amb els clients Zorin.

Per simular la impressora de xarxa sense gastar en hardware, utilitzarem la impressora virtual `cups-pdf`. Aquesta eina actua com una impressora normal, però en lloc d'imprimir en paper, "imprimeix" el document en un fitxer PDF que desa al servidor. El vostre objectiu és configurar aquest escenari i demostrar que un client pot enviar una feina d'impressió al servidor.

### Escenari de Treball
Utilitzarem el mateix escenari de la PoC de NFS (podeu seguir usant les mateixes màquines):

* **Màquina 1 (Servidor):** Ubuntu Server configurat amb una interfície en NAT i una segona amb xarxa *Host-Only*.
* **Màquina 2 (Client):** Zorin OS (Desktop) amb la mateixa configuració de xarxa que el servidor.

---

## PoC (Prova de Concepte) — Passes a seguir

1. [ ] **Instal·lació de CUPS** al servidor.
2. [ ] **Instal·lar la impressora virtual** (`cups-pdf`).
3. [ ] **Configuració de l’administració de CUPS** i permetre que CUPS escolti per totes les interfícies.
4. [ ] **Compartir la impressora** usant el navegador i el frontal web de CUPS.
5. [ ] **Afegir la impressora** en el client Zorin OS.
6. [ ] **Fer una prova d'impressió** de diversos documents.
7. [ ] **Comprovar al servidor** com s’han generat els arxius PDF corresponents als treballs impresos.

> 📝 **Requisit de lliurament:** Cal documentar les comandes utilitzades (tal com s’ha explicat a la tasca PDF) i incorporar les captures de pantalla necessàries per demostrar el correcte funcionament de la prova.

---

## Materials i links de suport
* **Material propi:** UD5. AA1. CUPS. Disponible al Moodle del mòdul de *Sistemes Operatius en Xarxa*.
* **J.B. Alex Mantich. (2024, 15 febrer).** *Instalación de servidor de impresión en cups para linux* [Vídeo]. YouTube.  
  [https://www.youtube.com/watch?v=FNwSTrOSgZQ](https://www.youtube.com/watch?v=FNwSTrOSgZQ)
* **Canonical.** *Network File System (NFS).* Ubuntu Server Documentation.  
  [https://documentation.ubuntu.com/server/how-to/networking/install-nfs/](https://documentation.ubuntu.com/server/how-to/networking/install-nfs/)
* **R00t (2025, 25 abril).** *How To Install CUPS Print Server on Ubuntu 24.04 LTS.* Idroot.  
  [https://idroot.us/install-cups-print-server-ubuntu-24-04/](https://idroot.us/install-cups-print-server-ubuntu-24-04/)
