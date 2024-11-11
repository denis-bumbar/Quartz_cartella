Xcode permette di progettare l'interfaccia utente, scrivere codice, testare e eseguire il debug tutto all'interno di un unico flusso di lavoro. Ci risulterà quindi fondamentale nell'installazione e gestione delle applicazioni da linea di comando. Per farlo esistono diversi pacchetti e io userò il **homebrew.** Puoi installarlo usando il seguente comando:

	/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Una volta finita l'installazione di tutti i pacchetti esegui i seguenti comandi per aggiungere **HOMEBREW** al tuo percorso:

	echo >> /Users/nome_utente_del_tuo_mac/.zprofile

	echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/nome_utente_del_tuo_mac/.zprofile

	eval "$(/opt/homebrew/bin/brew shellenv)"

Esegui "brew help" per iniziare.
#### <span style="color:green"> Se vuoi tornare all'inizio dell'argomento:</span> [[COME PRENDERE APPUNTI]]

#### <span style="color:green"> Se vuoi tornare alla Home della materia: </span>[[SRI]]
#### <span style="color:green"> Se vuoi tornare nella Home: </span>[[Appunti]]