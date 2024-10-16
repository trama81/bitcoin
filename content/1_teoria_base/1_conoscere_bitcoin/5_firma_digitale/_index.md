+++
title = 'Firma digitale'
author = 'me'
date = 2024-10-13
weight = 5
draft = true
+++

>[!important] Brief:
> Questa sezione ti aiuterà a capire cos'è la firma digitale e che ruolo gioca nelle transazioni.

> [!TIP]+ Con parole semplici
> ##### Titolo
> Testo




### Come funziona la firma digitale?

Quando si effettua una transazione in Bitcoin, entra in gioco la **firma digitale**, che è un meccanismo crittografico utilizzato per garantire che il proprietario della chiave privata sia effettivamente colui che possiede i fondi e che sta autorizzando la transazione. La firma digitale consente di nascondere la chiave privata senza comprometterne la funzione.

Ecco come funziona il processo di creazione della firma digitale:




Ecco come funziona il processo di verifica della firma digitale:


---



Ecco come funziona il processo:
1. **Creazione della firma**: Quando invii bitcoin, il software del portafoglio utilizza la tua chiave privata per creare una firma digitale. Questa firma è un insieme di dati che conferma che tu possiedi la chiave privata senza mai rivelarla.
2. **Verifica della firma**: Una volta creata, la firma digitale viene verificata da altri nodi della rete Bitcoin utilizzando la tua **chiave pubblica**. Questi nodi possono confermare che la firma è stata creata da chi possiede la chiave privata associata alla chiave pubblica, senza che la chiave privata stessa venga esposta. In questo modo, la rete garantisce che solo il proprietario effettivo dei bitcoin possa spenderli, mantenendo al sicuro la chiave privata.





### La chiave privata e la firma digitale: Come funzionano nel mondo di Bitcoin

#### Il ruolo della chiave privata nelle transazioni Bitcoin

Ogni volta che invii bitcoin a qualcun altro, la tua chiave privata entra in gioco in modo invisibile ma essenziale. Vediamo come funziona il processo.

1. **Creazione della transazione**: Quando decidi di inviare bitcoin, il software del portafoglio genera una transazione che specifica la quantità di bitcoin da inviare e l’indirizzo del destinatario.
    
2. **Firma digitale**: Per autorizzare la transazione, la tua chiave privata viene utilizzata per creare una **firma digitale**. Questo è un processo crittografico che certifica che sei tu il legittimo proprietario dei fondi che stai inviando. La firma digitale agisce come una prova matematica che conferma l’autenticità della transazione senza rivelare la tua chiave privata.
    
3. **Invio della transazione**: Una volta firmata, la transazione viene trasmessa alla rete Bitcoin, dove sarà verificata dai nodi (computer che mantengono la rete). I nodi usano la tua **chiave pubblica** (che è collegata matematicamente alla tua chiave privata) per verificare la firma digitale e confermare che è stata creata da chi possiede effettivamente i fondi.
    
4. **Verifica della transazione**: La rete può verificare che la firma digitale sia corretta senza mai vedere la tua chiave privata. Questo sistema garantisce la sicurezza delle transazioni e il possesso dei fondi, senza compromettere la segretezza della chiave privata.

Una volta che la rete conferma la validità della firma, la transazione viene inclusa nel blocco successivo della blockchain, e i fondi vengono trasferiti al destinatario.

#### Firma digitale: Come protegge la tua chiave privata

Vediamo più nel dettaglio come funziona:

- Quando firmi una transazione con la tua chiave privata, il risultato è una firma unica che corrisponde solo a quella specifica transazione.
- La firma digitale può essere verificata da chiunque utilizzi la tua chiave pubblica, ma solo tu, con la chiave privata, puoi crearla.
- La firma certifica che la transazione è stata autorizzata dal proprietario dei fondi, ma non rivela alcuna informazione sulla chiave privata, proteggendo così la tua identità e sicurezza.

Questo sistema di firma digitale è il motivo per cui il Bitcoin è così sicuro: anche se la rete verifica le transazioni, nessuno può accedere ai fondi senza la chiave privata.

### Firma digitale: Come protegge la tua chiave privata

La **firma digitale** è un meccanismo crittografico che permette di autorizzare una transazione Bitcoin senza rivelare la tua chiave privata. Il processo di validazione di una transazione coinvolge vari passaggi, ciascuno con input e output specifici. Vediamo un esempio concreto. Supponiamo tu voglia inviare 1 bitcoin a un amico. Il primo passo è creare una transazione che include l'indirizzo del destinatario (l'**input**) e l'ammontare di bitcoin da trasferire. Questa transazione viene poi firmata utilizzando la tua chiave privata. Qui entra in gioco la **funzione hash**, che prende l'intera transazione come input e genera un valore crittografico univoco (l'**output**), una sorta di impronta digitale della transazione. A questo punto, utilizzi la tua chiave privata per creare la **firma digitale** di questo hash, che dimostra che la transazione è stata effettivamente autorizzata dal proprietario dei fondi. Quando invii la transazione firmata alla rete, i nodi Bitcoin prendono la tua **chiave pubblica** come input per verificare la firma. La rete non ha bisogno della tua chiave privata per effettuare questa verifica: usando la chiave pubblica e l’hash della transazione, i nodi possono confermare che la firma corrisponde ai fondi che possiedi senza rivelare la tua chiave privata. Solo se la firma è valida, la transazione viene accettata e inclusa nel prossimo blocco della blockchain. In questo modo, la firma digitale protegge la tua chiave privata garantendo comunque la sicurezza e l'integrità della transazione.








Per comprendere come si ricava la chiave pubblica partendo dall'indirizzo Bitcoin, è utile spiegare più in dettaglio il processo di creazione di un indirizzo e come la chiave pubblica sia collegata ad esso.

### Chiavi pubbliche e indirizzi Bitcoin: come funzionano?

In Bitcoin, ogni utente possiede una coppia di chiavi crittografiche: una **chiave privata** e una **chiave pubblica**. Queste chiavi sono generate tramite crittografia a curva ellittica (ECDSA, Elliptic Curve Digital Signature Algorithm). La **chiave privata** è segreta e deve essere protetta, mentre la **chiave pubblica** è derivata matematicamente dalla chiave privata e può essere condivisa in sicurezza con il mondo.



### Come si ricava la chiave pubblica a partire dall'indirizzo?

Normalmente, **non si risale direttamente alla chiave pubblica partendo dall'indirizzo**. L'indirizzo Bitcoin è un derivato della chiave pubblica, e quindi è possibile partire dalla chiave pubblica per ottenere un indirizzo, ma non viceversa. Questo è intenzionale per motivi di sicurezza: l'indirizzo è una rappresentazione più sicura e breve della chiave pubblica.

Tuttavia, quando una persona invia Bitcoin, **la chiave pubblica del mittente viene rivelata all'interno della transazione**. Questo accade perché la rete ha bisogno di verificare che la transazione sia stata firmata correttamente usando la chiave privata associata all'indirizzo del mittente. Quindi, nel momento in cui una transazione viene trasmessa, la chiave pubblica diventa disponibile per chiunque.

### Esempio pratico di utilizzo della chiave pubblica

Immagina che Alice invii 1 bitcoin a Bob. Ecco cosa accade:

1. Alice crea una transazione nel suo portafoglio che specifica l'importo e l'indirizzo di Bob.
2. Alice firma la transazione con la sua **chiave privata**. Questa firma digitale dimostra che Alice possiede i fondi.
3. La transazione include sia l'indirizzo di Alice che la sua **chiave pubblica**, che viene rivelata alla rete per permettere la verifica.
4. I nodi della rete Bitcoin verificano che la chiave pubblica di Alice corrisponde all'indirizzo Bitcoin da cui sta inviando i fondi.
5. I nodi usano la chiave pubblica di Alice e la firma digitale per verificare che la transazione sia stata effettivamente autorizzata da chi possiede i fondi, senza rivelare la chiave privata.

### Conclusione

In sintesi, l'indirizzo Bitcoin è derivato dalla chiave pubblica tramite una serie di passaggi di hashing e codifica. Non si può risalire alla chiave pubblica dall'indirizzo, ma ogni volta che una transazione viene inviata, la chiave pubblica viene rivelata per consentire la verifica della transazione. Questo sistema crittografico assicura che i fondi possano essere trasferiti in modo sicuro, garantendo al contempo che la chiave privata rimanga segreta.





### La Verifica della Firma Digitale nelle Transazioni Bitcoin: Un Approfondimento Tecnico con Esempio Pratico

La **verifica della firma digitale** nelle transazioni Bitcoin è un processo fondamentale per garantire la sicurezza delle transazioni senza svelare la chiave privata del mittente. La **firma digitale** consente alla rete di confermare che chi invia i fondi è effettivamente il legittimo proprietario, proteggendo allo stesso tempo la segretezza della chiave privata. In questo articolo esamineremo tecnicamente come avviene questo processo e forniremo un esempio concreto per illustrarlo.

#### 1. Cos'è una firma digitale?

La firma digitale è una prova crittografica che dimostra che una transazione è stata autorizzata dal proprietario dei fondi. Quando un utente crea una transazione Bitcoin, utilizza la sua **chiave privata** per generare una firma digitale che è unica per quella specifica transazione.

L’algoritmo crittografico utilizzato da Bitcoin per le firme digitali è l’**ECDSA** (Elliptic Curve Digital Signature Algorithm). Questo algoritmo crea una firma che è verificabile da chiunque conosca la chiave pubblica del mittente, ma senza mai rivelare la chiave privata.

#### 2. Informazioni necessarie per verificare la firma digitale

Per verificare una firma digitale, i nodi della rete Bitcoin hanno bisogno di tre elementi chiave:

- **Chiave pubblica** del mittente: Derivata matematicamente dalla chiave privata, permette di verificare la firma digitale.
- **Firma digitale**: Creata dal mittente utilizzando la chiave privata per firmare i dati della transazione.
- **Dati della transazione**: Include dettagli come l’indirizzo del destinatario, l’ammontare di bitcoin da inviare, e altre informazioni specifiche della transazione.

#### 3. Il processo di verifica della firma digitale

La verifica della firma digitale si svolge in diversi passaggi tecnici:

##### a. Creazione dell’hash della transazione

Prima di verificare la firma, il nodo calcola un **hash** della transazione. L’hash è un’impronta digitale unica creata da una funzione crittografica che trasforma i dati della transazione in una stringa univoca di lunghezza fissa. Anche una piccola modifica ai dati della transazione genererebbe un hash completamente diverso, garantendo così che i dati non siano stati manomessi.

##### b. Uso della chiave pubblica per la verifica

Il nodo utilizza la **chiave pubblica** del mittente per verificare che la firma digitale sia valida. Poiché la chiave pubblica è pubblicamente disponibile, chiunque può eseguire questa verifica. Tuttavia, la chiave pubblica non può essere utilizzata per risalire alla chiave privata, proteggendo così la sicurezza del proprietario.

##### c. Verifica tramite l’algoritmo ECDSA

L’algoritmo **ECDSA** confronta la firma digitale con l’hash della transazione e la chiave pubblica. Se la firma è valida, significa che solo chi possiede la chiave privata associata alla chiave pubblica potrebbe aver generato quella firma. Se la verifica riesce, la transazione è considerata autentica.

##### d. Convalida della transazione

Se la firma è corretta, la transazione viene convalidata e diffusa sulla rete. Se invece la firma non è valida, la transazione viene rigettata.

#### 4. Esempio concreto di verifica della firma digitale

Vediamo ora un esempio pratico di come avviene la verifica di una firma digitale in una transazione Bitcoin.

**Scenario**: Supponiamo che Alice voglia inviare 1 bitcoin a Bob. Ecco come si svolge il processo.

##### 1. Creazione della transazione

Alice apre il suo portafoglio Bitcoin e crea una transazione in cui specifica che vuole inviare 1 bitcoin all'indirizzo di Bob. Il portafoglio di Alice raccoglie le informazioni necessarie, come l'ammontare da inviare e l'indirizzo del destinatario (l'indirizzo di Bob).

##### 2. Generazione della firma digitale

Per autorizzare questa transazione, il portafoglio di Alice utilizza la sua chiave privata per firmare i dati della transazione. Il software del portafoglio crea prima un **hash della transazione** e poi usa la chiave privata per firmare questo hash, creando così una firma digitale univoca.

##### 3. Invio della transazione

La transazione firmata viene inviata alla rete Bitcoin, dove viene ricevuta dai nodi che eseguono la verifica.

##### 4. Verifica della firma

Uno dei nodi riceve la transazione e inizia il processo di verifica:

- Il nodo calcola l'hash della transazione utilizzando i dati inviati da Alice.
- Utilizza poi la **chiave pubblica** di Alice (che è pubblicamente associata al suo indirizzo Bitcoin) per verificare che la firma digitale corrisponda all'hash della transazione. Questo passaggio conferma che solo Alice, che possiede la chiave privata, avrebbe potuto firmare la transazione.

##### 5. Validazione e inclusione nella blockchain

Se la firma digitale è valida, il nodo accetta la transazione e la diffonde ulteriormente nella rete. Alla fine, la transazione di Alice viene inclusa in un blocco della blockchain, e 1 bitcoin viene trasferito da Alice a Bob. In tutto questo processo, la chiave privata di Alice non è mai stata rivelata.

#### 5. Perché la chiave privata non viene mai svelata

La chiave privata di Alice è utilizzata solo per generare la firma digitale, e non è mai condivisa con la rete. Grazie alla crittografia a chiave pubblica, la chiave privata non può essere dedotta dalla chiave pubblica o dalla firma digitale. Questo sistema garantisce che, anche se la transazione viene verificata pubblicamente, solo chi possiede la chiave privata può autorizzare l’invio di fondi.

#### 6. Conclusione

La verifica della firma digitale nelle transazioni Bitcoin è un processo crittografico sofisticato ma essenziale per la sicurezza della rete. Utilizzando la crittografia a chiave pubblica e l'algoritmo ECDSA, Bitcoin permette di verificare l'autenticità delle transazioni senza compromettere la segretezza della chiave privata. Grazie a questo sistema, gli utenti possono trasferire fondi in modo sicuro, mentre la rete mantiene la fiducia e l'integrità delle transazioni.



### Come si ricava la chiave pubblica a partire dall'indirizzo?

Normalmente, **non si risale direttamente alla chiave pubblica partendo dall'indirizzo**. L'indirizzo Bitcoin è un derivato della chiave pubblica, e quindi è possibile partire dalla chiave pubblica per ottenere un indirizzo, ma non viceversa. Questo è intenzionale per motivi di sicurezza: l'indirizzo è una rappresentazione più sicura e breve della chiave pubblica.

Tuttavia, quando una persona invia Bitcoin, **la chiave pubblica del mittente viene rivelata all'interno della transazione**. Questo accade perché la rete ha bisogno di verificare che la transazione sia stata firmata correttamente usando la chiave privata associata all'indirizzo del mittente. Quindi, nel momento in cui una transazione viene trasmessa, la chiave pubblica diventa disponibile per chiunque.

### Esempio pratico di utilizzo della chiave pubblica

Immagina che Alice invii 1 bitcoin a Bob. Ecco cosa accade:

1. Alice crea una transazione nel suo portafoglio che specifica l'importo e l'indirizzo di Bob.
2. Alice firma la transazione con la sua **chiave privata**. Questa firma digitale dimostra che Alice possiede i fondi.
3. La transazione include sia l'indirizzo di Alice che la sua **chiave pubblica**, che viene rivelata alla rete per permettere la verifica.
4. I nodi della rete Bitcoin verificano che la chiave pubblica di Alice corrisponde all'indirizzo Bitcoin da cui sta inviando i fondi.
5. I nodi usano la chiave pubblica di Alice e la firma digitale per verificare che la transazione sia stata effettivamente autorizzata da chi possiede i fondi, senza rivelare la chiave privata.