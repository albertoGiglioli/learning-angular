# Building your first Angular application

## Cross-platform
Le applicazioni angular possono essere lanciate su diverse piattaforme: web, server, desktop e mobile.

- Angular è nativo solamente solo sul web perché è un framework JavaScript 
- **Angular Universal**: renderizza applicazioni angular lato server
- **Angular Service Worker**: abilita applicazioni angular al lancio come **PWA** (Progressive Web Application)
- **Ionic FrameWork**: permette di costruire applicazioni mobile usando angular

## Tooling

- **Angular CLI**: un interfaccia command-line che ci permette di lavorare con progetti angular, 
dalla creazione al rilascio
- **Angular DevTools**: un'estensione browser che ci abilita il debug e profila application angular dal comfort del
nostro browser

## Installing the angular CLI
*npm install -g @angular/cli*

- install o i per installare un pacchetto
- -g indica che il pacchetto sarà installato sul sistema globalmente
- con @angular/cli installerà l'ultima versione stabile (**lst**), per installare una versione precisa @v
es: @angular/cli@17

## CLI commands
La cli è un tool che automatizza specifici task durante lo sviluppo.
La sintassi è *ng command [options]*

per vedere tutti i comandi disponibili: *ng help*

i comandi più comuni:
- new: crea un nuovo angular cli workspace da zero, alias n
- build: compila un'applicazione angular e ritorna i file generati in una cartella predefinita, alias b
- generate: crea nuovi file che comprendono un'applicazione angular, alias g
- serve: costruisce un'applicazione angular e la serve usando un pre-configurato server web, alias s
- test: lancia i test di unità di un'applicazione angular, alisa t
- deploy: distribuisce un'applicazione angular su un provider web-hosting, si possono scegliere da una collezione di 
provider inclusi nel CLI
- add: installa una libreria angular nell'applicazione
- completion: abilita l'auto-completamento per i comandi del CLI attraverso il terminale
- update: aggiorna un'applicazione angular all'ultima versione di angular

guida e tips per eseguire gli aggiornamenti ad angular in questo [link](https://update.angular.io)

## Creating a new project
*ng new nome-app* per creare un progetto nuovo

Dentro alla cartella del progetto saranno presenti varie cartelle e file di configurazione che CLI ha bisogno per 
buildare, testare e pubblicare l'app:
- node_modules: include i pacchetti npm necessari per lo sviluppo e lancio dell'app
- src: contiene i file sorgente dell'app
- .gitignore: file ignorati da git
- angular.json: il file di configurazione principale della workspace (cartella nome-app)
- package.json e package-lock.json: fornisce definizioni dei pacchetti di npm, con le loro versioni esatte, le quali 
sono necessarie per lo sviluppo, test e lancio dell'app
- README.md
- tsconfig.app.json: configurazione di typescript che è specifica per l'app
- tsconfig.json: configurazione di typescript che è specifica per la workspace
- tsconfig.spec.json: configurazione di typescript che è specifica per unit test

