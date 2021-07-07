# IAesame
Challenge di luglio: Customer Churn

###Contesto
I vostri clienti non versano più gli stipendi nei conti correnti della vostra banca? Usano il bancomat solo per prelevare e la giacenza media è di 20€? Mi sa che stanno per mollarvi!

###Obiettivo

Tirate fuori un classificatore che preveda se un cliente, data la "foto" che il dataset inquadra, stia per abbandonare la banca oppure sia destinato a rimanere.

###Dataset
Le stats:

    CustomerId: id cliente
    Surname: cognome del cliente
    CreditScore: score creditizio
    Geography: paese d'appartenenza
    Gender: sesso
    Age: età
    Tenure: da quanto è cliente
    Balance: ammontare del conto in banca
    NumOfProducts: quanti prodotti finanziari usa
    HasCrCard: ha una carta di credito
    IsActiveMember: se il conto è attivo
    EstimatedSalary: entrate stimate del cliente
    Exited: se ha cambiato banca o no

###Consegna

Avete 24 ore di tempo.

Produrre 2 notebook, 1 di preparazione dati ed 1 di training.

Il notebook di training, fa tutto quello che vi immaginate: apre il dato di test/train, fa l'analisi, fa la trasformazione dei dati, addestra il classificatore ed emette l'accuracy.

Il notebook di preparazione, a partire dal file di dati che vi verrà passato, crea e scrive su disco 2 file CSV con nome fisso, train.csv e test.csv, che dovranno contenere i rispettivi dati di train e test. Nel notebook di training dovrete aprire ed usare quei due file. Non c'è quindi bisogno di salvare modelli da un notebook all'altro poichè tutto avviene in quello di training. Questo notebook non fa calcoli, nè pulizia, nè altro. Fa solo split.

In sede di valutazione userò come file di training l'intero dataset che vi ho passato e come file di test un mio personale che conterrà la parte di dati che non vi ho fornito; farò quindi girare nuovamente il notebook di training facendo calcolare al vostro algoritmo la metrica di accuratezza sul mio file, non sul file di test che avrete prodotto e usato durante la challenge.

In questo modo avremo la misura oggettiva del vostro modello su una porzione di dati non vista.

Consegnate un testo con solamente l'indirizzo di un repo GitHub (niente "Caro professore, ecco i notebook", che mi fare crashare gli script che scaricano i file), creato ad-hoc e contenente i 2 soli notebook (preparazione e train) e l'eventuale requirements.txt, senza i file di training/test set. Usate main come branch.

Non usate path assoluti nel vostro codice e occhio ai nomi file che mi devo aspettare (train.csv e test.csv); se nel codice scriverete altro e il notebook non girerà, verrà interpretata come non compilante e saranno zero punti.

Tutte le dipendenze devono essere gestite speficate nelle celle del notebook; se volete usare un requirements.txt, fate "!pip install" direttamente nelle celle all'inizio. Se vi dimenticherete di fare "pip install" e il notebook non compilerà, saranno zero punti. Farò girare il notebook in un ambiente pulito, ma voi sforzatevi di non includere dipendenze inutili e mantenete il requirements minimale altrimenti potrebbero comunque verificarsi conflitti.

Tutte le spiegazioni devono stare nel notebook: se usate metodi non spiegati a lezione dovete documentarli: non basta fare copia incolla dal web, devo capire che abbiate capito. Potete come al solito usare qualunque tecnica o tecnologia, ma siate descrittivi.

Il notebook serve a comunicare: fatemi vedere una linea di pensiero concisa e ben argomentata. Niente flussi di coscienza, prove, vicoli ciechi o kilometri di grafici senza didascalie esplicative

Buon divertimento e in bocca al lupo!
