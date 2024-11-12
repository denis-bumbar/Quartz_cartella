I possibili stati sono, come rappresentati in figura: 
- <span style= "color:red">new: </span>stato in cui si trova appena creato (quindi appena caricato in RAM) 
- <span style = "color:red">ready: </span> un processo è nello stato di pronto se ha tutte le risorse necessarie alla sua evoluzione ad eccezione della CPU 
- <span style = "color:red">running: </span>la CPU sta eseguendo le sue istruzioni, quindi a esso è assegnato il processore 
- <span style = "color:red">waiting:</span> un processo è in attesa quando gli manca una risorsa per poter evolvere; quindi attende che si verifichi un evento che lo riporti in stato di “*ready*” 
- <span style = "color:red">terminated:</span> tutto il codice del processo è stato eseguito e quindi ha terminato l’esecuzione; il SO può rilasciare tutte le risorse che utilizzava

<span style="color:green">Per tornare indietro: </span> [[GESTIONE DEL PROCESSORE]]