# MODULO 1
Esistono 2 modalitá per vedere le connessioni tra i dispositivi in una rete. 
- Logical
	 Ignora ogni aspetto fisico della rete, e ci fornisce una visione "high level" della nostra topologia di rete
- Physical 
	 Tiene conto della scala fisica della nostra rete e della collocazione dei dispositivi nella rete.


Packet Tracer ci offre la possibilitá di creare 4 tipi di file diversi. Questi file sono usati per scopi differenti ed includono:

- .pka
	 Questo tipo di file é una attivitá. |"a" => activity|  Solitamente contiene una rete iniziale e una finale "answer network".  La rete finale non é accessibile a chi svolge l'attivitá in modo che non possa barare durante la costruzione della sua rete. 
- .pkt
	 Questo tipo di file contiene una rete qualsiasi (no attivitá) che viene salvata. Questa é una rete comune, non contiene challenge o istruzioni.
- .pksz
	 Questo tipo di file é usato per le Tutored Activities. Contiene un bundle con, un file .pka, degli assets e un file di scripting per dare suggerimenti all'utente. Queste attivitá offrono un supporto visivo, dei suggerimenti per il completamento delle sfide.
- pkz
	 Questo tipo di file é ormai obsoleto. Veniva usato nelle versioni precedenti.



PTSA (Packet Tracer Skills Assessments) e PTMO (Packet Tracer Media Objects)

- I PTSA sono valutazioni sommative delle competenze in cui si dimostra la propria abilità implementando le tecnologie apprese. I PTSA sono valutazioni autonome, hanno un proprio motore di valutazione e i risultati sono registrati nel libro dei voti del corso, se presente. Dopo aver completato un PTSA, si riceve un feedback a livello di elemento per ogni componente valutato.

- I PTMO possono essere file .pkt o .pka. Un PTMO viene visualizzato in linea con una domanda del quiz, dell'esame del modulo o di un altro tipo di valutazione. Il file .pkt o .pka viene lanciato direttamente dall'interno della valutazione. In genere, si configura la rete o si analizza la topologia, quindi si risponde a una o più domande di valutazione a scelta multipla.



# Build a Home Network  (PTTA)


Pre-Esercizio;

Per vedere l'IP di un PC si puó schiacciare il PC e andare nella config Tab, qui andare su FastEthernet0 (o la rete) e qui si vedono tutte le informazioni.
Oppure si va nel Desktop Tab e si apre il Command Prompt, qui si puó usare `ipconfig`.

Svolto in  +- 15 min
#  Create Realistic Structured Cabling in the Physical Workspace and Cabling Devices in a Rack (PTA)

- Part 1: Install a Patch Panel in the Wiring Closet
- Part 2: Attach a Wall Mount in the Office
- Part 3: Connect an Additional Wall Mount and Cables

Svolto in +- 20 min

---
# MODULO 2
# Connect Devices using Wireless Technologies (PTA)

- Part 1: Connect a Laptop to the Office WLAN
- Part 2: Connect Devices with Bluetooth Technology
- Part 3: Tether a Laptop to use a Cellular Network via the Smartphone

Svolto in +- 7 min


# Explore Device Configuration Using the CLI (console) (PTA)

- Part 1: Connect to the Device Using a Console Connection
- Part 2: Copy Configuration Information to the Device
- Part 3: Save the Updated Configuration to the Device

Svolto in +- 7 min

# Packet Tracer Simulation Mode (PTA)

Packet Tracer fornisce una modalità di simulazione che consente di creare e acquisire PDU (protocol data unit) per controllare diverse funzioni all'interno della rete, come:

- Connettività di base: tutti i dispositivi possono comunicare tra loro?
- Sicurezza: gli elenchi di accesso funzionano come previsto?
- Applicazioni e servizi: le applicazioni e i servizi come DNS, HTTP e FTP funzionano come previsto?

La modalità predefinita per Packet Tracer è la modalità Realtime. Nella modalità Tempo reale il tempo scorre continuamente come indicato dall'orologio nell'angolo in basso a destra dell'area di lavoro. Nella modalità Simulazione, il tempo può essere fermato o rallentato per consentire agli utenti di visualizzare il traffico dati un pacchetto alla volta. La modalità di simulazione viene utilizzata per osservare in dettaglio il traffico di rete con un tempo controllato direttamente dall'utente.

Dopo che le PDU sono state acquisite, sono disponibili diversi modi per visualizzarne il contenuto. La visualizzazione del contenuto delle PDU può essere utilizzata per verificare la connettività, verificare la funzionalità e risolvere i problemi. È anche un ottimo strumento per studiare o rivedere il contenuto degli strati del modello OSI e i meccanismi di comunicazione di rete.

Se visualizzato in modalità Modello OSI, viene visualizzato un riepilogo degli indirizzi e dei contenuti delle intestazioni su ciascun livello. Se si seleziona Dettagli PDU in entrata o in uscita, viene visualizzato il formato esatto delle intestazioni appropriate.


# Examine Packets in the Small Office (PTA)

- Part 1: Create a Simple PDU in Simulation Mode
- Part 2: View Contents of PDUs
- Part 3: Create a Complex PDU in Simulation Mode

Svolto in +- 10 min


# Edit Topologies (PTA)

- Part 1: Add an Additional Switch to the Rack in the Office Network
- Part 2: Connect a PC to the Office Network
- Part 3: Work with Clusters
- Part 4: Add a Second Home Cluster to the Network

Svolto in  +- 45 min (pranzo)


# Monitor Your Network Using a Network Controller (PTA)

- Part 1: Implement a Network Controller
- Part 2: Monitor the Network

Svolto in +- 17 min


# Manage and Configure your Network using a Network Controller (PTA)

Course Summary

Svolto in +- 11 min


# Troubleshoot a Wireless Connection (PTTA)

Learn to troubleshoot a wireless connection.

Svolto in +- 10 min

# Summary of this Course

**Lezione 1 - Set Up Your Small Office Network**

Il cablaggio strutturato è un approccio organizzato all'infrastruttura di cablaggio. Nella modalità fisica Packet Tracer è possibile utilizzare supporti a parete, cavi codificati a colori e creare punti di piegatura per organizzare il cablaggio di rete in modo realistico.

Molte reti sono parzialmente wireless e possono includere Wi-Fi, Bluetooth e dati cellulari. Le schede per la configurazione del dispositivo includono quanto segue:

- Fisico
- Config
- CLI
- Scrivania
- Servizi

Le schede visualizzate dipendono dal dispositivo che stai attualmente configurando.

La scheda CLI fornisce l'accesso all'interfaccia della riga di comando di un dispositivo Cisco. L'utilizzo della scheda CLI richiede la conoscenza della configurazione del dispositivo con Cisco Internetwork Operating System (IOS).

**Lezione 2 - Manage and Monitor Your Small Office Network**

Packet Tracer fornisce una modalità di simulazione che consente di creare e acquisire PDU per controllare diverse funzioni all'interno della rete, come:

- **Connettività di base** – Tutti i dispositivi possono comunicare tra loro?
- **Sicurezza** - Gli elenchi di accesso funzionano come previsto?
- **Applicazioni e servizi** - Applicazioni e servizi come DNS, HTTP e FTP funzionano come previsto?

La modalità in tempo reale in Packet Tracer mostra il tempo in esecuzione continua come indicato dall'orologio nell'angolo in basso a destra dell'area di lavoro. Nella modalità Simulazione, il tempo può essere fermato o rallentato per consentire agli utenti di visualizzare il traffico dati un pacchetto alla volta.

La visualizzazione del contenuto delle PDU può essere utilizzata per verificare la connettività, verificare la funzionalità e risolvere i problemi. Se visualizzato in modalità Modello OSI, viene visualizzato un riepilogo degli indirizzi e dei contenuti delle intestazioni su ciascun livello. Se si seleziona Dettagli PDU in entrata o in uscita, viene visualizzato il formato esatto delle intestazioni appropriate.

La progettazione della rete è un processo iterativo. Le reti vengono solitamente modificate dopo essere state costruite. Allo stesso modo, le reti Packet Tracer simulate che crei o con cui lavori potrebbero richiedere modifiche per apportare miglioramenti rispetto alla progettazione iniziale.

I controller di rete forniscono un modo centralizzato per monitorare e configurare più dispositivi di rete compatibili da un'unica GUI. È possibile accedere all'interfaccia del controller di rete collegando un browser Web all'indirizzo IP dell'interfaccia di gestione del controller di rete