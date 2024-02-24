# ReversoContextPPC Client

> Il traduttore Reverso Context per l'architettura PPC e Intel

## Informazioni

Questa applicazione è un esercizio di stile nella programmazione su macchine e sistemi più datati rispetto agli attuali. Il programma è stato scritto sull'ultima versione di Xcode supportata dal sistema Mac OS X 10.5, eseguita su un [PowerMac G4 di prima generazione](https://it.wikipedia.org/wiki/Power_Mac_G4). Nella costruzione su Interface Builder ho utilizzato molti degli elementi grafici forniti da Cocoa, cercando di mantenere una linea grafica che non si scostasse dallo stile Macintosh. Nella costruzione delle strutture mi sono rifatto alle guide incluse nella versione di Xcode e ho cercato di rimanere più vicino possibile agli approcci logici suggeriti dalla documentazione.

## Implementazione

Cercando questa convergenza tra l'attuale e il non, ho voluto portare il servizio di traduzione Reverso su questa macchina che altrimenti non sarebbe stata in grado di  accedervi. Oltre alla mancanza dei certificati SSL nativi per la navigazione di siti web HTTPS, arginabile con l'uso di certi browser come [TenFourFox](https://github.com/classilla/tenfourfox), il caricamento e l'uso di pagine complesse avrebbe comunque impedito una navigazione agevole all'utente.

Ho creato un bridge, eseguibile su un computer in grado di lavorare con le API di Reverso, capace di elaborare le risposte e le richieste e inviare i dati ottenuti, tramite la rete LAN, al computer che li ha richiesti. Maggiori infomazioni sulla [pagina del progetto](https://github.com/francescomattiussi/ReversoContextPPCServer?tab=readme-ov-file).

L'ultima compilazione dell'applicazione si data a giugno 2021 su un sistema PPC, questa build si trova nella sezione delle releases. 

## To-do

Nonostante il mantenimento della repository non sia più attivo, di seguito i punti ancora mancanti nello sviluppo del progetto.

| Stato | Attività | Completamento |
| :---: | -------- | :-----------: |
| ⏸️ | Implementare lo spinner in basso | |
| ⏸️ | Controllo delle eccezioni nella barra di ricerca (testo vuoto) | |
| ⏸️ | Implementare la traduzione singola | |
| ⏸️ | Provare il dropdown menu con i search suggestions | |
| ⏸️ | Pensare a cosa mettere nel drawer | |
| ✅ | Implementare lo switch delle view nelle impostazioni | 04-06-2021 |
| ✅ | Testare con pulsanti normali | 04-06-2021 |
| ✅ | Aggiungere gli elementi alla barra, icone impostate | 04-06-2021 |
| ⏸️ | Far attivare le icone nella barra ||
| ⏸️ | Collegare le azioni alla barra ||
| ⏸️ | Sistemare le altezze delle viste ||
| ✅ | Rendere la toolbar completamente funzionante | 07-06-2021 |
| ✅ | Salvare negli user defaults e fare il retrieving dei parametri all'avvio delle impostazioni | 07-06-2021 |
| ✅ | Eseguire richieste con indirizzo IP impostato nelle impostazioni | 07-06-2021 |
| ✅ | Implementare lo spinner | 07-06-2021 |
| ⏸️ | Sistemare altezze impostazioni ||
| ⏸️ | Lato server, implementare login con account reverso ||
| ⏸️ | Lato server, errore di responso quando si verificano gli errori di troppe richieste ||
