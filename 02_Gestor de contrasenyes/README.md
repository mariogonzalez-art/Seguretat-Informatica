### Fase 1: Anàlisi i Justificació (Document d'Informe)

Heu de redactar un informe que justifiqui tècnicament la decisió de la Direcció i comparin les opcions. Aquest informe ha d'incloure:

1. Introducció i Justificació:

- Explicació de perquè les contrasenyes febles o reutilitzades són un risc crític per a l'empresa (atac de diccionari, credential stuffing, etc.)

<br>

Utilitzar claus fàcils o repetir la mateixa contrasenya a tot arreu posa l'empresa en un risc molt alt ja que els programes automàtics poden fer atacs de diccionari provant paraules comunes fins a encertar la contrasenya. També, si filtren la contrasenya d'un empleat en una altra web, els hackers aprofitaran aquestes dades per intentar entrar als sistemes de la nostra organització mitjançant el farciment de credencials.

<br>

- La funció crucial d'un gestor de contrasenyes per mitigar aquests riscos.

<br>

Un gestor de contrasenyes serveix per crear claus llargues i úniques sense haver de recordar-les totes. També ens protegeix del phishing i manté totes les credencials guardades de forma segura sota una sola contrasenya mestra.

<br>

2. Comparativa Tècnica: Realitzeu una taula comparativa detallada entre:

- Bitwarden (Alternativa Online / Núvol): Analitzeu la sincronització, el model de seguretat (xifratge end-to-end), la facilitat d'accés des de múltiples dispositius i el cost/model freemium.
- KeePassX / KeePassXC (Alternativa Offline / Escriptori): Analitzeu l'emmagatzematge local de l'arxiu (KDBX), la independència del núvol, el model open source i la portabilitat de l'arxiu.

| Característica | Bitwarden (núvol) | KeePassXC (local) |
|---|---|---|
| Sincronització | Automàtica entre dispositius. | Manual o amb serveis externs. |
| Model de Seguretat | Xifratge d'extrem a extrem. | Base de dades xifrada amb AES-256 o altres algoritmes compatibles. |
| Facilitat d'accés | Ordinadors, mòbils i navegadors. | Cal disposar del fitxer de contrasenyes compatibles. |
| Emmagatzematge | Núvol amb dades xifrades. | Fitxer local **.kdbx**. |
| Dependència del núvol | Sí, per a la sincronització habitual. | No, funciona sense Internet. |
| Cost | Versió gratuïta i plans de pagament. | Gratuït. |
| Portabilitat | Accés des de diferents dispositius amb el mateix compte. | El fitxer es pot copiar a un USB o transferir a altres dispositius. 

3. Avantatges i Inconvenients: Resumiu els principals pros i contres de cada model (online vs. offline) des del punt de vista de seguretat, usabilitat i continuïtat del negoci.

### Bitwarden (Online / Núvol)

**Avantatges:**
- Sincronitza les contrasenyes automàticament.
- Utilitza xifratge d'extrem a extrem per protegir les dades.
- És fàcil d'utilitzar.

**Inconvenients:**
- Depèn del servei al núvol per sincronitzar les dades.
- Cal protegir bé el compte principal.
- Algunes funcions són de pagament.

### KeePassXC (Offline / Local)

**Avantatges:**
- Les contrasenyes es guarden localment i no depenen del núvol.
- És gratüit.
- Es pot utilitzar sense connexió a Internet.

**Inconvenients:**
- La sincronització entre dispositius és més complicada.
- Si es perd o es fa malbé el fitxer sense tenir una còpia de seguretat, es poden perdre totes les contrasenyes.
- Requereix més gestió manual i pot ser menys còmode per treballar en equip.

4. Recomanació: Concloeu l'informe escollint l'eina que considereu més adequada per al personal tècnic de l'empresa i justifiqueu la vostra elecció.

*La meva recomanació és utilitzar Bitwarden ja que utilitza xifratge d'extrem a extrem.*

### Fase 2: Guia d'Ús Tècnica (Manual Operatiu)

Utilitzant l'eina que heu seleccionat a la Fase 1 (Bitwarden, KeePassX, o similar), heu de crear una Guia d'Ús per a l'Equip Tècnic. Aquesta guia ha de ser clara i basada en captures de pantalla i instruccions pas a pas.

La guia ha de cobrir els següents punts obligatoris:

1. Instal·lació i Configuració Inicial: Descàrrega, instal·lació i creació de la BBDD principal o compte mestre.
2. Generació de Contrasenyes Segures: Explicació de com utilitzar el generador de contrasenyes de l'eina (paràmetres, longitud, caràcters especials).
3. Exemples d'Ús i Emplenament Automàtic:
   - Com desar una credencial d'un compte de correu electrònic.
   - Com desar una credencial d'una aplicació o servei web.
   - Com fer servir l’extensió del navegador per emplenar automàticament les dades.
4. Gestió de Còpies de Seguretat (Backup):
   - Explicació detallada de com fer una còpia de seguretat de l'arxiu de contrasenyes (KDBX en KeePass o Exportació en Bitwarden).
   - Recomanació de la millor pràctica per emmagatzemar aquesta còpia de seguretat de forma segura (clau USB xifrada o emmagatzematge xifrat al núvol).