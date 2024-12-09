## <span style="color:yellow"> PROTOCOLLI DI RETE </span>

Un protocollo di rete è un insieme di regole stabilite che specificano come formattare, inviare e ricevere dati in modo che gli endpoint della rete possano comunicare nonostante le differenze nelle loro infrastrutture e standard.

Ecco i protocolli più importanti:

### <span style="color:red"> IP: </span>
È il protocollo utilizzato per la ricerca di computer in base al loro indirizzo IP. Esegue l’instradamento dei datagrammi, ovvero si tratta di determinare il percorso dei dati lungo i nodi di rete.. La trasmissione avviene anche senza stabilire una connessione e non invia nemmeno notifiche della corretta e integra ricezione dei dati. IPv4 è il più famoso e presenta indirizzi a 32 bit.

### <span style="color:red"> TCP/IP </span>
Sono in realtà un insieme di protocolli che consentono la comunicazione in rete di dispositivi. Protocolli di questo tipo consentono di implementare un modello di connessione a pacchetto. Sono la spina dorsale dell’intero Internet.
- <span style="color:green">**TCP (Transmission Control Protocol) :** </span> è un protocollo speciale che controlla la trasmissione. È progettato per stabilire e mantenere una connessione affidabile tra i dispositivi. È lui che è responsabile del trasferimento dei dati, controlla il volume dei file trasferiti ed esegue un nuovo invio in caso di guasti.
- <span style="color:green"> **IP(Internet Protocol) :** </span> è la base per l’architettura di trasferimento file ed è necessaria per inviare un pacchetto di rete all’indirizzo richiesto. Tutti i dati sono pre-divisi in più pacchetti, che vengono inviati indipendentemente l’uno dall’altro alla destinazione finale.
- <span style="color:green"> **Come funziona? :** </span> la suite di protocolli TCP/IP è senza stato, il che significa che ogni richiesta del client è considerata nuova perché non è correlata alle richieste precedenti. L’assenza di stato consente di utilizzare permanentemente qualsiasi percorso di rete anche per altre richieste. Il livello di trasporto della rete funziona in modo stateful. Cioè la connessione non viene chiusa finchè tutti i pacchetti non sono stati ricevuti e riassemblati correttamente. Ricorda che è formato da solo 4 livelli: canale, rete, trasporto, applicato. Il livello collegamento integra anche quello fisico.

Uno stack di protocolli di rete è necessario per mantenere la comunicazione tra i computer (host) connessi a una rete. Questo permette l’indipendenza dall’Hardware di questi protocolli. Essenzialmente, lo scopo principale di TCP/IP è fornire traffico per reti di grandi dimensioni e mantenere funzionante l’intera Internet, è inoltre un modello di rete che descrive l’intero processo di trasferimento dei dati digitali.

### <span style="color:red"> HTTP </span>
È un protocollo di trasferimento di marcatura ipertestuale. Funziona tramite client(richiesta) - server(risposta). Il cliente richiede dei dati al server che quindi glieli manda, il protocollo HTTPS quindi si occupa del trasporto di dati nello scambio di informazioni client-server. HTTPS è più sicuro e per questo c’è maggiore tendenza al suo utilizzo. Questa sicurezza è data da due protocolli di crittografia: SSL e TLS che lavorano entrambi con chiavi di sicurezza e certificazione emesse tramite lo standard X.509.

### <span style="color:red"> UDP </span>
L'User Data Protocol è simile al TCP ma differisce in un piccolo dettaglio, cioè il comportamento sulla rete. L'utente con esso non ha bisogno di confermare l'avvenuto invio o ricezione di dati. Abbiamo quindi un incremento della velocittà a discapito di sicurezza e affidabilità. Molto utile quindi nella messaggistica istantanea, nelle chat dei videogiochi e di stream live.

### <span style="color:red"> SSL/TLS </span>
SSL è un protocollo crittografico per la crittografia di richieste e risposte, è necessario per spostare in modo sicuro i dati su Internet e TLS è la sua versione avanzata.

### <span style="color:red"> SHH </span>
Il protocollo Secure Shell è implementato a livello di applicazione ed è progettato per gestire da remoto il sistema attraverso un canale sicuro. Ecco le funzionalità da lui incluse:
- <span style="color:green"> crittografia: </span> autorizzazione per chiave, ovvero tutto il traffico, comprese le password, viene crittografato utilizzando algoritmi diversi;
- <span style="color:green"> sicurezza: </span> derivata dalla crittografia;
- <span style="color:green"> compressione: </span> molto utile durante la trasmissione di dati.

### <span style="color:red"> FTP </span>
Il File Transfer Protocol viene utilizzato per accedere a host remoti e trasferire software. Ecco le proprietà:
- <span style="color:green"> efficenza: </span> il protocollo garantisce l’invio o l’emissione di un errore, poiché viene utilizzato un sistema di quote;
- <span style="color:green"> variabilità della crittografia: </span> in diversi casi sono possibili connessioni anonime o il trasferimento di password e accessi in chiaro;
- <span style="color:green"> autenticazione integrata: </span> gli utenti sono autenticati per impostazione predefinita;
- <span style="color:green"> connessioni multiple: </span> il protocollo FTP utilizza almeno una doppia connessione.

## <span style="color:yellow"> PROTOCOLLI DI FLUSSO </span>
- ### <span style="color:red"> UTOPIA </span>


#### <span style="color:green">  Se vuoi tornare nella Home: </span> [[index]]