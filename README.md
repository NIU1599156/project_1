# Pràctica 1: Fonaments d'Enginyeria
## Nom i NIU de l'equip de pràctiques
- Ivan Peñarando Martínez / **NIU**: 1599156
- Jan Naverrete Santos / **NIU**: 1571232 
- Isaac Pascual Mauriz / **NIU**: 1597521

## Part-A de la pràctica

La pràctica Oscars es basa en l'anàlisi, tria i organització de les diverses dades que ens proporcionen sobre els guanyadors dels Oscars des de l'any 1928 fins al 2016. En aquestes taules estan organitzats per any tots els guanyadors. Els valors de camps que ens proporcionen són el nom i cognoms, l'edat, l'any que va guanyar i el nom de la pel·lícula a la qual van ser premiats.

Amb totes aquestes dades se'ns demana que creem un programa amb diverses opcions, el qual cada opció donarà a l'usuari una organització de les dades específica de cada apartat. Per exemple, si l’usuari vol saber qui va guanyar l’any 1995, el programa donarà els resultats organitzats i ben estructurats d’aquesta cerca.

### Problemes sorgits
El problema més notable que hem tingut ha estat aconseguir una bona organització dels apartats i subapartats, ja que era la primera vegada que treballàvem amb GitHub. En un principi se'ns van acumular branques innecessàries o repetides, per la qual vam haver de tornar-ho a fer de nou. A la primera sessió de pràctiques, per exemple, vam començar fent cadascú una opció (menú, opció-1 i opció-2) atès que no sabíem molt bé el funcionament de GitHub, i per això a la segona sessió vam haver de començar de nou.

### Com executar
1. Entrem a la carpeta de la pràctica i executem el programa amb una de les següents comandes:
```
./oscars.sh 
bash oscars.sh 
```
2. Sortirà el següent menú:
```
--------------------------------------------------------- 
Base de Dades d’actors i actrius guanyadors/es de l’Oscar
--------------------------------------------------------- 
  1. Històric d’Oscars.
  2. Qui va guanyar ...?
  3. Ets un Expert?
  4. Altes, baixes i modificacions.
  0. Sortir. 
Selecciona una opcio (0-4): 
```
Aquest et demana que introdueixis un número de l'1-4. Si introdueixes un nombre fora del rang et sortirà un missatge d'error i després de 5 segons et tornarà al menú. Si introdueixes 3 o 4 sortirà un missatge de "En desenvolupament".

3. Si introdueixes un 1, et sortirà un nou menú:
```
--------------------------------------------------
              Històric d'Oscars                   
--------------------------------------------------
1.1 Mostrar històric d'Oscars a millor actor (alfabètic).
1.2 Mostrar històric d'Oscars a millor actriu (edat).
1.3 Mostrar històric d'Oscars (actors/actrius).
Selecciona una opcio (1-3): 
```
Aquest tornarà a demanar que introdueixis un nombre entre 1-3. Si introdueixes un nombre fora de rang et donarà un missatge d'error i et demanarà un nombre fins que introdueixis un dins del rang. Si introdueixes: 
- un 1 mostrarà l'històric d'Oscars a millor actor ordenats alfabèticament pel nom dels actors. 
- un 2 mostrarà l'històric d'Oscars guanyats per actrius ordenats per l'edat de l'actriu. 
- un 3 mostrarà l'històric d'Oscars guanyats per actors i actrius ordenats per l'any de l'Oscar.

Després de mostrar la informació demanada tornarà al menú "Base de Dades d’actors i actrius guanyadors/es de l’Oscar" quan premis qualsevol botó.

4. Si al menú "Base de Dades d’actors i actrius guanyadors/es de l’Oscar" introdueixes un 2 et sortirà el següent menú:
```
--------------------------------------------------
               Qui va guanyar ...?                
--------------------------------------------------
2.1 Mostrar l’actor i l'actriu que van guanyar un any determinat.
2.2 Mostrar els Oscars a millor actriu guanyats per una actriu determinada.
2.3 Mostrar els Oscars a millor actriu o actor que ha obtingut una pel·lícula determinada.
Selecciona una opcio (1-3): 
```
Et demana de cop que introdueixis un nombre de l'1 al 3. Si introdueixes un nombre fora de rang et donarà un missatge d'error i et demanarà un altre cop el nombre fins que escriguis un nombre dins del rang. Si introdueixes: 
- un 1 et demanarà que introdueixis un nombre entre 1928-2016. Si introdueixes un nombre fora de rang et sortirà un missatge d'error i et tornarà a demanar un altre cop. Quan introdueixis un nombre dins de rang, et mostrarà el guanyador i la guanyadora de l'Oscar d'aquell any amb tota la informació de les pel·lícules guanyadores. 
- un 2 et demanarà que introdueixis el nom d'un/a actor/actriu. Si introdueixes el nom d'una actriu amb un o més Oscars, et mostrarà tots els Oscars que ha obtingut aquella actriu, així com tota la informació d'ells (pel·lícula, any...). Si introdueixes algun nom que no coincideix amb cap guanyadora d'Oscar et sortirà un missatge d'error i et demanarà un altre nom. Per facilitar a l'usuari, si escrius el nom de l'actriu en minúscula, el programa també la reconeixerà sense problemes. 
- un 3 et demanarà el nom d'una pel·lícula. Si introdueixes el nom d'una pel·lícula amb actors/actrius guanyadors/es d'Oscar, et donarà l'any de la pel·lícula i l'actor i/o actriu guanyador/s d'aquella pel·lícula en concret, així com les edats. Si introdueixes un nom d'una pel·lícula amb actors no guanyadors d'Oscar o inventat et sortirà un missatge d'error i et demanarà un altre nom. Per facilitar a l'usuari, si escrius el nom de la pel·lícula en minúscula, el programa també el reconeixerà sense problemes.

### Comandes utilitzades
Les comandes que hem utilitzat han estat sobretot: llegir i escriure funcions amb echo, els diversos bucles fets amb while així com més d’un case per poder esquematitzar les diverses opcions molt més eficientment. També hem utilitzat l’eina de comandes de cercat i estructuració **AWK**, la qual ens ha servit de gran ajuda a l’hora de buscar informació precisa en un document de grans dimensions. En conjunt i harmonia amb l’AWK també hem aplicat comandes com grep, tail, head, sed… també amb el mateix propòsit de cerca.

### Conclusions
Les conclusions de la pràctica són les següents; aquesta pràctica ha tingut una bona corba d’aprenentatge per part de tots, ja que com hem dit anteriorment, era la primera vegada que ens enfrontàvem a un projecte de git, grupal i compartit en el núvol. No obstant ens hem pogut defensar correctament i hem assolit els apartats que se'ns demanava.

