### <span style="color:red"> COPIA LA REPOSITORY DI QUARTZ. </span>
Apri il terminale ed esegui il seguente comando attraverso il quale si scarica la repository "quartz.git" e la si salva localmente nel computer nella cartella "scegli_nome_cartella" che puoi rinominare come preferisci:

	git clone https://github.com/jackyzha0/quartz.git scegli_nome_cartella

### <span style="color:red"> INSTALLA LE LIBRERIE. </span>

Quartz è un progetto Node e ha bisogno di altre librerie per funzionare. 
Cambia la directoy entrando nella nuova cartella dove hai copiato la repository di git:

	cd scegli_nome_cartella

Se hai bisogno di altri approfondimenti su come muoverti tramite terminale ecco un link: [[COMANDI DI MOVIMENTO]]. 

Usa questo comando per installare le librerie:

	npm i

### <span style="color:red"> INIZIALIZZA QUARTZ. </span>

Crea un nuovo progetto di quartz, usa il seguente comando:

	 npx quartz create

Ti verranno proposte 3 opzioni:

	 - Empty Quartz
	 - Copy an existing folder
	 - Symlink an existing folder

Tramite le frecce della tastiera seleziona "Empty Quartz". Verrà visualizzato il seguente messaggio:

	 Choose how Quartz should resolve links in your content. You can change this  later in `quartz.config.ts`.
	- Treat links as absolute path
	- Treat links as shortest path
	- Treat links as relative paths

Di default Quartz userà il percorso più breve esistente. Se visualizzi il seguente messaggio hai finito: 

	You're all set! Not sure what to try next? Try:
	- Customizing Quartz a bit more by editing `quartz.config.ts`
	- Running `npx quartz build --serve` to preview your Quartz locally
	- Hosting your Quartz online (see: https://quartz.jzhao.xyz/hosting)


#### <span style="color:green"> Se vuoi tornare all'inizio dell'argomento: </span> [[COME PRENDERE APPUNTI]]

#### <span style="color:green"> Se vuoi tornare alla Home della materia: </span> [[SRI]]

#### <span style="color:green">  Se vuoi tornare nella Home: </span> [[index]]