Quando è creato un nuovo processo (*caricato in RAM il programma*), gli viene assegnato un identificatore (*PID, Process Identifier*) e viene inserito nell’elenco dei processi pronti (*RL, Ready List*).
Quando gli viene assegnata la CPU, il processo passa nello stato di esecuzione, dal quale può uscire per tre motivi:
- <span style="color:red">termina la sua esecuzione</span>, cioè il processo esaurisce il suo codice e quindi finisce;
- <span style="color:red">termina il suo tempo di CPU</span>, cioè il quanto di tempo a sua disposizione, e quindi ritorna nella lista dei **processi pronti RL**
- <span style="color:red">gli manca la disponibilità di una risorsa:</span> per poter evolvere necessita di una risorsa al momento non disponibile e quindi il processo si sospende e passa nello stato di attesa formando la waiting list (WL).
Dallo stato di **sospeso** (in WL) un processo esce solo quando ottiene la risorsa attesa, per passare poi nella RL dalla quale può essere prelevato per passare di nuovo in stato di **esecuzione.**

#### <span style="color:green"> Per tornare indietro: </span> [[GESTIONE DEL PROCESSORE]]
#### <span style="color:green"> Se vuoi tornare alla Home della materia: </span>[[TPI]]
#### <span style="color:green"> Se vuoi tornare nella Home: </span>[[index]]
