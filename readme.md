# Demo Center	

### Sommario

 1. [Introduzione](#introduzione)
 2. [Setup Localizzazione e movimento](#setup-Localizazzione-e-movimento)
 3. [Mappatura ambiente](#mappatura-ambiente)
 4. [Configurazione punti di riferimento](#configurazione-punti-di-riferimento)
 5. [Utilizzo giornaliero nel Demo Center](#utilizzo-giornaliero-nel-demo-center)
 6. [Tips & Tricks](#tips-&-tricks)

## Introduzione
La gestione della navigazione di Pepper deve essere svolta in due fasi: ***Setup***, dove il robot studia l'ambiente in modo da ottenerne una mappa virtuale e una di ***Production*** dove il robot si muove utilizzando la mappa creata in precedenza. Queste due fasi possono essere portate a termine nell'experience *DemoCenter Intesa Sanpaolo*, grazie a due app separate, che possono essere trovate nel menù applicazioni di Pepper.

 1. LOCSEC ISPIC Demo Center
 2. ISPIC Demo Center
 
lo scopo della prima app è la prima configurazione del movimento e della navigazione (mappatura ambiente, configurazione punti di riferimento), invece la seconda funge da app principale contenente i flussi riguardanti le isole e il demo center vero e proprio.

## Setup Localizazzione e movimento
Questa fase va effettuata solo una volta, oppure nel caso che il Pepper non riesca a localizzarsi e/o muoversi con successo nell'ambiente.
Durante la configurazione, bisogna insegnare al robot la mappa dell'ambiente in cui dovrà muoversi, così come tutti i punti di interesse. Questo passaggio viene effettuato manualmente, spingendo il robot in giro per l'area per mostrargli il percorso e gli spazi che può percorrere. Per un risultato ottimale <ins>questo processo deve avvenire in assenza di oggetti o persone</ins> che non saranno presenti durante la fase di ***production*** altrimenti verranno registrati come ostacoli permanenti nella mappa.
Il robot riconosce la sua posizione nello spazio grazie a dei **punti di riferimento** che in questo caso sono le <ins>lettere dalla A alla H scritte rigorosamente in maiuscolo</ins>, entreremo nel dettaglio delle funzioni di suddetti punti in seguito.

### Mappatura ambiente
Il primo step per la configurazione della ***Navigation*** consiste nel mappare l'ambiente seguendo i prossimi punti:

 1. Posizionare il Robot nel *punto A* (il punto A rappresenta la posizione dove l'experience verrà avviata ogni giorno, altresì dove Pepper accoglierà gli ospiti)
 2. Chiudere il flap del freno (quello sul bumper posteriore)
 3. Aprire l'app **LOCSEC ISPIC Demo Center**
 4. Cliccare su *"Setup Mode"*
 5. Cliccare su *"LOCALIZE & MAP"*
 6. Seguire le indicazioni vocali e sul tablet di Pepper, utilizzando come percorso il seguente, partendo da A e seguendo il tracciato: 
 >Durante gli spostamenti, rimanere dietro al Pepper, spingendolo lentamente attraverso l'ambiente che si intende mappare. Per una mappatura di successo eseguire percorsi il più possibile rettilinei con angoli netti.
 #### Planimetria
![planimetria](https://publicdeliveryfiles.s3-eu-west-1.amazonaws.com/democenter/path.png)
 7. Una volta arrivati al punto H il processo di mappatura è completato.
 
 ### Configurazione punti di riferimento
Ora che è stato mappato l'ambiente e Pepper è in grado di posizionarsi in esso, si può procedere con la configurazione dei punti di riferimento.
 
 1. Posizionare il Robot nel *punto A* (il punto iniziale durante la fase di [mappatura](#mappatura-ambiente)).
 2. Andare in *Setup Mode* > *SAVE LOCATIONS*
 > Se sono presenti dei punti precedentemente salvati eliminarli tutti cliccando sui pulsanti rossi con scritto "*DELETE X*", chiudere la finestra con scritto "*No Locations to load*" e successivamente cliccare sul tasto verde in basso a destra con scritto "*Save locations*". Chiudere la finestra di avvenuto salvataggio.
 3. Chiudere il flap del freno (quello sul bumper posteriore)
 4. Cliccare su "*Add Location*"
 5. Cliccare su "*You are at home*"
 > Ora Pepper si localizzerà nell'ambiente, mantenete le distanze
 6. Una volta localizzato e riaperto il flap posteriore e si può procedere a salvare direttamente il Punto **A** (essendo già nella posizione di partenza)
 > Durante il salvataggio dei punti di riferimento assicurarsi che il robot sia rivolto nella direzione indicata dalle frecce, come indicato nella [platimetria](#planimetria).
 7. Spostare il robot al punto successivo seguendo il percorso indicato
 8. Inserire il nome del punto corrispondente
 9. Cliccare su "*save*"
 10. Ripetere dal passo 7 fino a quando non si arriva al punto **H**. 
 
Una volta completata la configurazione dei punti di riferimento è possibile chiudere l'app **LOCSEC ISPIC Demo Center**.

 ## Utilizzo giornaliero nel Demo Center
Ora che il robot ha una mappa dell'ambiente e dei punti di riferimento è possibile utilizzare l'app **ISPIC Demo Center**. 
Una volta portato il robot nella posizione **A** e aperta l'app ci si trova davanti una schermata di **Configurazione** con diverse tab.
Recandosi nella tab "*Localizzazione*" è possibile verificare che tutti i punti richiesti dall'applicazione siano stati mappati e caricati correttamente dal colore dei pulsanti corrispondenti al punto. Se uno o più dei punti risultassero col bordo in rosso si può ritornare al processo di [mappatura](#mappatura) cliccando sul pulsante "*Esegui la mappatura*", altrimenti si procede con la localizzazione del robot con il pulsante "*Localizza*".
A questo punto il robot attende 20 secondi, in modo da dare il tempo di liberare l'area, per poi procedere con la localizzazione.
Avendo il robot localizzato con successo, si può selezionare quale versione dell'app bisogna eseguire (lunga o corta) ed infine dare inizio all'experience vera e propria col pulsante "*Inizia*".

Si può ritornare in qualsiasi momento a questa schermata premendo il bumper posteriore.

## Tips & Tricks

 - Durante gli spostamenti, restare sempre dietro al Pepper per un miglior risultato.
 - Se l'app viene interrotta, ripristinata quando il Pepper non è in posizione **A** oppure quando il Pepper si perde durante il tragitto bisogna rieffetture la localizazione, dalla schermata di **Configurazione**.
 - Sulla vecchia versione di Pepper(quello con due fori sul collo) il processo di [Setup Localizzazione e movimento](#setup-Localizazzione-e-movimento) conviene effettuarlo prima di ogni esecuzione dell'app **ISPIC Demo Center** e porta ad un'affidabilità nella navigazione di circa 20 minuti, in condizioni di luce variabile.

