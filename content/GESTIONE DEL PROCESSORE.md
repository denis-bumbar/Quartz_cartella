I SO moderni sfruttano le potenzialità di parallelismo dell’hardware per minimizzare i tempi di risposta del sistema ed aumentare il *throughput del sistema* (numero di programmi eseguiti per unità di tempo). L’ottimizzazione del tempo di CPU si ha con la *multi-programmazione* (ossia la contemporanea presenza di più programmi in memoria). La gestione del sistema prevede:
- <span style = "color:red" >Scheduling dei job:</span> insieme di strategie e meccanismi usati per la scelta dei programmi che dal disco devono essere caricati in RAM
- <span style = "color:red"> Scheduling della CPU: </span> insieme di strategie e meccanismi usati per assegnare e sospendere l’utilizzo della CPU da parte dei vari processi

### <span style="color:red"> PROGRAMMA </span>

È l'insieme di istruzioni, memorizzato su memoria di massa (*entità statica*). E’ possibile avere più processi originati dallo stesso codice (esempio: si possono avere aperte due finestre con lo stesso programma in esecuzione). I processi possono essere:
- <span style = "color:red">Indipendenti:</span> un processo può evolvere autonomamente senza necessità di scambiare dati con altri processi;
- <span style = "color:red"> Cooperanti: </span>due o più processi per evolvere necessitano di scambiarsi informazioni;
- <span style = "color:red">Competitori:</span> possono ostacolarsi a vicenda, per usare la medesima risorsa, compromettendo la terminazione delle loro elaborazioni

### <span style="color:red"> PROCESSO </span>

È un'istanza di programma in evoluzione, cioè che è eseguito dal processore, quindi deve risiedere in RAM (*entità dinamica*). L’esecuzione di un processo consta di un alternarsi di fasi di uso della CPU a fasi di attesa di esecuzione di operazioni su altre risorse di sistema. I SO multitasking aumentano il throughput portando avanti in parallelo più processi e riducendo al minimo l’inattività della CPU. Ogni processo è costituito da due parti: 
- ***codice*** (composto dalle istruzioni); 
- ***dati del programma***. L’insieme di tutti i dati di un processo prende il nome di ***contesto del processo.***
Durante il ciclo di vita di un processo, questo può trovarsi in una certa “situazione” rispetto alla CPU, definita come [[Stato del processo.]]
