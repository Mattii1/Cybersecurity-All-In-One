
# MODULE 1
# Natural languages vs. programming languages

Una lingua è un mezzo (e uno strumento) per esprimere e registrare pensieri. Ci sono molte lingue intorno a noi. Alcuni di essi non richiedono né la parola né la scrittura, come il linguaggio del corpo; è possibile esprimere i tuoi sentimenti più profondi in modo molto preciso senza dire una parola.

Un'altra lingua che usi ogni giorno è la tua lingua madre, che usi per manifestare la tua volontà e per riflettere sulla realtà. Anche i computer hanno un proprio linguaggio, chiamato linguaggio macchina, che è molto rudimentale.

Un computer, anche il più sofisticato dal punto di vista tecnico, è privo anche di una traccia di intelligenza. Si potrebbe dire che è come un cane ben addestrato: risponde solo a una serie predeterminata di comandi conosciuti.

I comandi che riconosce sono molto semplici. Possiamo immaginare che il computer risponda a ordini del tipo "prendi quel numero, dividi per un altro e salva il risultato".

Un insieme completo di comandi conosciuti è chiamato elenco di istruzioni, talvolta abbreviato in IL. Diversi tipi di computer possono variare a seconda delle dimensioni dei rispettivi IL e le istruzioni potrebbero essere completamente diverse a seconda dei modelli.

Nota: i linguaggi macchina sono sviluppati dagli esseri umani.

Nessun computer è attualmente in grado di creare una nuova lingua. Tuttavia, ciò potrebbe cambiare presto. Proprio come le persone usano un numero di lingue molto diverse, anche le macchine hanno molte lingue diverse. La differenza, però, è che le lingue umane si sono sviluppate naturalmente.

Inoltre, sono ancora in evoluzione e ogni giorno vengono create nuove parole man mano che le vecchie parole scompaiono. Queste lingue sono chiamate lingue naturali.

Possiamo dire che ogni linguaggio (macchina o naturale, non importa) è costituito dai seguenti elementi:
- un alfabeto
- un lessico
- una sintassi
- semantica

# Machine language vs. high-level language

L'IL è, infatti, l'alfabeto di un linguaggio macchina. Questo è l'insieme di simboli più semplice e primario che possiamo utilizzare per impartire comandi a un computer. È la lingua madre del computer.

Sfortunatamente, questa lingua madre è ben lontana dalla lingua madre umana. Entrambi (computer e esseri umani) abbiamo bisogno di qualcos'altro, un linguaggio comune per computer e esseri umani o un ponte tra due mondi diversi.

Abbiamo bisogno di un linguaggio in cui gli esseri umani possano scrivere i propri programmi e di un linguaggio che i computer possano utilizzare per eseguire i programmi, un linguaggio che sia molto più complesso del linguaggio macchina e tuttavia molto più semplice del linguaggio naturale.

Tali linguaggi sono spesso chiamati linguaggi di programmazione di alto livello. Sono almeno in qualche modo simili a quelli naturali in quanto utilizzano simboli, parole e convenzioni leggibili dagli esseri umani. Questi linguaggi consentono agli esseri umani di esprimere comandi ai computer molto più complessi di quelli offerti dagli IL.

Un programma scritto in un linguaggio di programmazione di alto livello è chiamato codice sorgente (in contrasto con il codice macchina eseguito dai computer). Allo stesso modo, il file contenente il codice sorgente è chiamato file sorgente.

# Compilation vs. Interpretation

La programmazione informatica è l'atto di comporre gli elementi del linguaggio di programmazione selezionato nell'ordine che provocherà l'effetto desiderato. L'effetto potrebbe essere diverso in ogni caso specifico: dipende dall'immaginazione, dalla conoscenza e dall'esperienza del programmatore.

Naturalmente, una tale composizione deve essere corretta in molti sensi:

in ordine alfabetico: un programma deve essere scritto in uno script riconoscibile, come romano, cirillico, ecc.
lessicalmente – ogni linguaggio di programmazione ha il suo dizionario ed è necessario padroneggiarlo; per fortuna, è molto più semplice e più piccolo del dizionario di qualsiasi lingua naturale;
sintatticamente – ogni lingua ha le sue regole e devono essere rispettate;
semanticamente: il programma deve avere un senso.
Sfortunatamente, un programmatore può anche commettere errori con ciascuno dei quattro sensi sopra menzionati. Ognuno di essi può rendere il programma completamente inutile.

Supponiamo che tu abbia scritto con successo un programma. Come convinciamo il computer a eseguirlo? Devi rendere il tuo programma in linguaggio macchina. Fortunatamente, la traduzione può essere eseguita da un computer stesso, rendendo l’intero processo veloce ed efficiente.

Esistono due modi diversi per trasformare un programma da un linguaggio di programmazione di alto livello in linguaggio macchina:

- **Compilazione**: il programma sorgente viene tradotto una volta (tuttavia, questo atto deve essere ripetuto ogni volta che si modifica il codice sorgente) ottenendo un file (ad esempio un file .exe se il codice è destinato a essere eseguito sotto MS Windows) contenente il codice macchina. Ora puoi distribuire il file in tutto il mondo; il programma che esegue questa traduzione è chiamato compilatore o traduttore.
- **Interpretazione**: tu (o qualsiasi utente del codice) puoi tradurre il programma sorgente ogni volta che deve essere eseguito. Il programma che esegue questo tipo di trasformazione è chiamato interprete, poiché interpreta il codice ogni volta che è destinato ad essere eseguito. Significa anche che non è possibile distribuire semplicemente il codice sorgente così com'è, perché anche l'utente finale ha bisogno dell'interprete per eseguirlo.

# What does the interpreter do?

Supponiamo ancora una volta che tu abbia scritto un programma. Ora esiste come un file nel computer: un programma per il computer è in realtà un pezzo di testo, quindi il codice sorgente viene solitamente inserito nei file di testo.

Nota: deve essere testo puro, senza decorazioni come font diversi, colori, immagini incorporate o altri media. Ora devi invocare l'interprete e lasciargli leggere il tuo file sorgente.

L'interprete legge il codice sorgente nel modo comune nella cultura occidentale: dall'alto al basso e da sinistra a destra. Ci sono alcune eccezioni: verranno trattate più avanti nel corso.

Innanzitutto l'interprete controlla se tutte le righe successive sono corrette (utilizzando i quattro aspetti trattati in precedenza).

Se il compilatore trova un errore, termina immediatamente il suo lavoro. L'unico risultato in questo caso è un messaggio di errore.
![The concept of Interpretation](https://skillsforall.com/content/pe1/1.0/m1/course/en-US/assets/4fd41be92a5e901be1ed8ff242bb24bd16da7d08.gif)
L'interprete ti informerà dove si trova l'errore e cosa lo ha causato. Tuttavia, questi messaggi potrebbero essere ingannevoli, poiché l'interprete non è in grado di seguire le tue esatte intenzioni e potrebbe rilevare errori a una certa distanza dalle loro reali cause.

Ad esempio, se provi a utilizzare un'entità con un nome sconosciuto, verrà generato un errore, ma l'errore verrà scoperto nel punto in cui si tenta di utilizzare l'entità, non dove è stato introdotto il nome della nuova entità.

In altre parole, il motivo vero e proprio si trova solitamente un po' prima nel codice, ad esempio nel punto in cui dovevi informare l'interprete che avresti utilizzato l'entità del nome.

Se la riga sembra buona, l'interprete tenta di eseguirla (nota: ogni riga viene solitamente eseguita separatamente, quindi il trio "leggi-controlla-esegui" può essere ripetuto molte volte, più volte del numero effettivo di righe nel file sorgente , poiché alcune parti del codice potrebbero essere eseguite più di una volta).

È anche possibile che una parte significativa del codice venga eseguita con successo prima che l'interprete trovi un errore. Questo è un comportamento normale in questo modello di esecuzione.

Ora potresti chiederti: quale è meglio? Il modello “compilativo” o il modello “interpretativo”? Non esiste una risposta ovvia. Se ci fosse stato, uno di questi modelli avrebbe cessato di esistere già da molto tempo. Entrambi hanno i loro vantaggi e i loro svantaggi.


# Compilation vs. Interpretation

![[Pasted image 20240319170007.png]]

- Python è un linguaggio interpretato. Ciò significa che eredita tutti i vantaggi e gli svantaggi descritti. Naturalmente, a entrambi aggiunge alcune caratteristiche uniche.
- Se volete programmare in Python, avrete bisogno dell'interprete Python. Senza di esso non sarà possibile eseguire il codice. Fortunatamente, Python è gratuito. Questo è uno dei suoi vantaggi più importanti.
- 
Per ragioni storiche, i linguaggi progettati per essere utilizzati in modo interpretativo sono spesso chiamati **linguaggi di scripting**, mentre i programmi sorgente codificati con essi sono chiamati **script**. Bene, conosciamo Python.


# Python – a tool, not a reptile :D

Python è un linguaggio di programmazione di alto livello, interpretato, orientato agli oggetti e con semantica dinamica, ampiamente utilizzato per la programmazione generale.

Sebbene il pitone sia conosciuto come un grosso serpente, il nome del linguaggio di programmazione Python deriva da una vecchia serie di sketch televisivi della BBC intitolata Monty Python's Flying Circus.

All'apice del successo, i Monty Python eseguivano i loro sketch davanti al pubblico di tutto il mondo, anche all'Hollywood Bowl.

Poiché Monty Python è considerato uno dei due nutrimenti fondamentali per un programmatore (l'altro è la pizza), il creatore di Python ha chiamato il linguaggio in onore dello show televisivo.


# Who created Python?

Una delle caratteristiche sorprendenti di Python è che si tratta del lavoro di una sola persona. Di solito, i nuovi linguaggi di programmazione vengono sviluppati e pubblicati da grandi aziende che impiegano molti professionisti e, a causa delle norme sul copyright, è molto difficile fare i nomi delle persone coinvolte nel progetto. Python è un'eccezione.

Non sono molti i linguaggi i cui autori sono noti per nome. Python è stato creato da Guido van Rossum, nato nel 1956 ad Haarlem, nei Paesi Bassi. Naturalmente, Guido van Rossum non ha sviluppato ed evoluto da solo tutti i componenti di Python...

La velocità con cui Python si è diffuso in tutto il mondo è il risultato del lavoro continuo di migliaia di programmatori (molto spesso anonimi), tester, utenti (molti dei quali non sono informatici) e appassionati, ma va detto che la primissima idea (il seme da cui Python è germogliato) è venuta a una sola testa: quella di Guido.


# A hobby programming project

Le circostanze in cui Python è stato creato sono un po' sconcertanti. Secondo Guido van Rossum:

Nel dicembre 1989, stavo cercando un progetto di programmazione "hobbistico" che mi tenesse occupato durante la settimana di Natale. Il mio ufficio (...) sarebbe stato chiuso, ma avevo un computer a casa e non molto altro a disposizione. Decisi di scrivere un interprete per il nuovo linguaggio di scripting a cui avevo pensato ultimamente: un discendente dell'ABC che sarebbe piaciuto agli hacker di Unix/C. Ho scelto Python come titolo provvisorio per il progetto, essendo di umore leggermente irriverente (e un grande fan del Monty Python's Flying Circus). Guido van Rossum

## Python goals

Nel 1999, Guido van Rossum ha definito i suoi obiettivi per Python:

- un linguaggio **facile e intuitivo**, potente quanto quelli dei principali concorrenti;
- **open source**, in modo che chiunque possa contribuire al suo sviluppo;
- un codice **comprensibile** come l'inglese;
- adatto alle **attività quotidiane**, consentendo tempi di sviluppo brevi.
Circa 20 anni dopo, è chiaro che tutte queste intenzioni sono state realizzate. Alcune fonti affermano che Python è il linguaggio di programmazione più diffuso al mondo, mentre altre sostengono che sia il secondo o il terzo.

In ogni caso, occupa ancora un posto di rilievo nella top ten del PYPL PopularitY of Programming Language e del TIOBE Programming Community Index.

Python non è più un linguaggio giovane. È maturo e affidabile. Non è un caso isolato. È una stella luminosa nel firmamento della programmazione e il tempo speso per imparare Python è un ottimo investimento.


# Why Python?

Com'è possibile che i programmatori, giovani e meno giovani, esperti o alle prime armi, vogliano usarlo? Com'è possibile che le grandi aziende abbiano adottato Python e abbiano implementato i loro prodotti di punta utilizzandolo?

Le ragioni sono molte, alcune le abbiamo già elencate, ma vediamo di elencarle nuovamente in modo più pratico:

- è **facile da imparare** - il tempo necessario per imparare Python è più breve rispetto a molti altri linguaggi; questo significa che è possibile iniziare la programmazione vera e propria più velocemente;
- è **facile da insegnare** - il carico di lavoro didattico è minore rispetto a quello richiesto da altri linguaggi; ciò significa che l'insegnante può porre maggiore enfasi sulle tecniche generali di programmazione (indipendenti dal linguaggio), senza sprecare energie in trucchi esotici, strane eccezioni e regole incomprensibili;
- è **facile da usare** per scrivere nuovo software - spesso è possibile scrivere codice più velocemente usando Python;
- è **facile da capire** - spesso è anche più facile capire più velocemente il codice di qualcun altro se è scritto in Python;
- è **facile da ottenere**, installare e distribuire - Python è gratuito, open source e multipiattaforma, cosa che non tutti i linguaggi possono vantare.

# Python rivals?


Python ha due concorrenti diretti, con proprietà e predisposizioni comparabili. Si tratta di:

- **Perl** - un linguaggio di scripting originariamente scritto da Larry Wall;
- **Ruby** - un linguaggio di scripting originariamente scritto da Yukihiro Matsumoto.

Il primo è più tradizionale e conservatore di Python e ricorda alcuni dei vecchi linguaggi derivati dal classico linguaggio di programmazione C.
Al contrario, il secondo è più innovativo e ricco di idee fresche rispetto a Python. Python stesso si colloca a metà strada tra queste due creazioni.


# Why not Python?


Nonostante la crescente popolarità di Python, ci sono ancora alcune nicchie in cui Python è assente, o è visto raramente:

- programmazione a basso livello (a volte chiamata programmazione "close to metal"): se si vuole implementare un driver o un motore grafico estremamente efficace, non si userebbe Python;
- applicazioni per dispositivi mobili: anche se questo territorio è ancora in attesa di essere conquistato da Python, molto probabilmente un giorno accadrà.


# There is more than one Python

## Python 2 vs. Python 3

Esistono due tipi principali di Python, chiamati Python 2 e Python 3.

Python 2 è una versione più vecchia del Python originale. Il suo sviluppo è stato intenzionalmente interrotto, anche se questo non significa che non ci siano aggiornamenti. Al contrario, gli aggiornamenti vengono rilasciati regolarmente, ma non sono destinati a modificare il linguaggio in modo significativo. Piuttosto correggono eventuali bug e falle di sicurezza appena scoperte. Il percorso di sviluppo di Python 2 è già arrivato a un punto morto, ma Python 2 stesso è ancora molto vivo.

Python 3 è la versione più recente (o, per essere più precisi, quella attuale) del linguaggio. Sta attraversando il proprio percorso evolutivo, creando i propri standard e le proprie abitudini.

Queste due versioni di Python non sono compatibili tra loro. Gli script Python 2 non funzionano in un ambiente Python 3 e viceversa, quindi se si vuole che il vecchio codice Python 2 venga eseguito da un interprete Python 3, l'unica soluzione possibile è quella di riscriverlo, non da zero, ovviamente, perché ampie parti del codice possono rimanere intatte, ma bisogna rivedere tutto il codice per trovare tutte le possibili incompatibilità. Purtroppo questo processo non può essere completamente automatizzato.

È troppo difficile, troppo lungo, troppo costoso e troppo rischioso migrare una vecchia applicazione Python 2 su una nuova piattaforma, ed è anche possibile che la riscrittura del codice introduca nuovi bug. È più semplice e sensato lasciare questi sistemi in pace e migliorare l'interprete esistente, invece di cercare di lavorare all'interno del codice sorgente già funzionante.


# Python implementations

Oltre a Python 2 e Python 3, esistono più di una versione di ciascuno di essi.

Secondo la pagina wiki di Python, un'implementazione di Python si riferisce a "un programma o un ambiente che fornisce supporto per l'esecuzione di programmi scritti nel linguaggio Python, come rappresentato dall'implementazione di riferimento CPython".

L'implementazione tradizionale di Python, chiamata CPython, è la versione di riferimento di Guido van Rossum del linguaggio informatico Python e viene spesso chiamata semplicemente "Python". Quando si sente il nome CPython, probabilmente lo si usa per distinguerlo da altre implementazioni alternative non tradizionali.

Ma prima di tutto. Ci sono i Python che sono mantenuti dalle persone riunite intorno alla PSF (Python Software Foundation), una comunità che mira a sviluppare, migliorare, espandere e divulgare Python e il suo ambiente. Il presidente della PSF è Guido von Rossum in persona e per questo motivo questi Python sono chiamati canonici. Sono anche considerati dei Python di riferimento, in quanto qualsiasi altra implementazione del linguaggio deve seguire tutti gli standard stabiliti dal PSF.

Guido van Rossum utilizzò il linguaggio di programmazione "C" per implementare la primissima versione del suo linguaggio e questa decisione è ancora in vigore. Tutti i Python provenienti dalla PSF sono scritti in linguaggio "C". Le ragioni di questo approccio sono molteplici. Uno di questi (probabilmente il più importante) è che grazie ad esso Python può essere facilmente portato e migrato su tutte le piattaforme che hanno la possibilità di compilare ed eseguire programmi in linguaggio "C" (praticamente tutte le piattaforme hanno questa caratteristica, il che apre molte opportunità di espansione per Python).

Per questo motivo l'implementazione di PSF viene spesso chiamata CPython. È il Python più influente tra tutti i Python del mondo.


# MODULE 1 TEST

ovviamente Aced, 100% eazy.


# MODULE 2

# # Section 1

```
print("Hello, World!")
```

La parola print che si vede qui è un nome di una funzione. Questo non significa che ovunque la parola appaia sia sempre un nome di una funzione. Il significato della parola deriva dal contesto in cui è stata usata.

Probabilmente avete già incontrato il termine funzione molte volte, durante le lezioni di matematica. Probabilmente potete anche elencare diversi nomi di funzioni matematiche, come il seno  o il log.

Le funzioni di Python, tuttavia, sono più flessibili e possono contenere più contenuti dei loro fratelli matematici.

Una funzione (in questo contesto) è una parte separata del codice del computer in grado di:

- causare un effetto (ad esempio, inviare un testo al terminale, creare un file, disegnare un'immagine, riprodurre un suono, ecc); questo è qualcosa di completamente sconosciuto nel mondo della matematica;
- valutare un valore (ad esempio, la radice quadrata di un valore o la lunghezza di un testo) e restituirlo come risultato della funzione; questo è ciò che rende le funzioni Python parenti dei concetti matematici.

Inoltre, molte funzioni Python possono fare le due cose insieme.

Le funzioni posso derivare da:

- **Python**
- **Da un modulo**
- **Dal nostro codice**



# Function arguments


Come abbiamo detto prima, una funzione può avere:

un effetto;
un risultato.
C'è anche un terzo componente della funzione, molto importante: gli argomenti.

Le funzioni matematiche di solito hanno un argomento. Ad esempio, sin(x) prende una x, che è la misura di un angolo.

Le funzioni di Python, invece, sono più versatili. A seconda delle esigenze individuali, possono accettare un numero qualsiasi di argomenti, quanti sono necessari per svolgere il loro compito. Nota: quando si parla di un numero qualsiasi, si intende anche lo zero; alcune funzioni Python non hanno bisogno di alcun argomento.

```
print("Hello, World!")
```

Nonostante il numero di argomenti necessari/forniti, le funzioni Python richiedono fortemente la presenza di una coppia di parentesi, rispettivamente di apertura e di chiusura.

Se si desidera fornire uno o più argomenti a una funzione, li si inserisce all'interno delle parentesi. Se si intende utilizzare una funzione che non accetta alcun argomento, le parentesi devono comunque essere presenti.

Nota: per distinguere le parole ordinarie dai nomi delle funzioni, si inserisce una coppia di parentesi vuote dopo i loro nomi, anche se la funzione corrispondente vuole uno o più argomenti. Questa è una convenzione standard.

La funzione di cui stiamo parlando è print().

La funzione print() del nostro esempio ha degli argomenti?

Certo che sì, ma quali sono?

## Stringa come argomento della funzione print()

In questo esempio, l'unico argomento fornito alla funzione print() è una stringa:

```
print("Hello, World!")
```

Come si può notare, la stringa è delimitata da virgolette; in effetti, le virgolette creano la stringa, tagliando una parte del codice e assegnandole un significato diverso.

![](https://skillsforall.com/content/pe1/1.0/m2/course/en-US/assets/ba89b9b996a37d871a1e4f8179b6f2ebbb1905d5.png)

#  Function invocation

Il nome della funzione (print in questo caso), insieme alle parentesi e agli argomenti, costituisce l'invocazione della funzione.

Cosa succede quando Python incontra un'invocazione come questa qui sotto?

```
function_name(argument)
```

Vediamo:

- Per prima cosa, Python controlla se il nome specificato è lecito (sfoglia i suoi dati interni per trovare una funzione esistente con quel nome; se questa ricerca fallisce, Python interrompe il codice)
- in secondo luogo, Python verifica se il numero di argomenti richiesti dalla funzione consente di invocare la funzione in questo modo (ad esempio, se una funzione specifica richiede esattamente due argomenti, qualsiasi invocazione che fornisca un solo argomento sarà considerata errata e interromperà l'esecuzione del codice)
- terzo, Python abbandona per un attimo il codice e salta alla funzione che si vuole invocare; naturalmente, prende anche gli argomenti e li passa alla funzione;
- quarto, la funzione esegue il suo codice, provoca l'effetto desiderato (se c'è), valuta il risultato desiderato (se c'è) e termina il suo compito;
- infine, Python ritorna al codice (al punto immediatamente successivo all'invocazione) e riprende la sua esecuzione.

È necessario rispondere al più presto a tre importanti domande:

1. Quale effetto provoca la funzione print()?

	L'effetto è molto utile e molto spettacolare. La funzione:
	
	- prende i suoi argomenti (può accettare più di un argomento e può anche accettarne meno di uno)
	- li converte in forma leggibile, se necessario (come si può sospettare, le stringhe non richiedono questa azione, poiché la stringa è già leggibile)
	- e invia i dati risultanti al dispositivo di output (di solito la console); in altre parole, tutto ciò che viene inserito nella funzione print() apparirà sullo schermo.
	Non c'è quindi da stupirsi se d'ora in poi utilizzerete molto spesso print() per vedere i risultati delle vostre operazioni e valutazioni.

2. Quali argomenti si aspetta print()?

	Qualsiasi. Vi mostreremo presto che print() è in grado di operare praticamente con tutti i tipi di dati offerti da Python. Stringhe, numeri, caratteri, valori logici, oggetti: ognuno di questi può essere passato con successo a print().

3. Quale valore restituisce la funzione print()?

	Nessuno. Il suo effetto è sufficiente.


# Python escape and newline characters

```
print("The itsy bitsy spider\nclimbed up the waterspout.")
print()
print("Down came the rain\nand washed the spider out.")
```

Il backslash (\) ha un significato molto particolare quando viene utilizzato all'interno delle stringhe: si tratta del cosiddetto carattere di escape.
La parola escape deve essere intesa in modo specifico: significa che la serie di caratteri della stringa sfugge per un momento (un momento molto breve) per introdurre un'inclusione speciale.

In altre parole, il backslash non ha un significato in sé, ma è solo una sorta di annuncio che il carattere successivo al backslash ha un significato diverso.

La lettera n posta dopo il backslash deriva dalla parola newline.

Sia il backslash che la n formano un simbolo speciale chiamato carattere newline, che invita la console a iniziare una nuova riga di output.

Questa convenzione ha due importanti conseguenze:
1. Se si vuole inserire un solo backslash all'interno di una stringa, non bisogna dimenticare la sua natura di escape: bisogna raddoppiarlo. Ad esempio, un'invocazione come questa causerà un errore:
```
print("\") ❌
```
mentre questa non lo farà:
```
print("\\") ✅
```
2. Non tutte le coppie di escape (il backslash accoppiato a un altro carattere) hanno un significato.

# Using multiple arguments

Finora abbiamo testato il comportamento della funzione print() senza argomenti e con un argomento. Vale anche la pena di provare ad alimentare la funzione print() con più di un argomento.

```
print("The itsy bitsy spider" , "climbed up" , "the waterspout.")

	Console >_ The itsy bitsy spider climbed up the waterspout.
```

Abbiamo usato una sola invocazione della funzione print(), ma contiene tre argomenti. Tutti sono stringhe.

Gli argomenti sono separati da virgole. Li abbiamo circondati con degli spazi per renderli più visibili, ma non è necessario e non lo faremo più.

In questo caso, le virgole che separano gli argomenti hanno un ruolo completamente diverso dalla virgola all'interno della stringa. La prima fa parte della sintassi di Python, mentre la seconda è destinata a essere visualizzata nella console.

Se si guarda di nuovo il codice, si vedrà che non ci sono spazi all'interno delle stringhe.

Gli spazi, rimossi dalle stringhe, sono ricomparsi. Potete spiegare perché?

Da questo esempio emergono due conclusioni:
- una funzione print() invocata con più di un argomento li visualizza tutti su una riga;
- la funzione print() inserisce di sua iniziativa uno spazio tra gli argomenti inviati.


```
print("My name is", "Python.")
print("Monty Python.")
```

Il modo in cui passiamo gli argomenti alla funzione print() è il più comune in Python ed è chiamato modo posizionale (positional way).
Questo nome deriva dal fatto che il significato dell'argomento è dettato dalla sua posizione (ad esempio, il secondo argomento verrà inviato dopo il primo e non viceversa).


# Keyword arguments

Python offre un altro meccanismo per il passaggio di argomenti, che può essere utile quando si vuole convincere la funzione print() a cambiare un po' il suo comportamento.

Non lo spiegheremo in modo approfondito in questo momento. Ci riserviamo di farlo quando parleremo delle funzioni. Per ora, vogliamo semplicemente mostrarvi come funziona. Sentitevi liberi di usarlo nei vostri programmi.

Il meccanismo si chiama " **keyword arguments**". Il nome deriva dal fatto che il significato di questi argomenti non deriva dalla loro posizione (position), ma dalla parola speciale (keyword) utilizzata per identificarli.

La funzione print() ha due argomenti parola chiave che possono essere utilizzati per i propri scopi. Il primo si chiama end.

```
print("My name is", "Python.", end=" ")
print("Monty Python.")
```

Per utilizzarlo, è necessario conoscere alcune regole:

un argomento a parola chiave è composto da tre elementi: una parola chiave che identifica l'argomento (termina qui); un segno di uguale (=); e un valore assegnato a quell'argomento;
gli argomenti delle parole chiave devono essere messi dopo l'ultimo argomento posizionale (questo è molto importante).
Nel nostro esempio, abbiamo utilizzato l'argomento parola chiave end e lo abbiamo impostato su una stringa contenente uno spazio.

Come si può notare, l'argomento della parola chiave end determina i caratteri che la funzione print() invia all'output una volta raggiunta la fine dei suoi argomenti posizionali.

Il comportamento predefinito riflette la situazione in cui l'argomento della parola chiave end viene utilizzato implicitamente nel modo seguente: end="\n".

Ora è il momento di provare qualcosa di più difficile.

Se si osserva attentamente, si noterà che abbiamo usato l'argomento end, ma la stringa assegnata ad esso è vuota (non contiene alcun carattere).

```
print("My name is ", end="")
print("Monty Python.")
```

Poiché l'argomento end è stato impostato a zero, anche la funzione print() non produce nulla, una volta esauriti i suoi argomenti posizionali.

Nota: non sono state inviate linee nuove all'output.

La stringa assegnata all'argomento della parola chiave end può essere di qualsiasi lunghezza. Sperimentate con essa se volete.

Abbiamo detto in precedenza che la funzione print() separa i suoi argomenti in uscita con degli spazi. Anche questo comportamento può essere modificato.

L'argomento della parola chiave che può farlo si chiama sep (_separator_).

```
print("My", "name", "is", "Monty", "Python.", sep="-")
```

La funzione print() ora utilizza un trattino, anziché uno spazio, per separare gli argomenti in uscita.

Nota: il valore dell'argomento sep può essere anche una stringa vuota. Provate voi stessi.

Entrambi gli argomenti delle parole chiave possono essere mescolati in un'unica invocazione, proprio come in questo caso:

```
print("My", "name", "is", sep="_", end="*")
print("Monty", "Python.", sep="*", end="*\n")
```


# # Section 2