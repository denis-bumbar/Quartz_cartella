All'interno di questo file tratteremo come prendere appunti tramite **OBSIDIAN**  e **QUARTZ.** Saranno descritti tutti i passaggi da svolgere e nel mio caso utilizzerò un sistema operativo MacOs. I comandi saranno quindi scritti con sintassi Linux e nel caso che avete un sistema operativo Windows si possono cercare i relativi comandi. Buon divertimento.

Prerequisiti:

[[XCode Command Line Tools]] 

[[NodeJS v18.14+]] (puoi verificare la tua versione tramite node -v)

[[NPM v9.3.1+]] (puoi verificare la tua versione tramite npm -v)

[[Git]] (puoi verificare la tua versione tramite git --versione)

**Obsidian**

[[Quartz]]

#### Crea la tua repository:

Entra su Github, crea una nuova repository e come nome assegna quello che hai scelto precedentemente durante la preparazione di Quartz. In alto apparirà una barra con un percorso simile a questo:

	git@github.com:nicolevanderhoeven/doing-it-in-public.git

**Copialo.**

Dal terminale esegui i seguenti comandi, ricordando di essere nella cartella creata:

	git remote -v

Viene visualizzato questo testo:

	origin  https://github.com/jackyzha0/quartz.git (fetch)
	origin  https://github.com/jackyzha0/quartz.git (push)
	upstream        https://github.com/jackyzha0/quartz.git (fetch)
	upstream        https://github.com/jackyzha0/quartz.git (push)

Prossimo comando per rimuovere l'origine:

	git remote rm origin

Ora rimettila usando il seguente comando + ***il link prima copiato***:

	git remote add origin

Controlla che tutto sia andato a buon fine con il seguente comando:

	git remote -v

Dovresti vedere una scritta simile:

	origin  https://github.com/yourusername/my-notes.git (fetch)
	origin  https://github.com/yourusername/my-notes.git (push)
	upstream        https://github.com/jackyzha0/quartz.git (fetch)
	upstream        https://github.com/jackyzha0/quartz.git (push)

Sincronizza le modifiche:

	npx quartz sync --no-pull

***Crea un vault su obsidian.***

Controlla che il tuo sito funzioni in locale con il seguente comando:

	npx quartz sync --no-pull

Viene visualizzata la seguente scritta alla fine:

	Started a Quartz server listening at http://localhost:8080

Copia e incolla nella barra di ricerca del tuo browser questo:

	http://localhost:8080

Sincronizza le modifiche:

	npx quartz sync

Ora hai il tuo sito in locale.

#### PUBBLICA IL TUO SITO ONLINE.

Esegui i seguenti comandi da terminale ricordandoti di essere nella cartella creata prima.

Crea il seguente file:

	touch .github/workflows/deploy.yml

Apri il file, che però risulta nascosto quindi visualizzalo tramite il comando " CMD + OPT + . "

Copia e incolla il seguente codice controllando le varie versioni di sistema operativo e Node:

	name: Deploy Quartz site to GitHub Pages
	 
	on:
	  push:
	    branches:
	      - v4
	 
	permissions:
	  contents: read
	  pages: write
	  id-token: write
	 
	concurrency:
	  group: "pages"
	  cancel-in-progress: false
	 
	jobs:
	  build:
	    runs-on: ubuntu-22.04
	    steps:
	      - uses: actions/checkout@v3
	        with:
	          fetch-depth: 0 # Fetch all history for git info
	      - uses: actions/setup-node@v3
	        with:
	          node-version: 18.14
	      - name: Install Dependencies
	        run: npm ci
	      - name: Build Quartz
	        run: npx quartz build
	      - name: Upload artifact
	        uses: actions/upload-pages-artifact@v2
	        with:
	          path: public
	 
	  deploy:
	    needs: build
	    environment:
	      name: github-pages
	      url: ${{ steps.deployment.outputs.page_url }}
	    runs-on: ubuntu-latest
	    steps:
	      - name: Deploy to GitHub Pages
	        id: deployment
	        uses: actions/deploy-pages@v2

Salva e chiudi il file.

Sincronizza le modifiche:

	npx quartz sync

Se vedi che il sito online non funziona comunque, controlla il codice del file ***deploy.yml.*** Puoi controllare che corrisponda al tuo bisogno al seguente link:

	https://quartz.jzhao.xyz/hosting#github-pages

Visualizza il tuo sito con il seguente link, ricordati di cambiare yourusername con il tuo username e my-notes con il nome della cartella che hai creato:

	https://yourusername.github.io/my-notes

# GODITI IL TUO NUOVO SITO!!!

#### <span style="color:green"> Se vuoi tornare alla Home della materia: </span> [[SRI]]

#### <span style="color:green">  Se vuoi tornare nella Home: </span> [[index]]