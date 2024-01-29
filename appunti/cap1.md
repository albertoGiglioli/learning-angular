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

Per vedere tutti i comandi disponibili: *ng help*

I comandi più comuni:
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

Guida e tips per eseguire gli aggiornamenti ad angular in questo [link](https://update.angular.io)

## Creating a new project
*Ng new nome-app* per creare un progetto nuovo

Dentro alla cartella del progetto saranno presenti varie cartelle e file di configurazione che CLI ha bisogno per fare 
la build, testare e pubblicare l'app:
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


## Structure on an angular application
Dentro la cartella src sarà presente:
- app: contiene tutti i file dell'applicazione relativi ad angular
- assets: contiene gli asset static come font, immagini e icone
- favicon.ico: l'icona mostrata nella tab del browser, accanto al titolo della pagina
- index.html: la pagina main html dell'applicazione
- main.ts: entry point principale dell'applicazione
- style.css o scss o sass (scelto alla creazione): questo css è applicato globalmente all'applicazione. l'estensione di
questo file dipende dal formato stylesheet che è stato scelto alla creazione

L'applicazione angular che è stata creata automaticamente dalla CLI contiene i seguenti file:
- app.component.css
- app.component.html
- app.component.spec.ts
- app.component.ts
- app.module.ts
- app-routing.module.ts

## Components
## Modules
## Template syntax
## VS code tooling
## Angular language service
## Angular snippets
## Nx Console
## Material icon theme
## EditorConfig
## Angular Evergreen
