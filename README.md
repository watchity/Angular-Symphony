# Angular Symphony

La prova consistirà en posar en pràctica els coneixents d'Angular, TypeScript, HTML, Django, Python i bases de dades.

### Objectiu

A partir de la plantilla d'Angular del repositori, s'haurà de crear una pàgina que en entrar mostri un alfabet col·locat de manera horitzontal en què es puguin clicar totes les lletres.

En clicar una lletra, es farà una crida a l'api OpenOpus https://github.com/openopus-org/openopus_api/blob/master/USAGE.md per llistar tots els compositors que el seu nom comenci per la lletra seleccionada. Aquesta API és molt senzilla i no cal utilitzar cap mena de token o autenticitat.

Amb els resultats obtinguts s'haurà de generar una taula que mostri el retrat de cada compositor i un peu de foto amb cada nom.

L'usuari podrà clicar la foto o el nom de qualsevol compositor, el que farà que es mostri més informació seva, com l'època, data de naixement, data de mort i un parell d'obres. Aquesta informació pot ser mostrada com al desenvolupador li sembli més convenient, a una nova ruta, modificar la taula perquè aparegui la informació de manera més integrada, etc.

------

Per altra banda, s'haurà de preparar una petita API feta en Django i djangorestframework que reculli la informació de la quantitat de gent que ha sol·licitat la informació. És a dir, en el moment que des del frontend es demani més informació d'un compositor, s'haurà d'enregistrar la visita i emmagatzemar-ho en una base de dades (sqlite). Això servirà per poder afegir un comptador al frontend on es mostri quanta gent ha visitat cada compositor. A més, si hi ha un compositor de la taula que té més visites que la resta, se'l considerarà *trending* i s'haurà de destacar de la resta perquè es vegi a simple vista (estil lliure).

### Entrega

S'haurà de fer un fork d'aquest repositori i treballar a l'usuari personal de GitHub del desenvolupador. En aquell repositori es treballarà tota la part de frontend i simplement se'ns haurà de fer arribar una url. Per la part de backend s'haurà de fer o bé un altre repositori, o fer-nos arribar el codi en un .zip per correu electrònic.

### Utilitats

#### Com començar a utilitzar la plantilla d'Angular?

Tots aquests passos són completament opcionals i si el desenvolupador té qualsevol altra preferència ho podrà fer al seu gust.

1. Instal·lar nvm https://github.com/nvm-sh/nvm
2. Instal·lar la versió de node 20  `nvm install 20`
3. Clonar el repositori personal en què es treballarà i entrar a la carpeta.
4. Assegurar-se que s'utilitza la versió instal·lada `nvm use 20`
5. Instal·lar angular cli `npm install -g @angular/cli` o bé instal·lar totes les dependències amb `npm install`
6. Es recomana utilitzar Visual Studio Code i instal·lar l'extensió [https://marketplace.visualstudio.com/items?itemName=Angular.ng-template](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template)
7. Un cop fet tot això, només cal executar `ng serve` per poder servir l'aplicació a `http://localhost:4200/`

### Links útils

- Open Opus API: https://openopus.org/
- Django: https://www.djangoproject.com/
- djangorestframework: https://www.django-rest-framework.org/
- nvm: https://github.com/nvm-sh/nvm
- Angular: https://angular.io/
- RxJS: https://rxjs.dev/
