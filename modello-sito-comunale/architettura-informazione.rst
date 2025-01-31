Architettura dell'informazione
================================

L'architettura dell'informazione definisce la struttura di un sito, il modo in cui le informazioni sono organizzate, i metodi di navigazione e la terminologia usata entro il sistema, al fine di facilitare l'accesso intuitivo ai contenuti e il completamento di compiti da parte degli utenti. L'architettura rappresenta la guida per la realizzazione delle strutture di front-end e di back-end del sito stesso.

Il `documento di architettura dell’informazione <https://docs.google.com/spreadsheets/d/1D4KbaA__xO9x_iBm08KvZASjrrFLYLKX/edit?usp=sharing&ouid=109069620194773449819&rtpof=true&sd=true>`_ presenta:

- le **tipologie di contenuto** e le loro proprietà, che servono a creare le varie pagine del sito;
- le **tassonomie** e i **vocabolari controllati**, utili a classificare i vari contenuti del sito per renderli fruibili tramite motore di ricerca interno e a definire la struttura di secondo e terzo livello del sito;
- la coreografia del sito, ovvero la **struttura (alberatura)**, il **sistema di navigazione** e i **tipi di pagina**.


L'architettura del sito di un Comune è organizzata in alcune sezioni principali, corrispondenti al primo livello di navigazione:

- *Amministrazione*, contiene tutti i contenuti riguardanti la struttura politica e amministrativa del comune, inclusi i documenti pubblici;
- *Novità*, raggruppa notizie e comunicati stampa;
- *Servizi*, presenta tutti i servizi che eroga il comune, sia quelli digitali, sia quelli fisici;
- *Vivere il comune*, presenta i luoghi d'interesse del territorio comunale e gli eventi;
- *Area personale*, dove gli utenti possono trovare i documenti personali, lo stato d'avanzamento delle loro richieste e i messaggi o notifiche inviati dall'amministrazione comunale.

Gli ulteriori livelli di navigazione sono specificati nella `sezione Navigazione e alberatura <../modello-sito-comunale/architettura-informazione.html#navigazione-e-alberatura>`_.

Ontologia e tipologie di contenuti
----------------------------------
L'ontologia del sito di un Comune quindi definisce gli oggetti (concreti o astratti), gli agenti (persone e ruoli), i contesti (i luoghi) ed gli eventi (esperienze, attività, servizi) utili alla rappresentazione del Comune su un sito web e attraverso cui gli utenti (i cittadini) interagiscono con il Comune stesso. Tutti questi elementi sono suddivisi in *Tipologie di contenuto* che presentano vari *attributi* (proprietà), che possono essere combinati per creare le pagine del sito. 

La definizione di un'ontologia è utile non solo per capire l'ordine e la disposizione dei contenuti sulle varie pagine, ma anche per promuovere l'interoperabilità dei dati e il loro riuso all'interno dello stesso dominio informativo (il sito comunale, in questo caso) o in domini informativi diversi.

Le **tipologie di contenuto** del sito di un Comune sono:

- Punto di contatto;
- Unità organizzativa;
- Persona pubblica;
- Incarico;
- Luogo;
- Notizia;
- Evento;
- Servizio;
- Documento pubblico;
- Dataset;
- Pratica;
- Pagamento;
- Documento privato;
- Messaggio;
- Appuntamento.

La lista delle Tipologie di contenuto è riportata anche nel `foglio Ontologia, Tassonomie e Coreografia <https://docs.google.com/spreadsheets/d/1D4KbaA__xO9x_iBm08KvZASjrrFLYLKX/edit#gid=2066775910>`_ del documento di architettura, con i link alle rispettive schede di dettaglio. La matrice "Corrispondenza Tipologie di contenuto/Tipologie di contenuto" mostra come queste sono combinabili tra di loro per formare le pagine del sito del Comune. 

Le schede di dettaglio delle tipologie di contenuto presentano la lista di *attributi* che vanno a formare l'effettivo contenuto. Gli attributi sono pezzi di informazione, rappresentabili principalmente valori testuali, booleani (vero o falso), numerici, temporali (data e ora) o categoriali, ma anche allegati digitali (file di documenti, immagini, video, audio).

.. important::
  Il documento di architettura dell'informazione indica, per ogni tipologia di contenuto, gli **attributi obbligatori** da includere a livello informativo e il loro ordine di presentazione.
  
Sulle relative schede sono anche presenti indicazioni sulle tassonomie di riferimento, le relazioni con altre tipologie di contenuti e la cardinalità, ovvero il possibile numero di occorrenze di un determinato attributo.
 


Tassonomie
-----------------------------------

Le tassonomie sono classificazioni gerarchiche di concetti, ovvero delle liste di nomenclature con cui si possono categorizzare i contenuti del sito. L'uso di tassonomie fornisce contesto ai contenuti e facilita la ricerca di contenuti correlati.

Le tassonomie del sito di un Comune sono:

- la lista degli argomenti di un Comune;
- Eventi della vita delle persone;
- Eventi della vita delle imprese;
- Tipi di unità organizzativa;
- Tipi di incarico;
- Tipi di notizia;
- Tipi di luogo;
- Tipi di evento;
- Categorie di servizi;
- Tipi di documento;
- Tipi punto di contatto;
- Documenti albo pretorio;
- Temi di un dataset;
- Frequenza di aggiornamento;
- Stati di una pratica;
- Licenze.

La lista delle tassonomie è riportata anche nel `foglio Ontologia, Tassonomie e Coreografia <https://docs.google.com/spreadsheets/d/1D4KbaA__xO9x_iBm08KvZASjrrFLYLKX/edit#gid=2066775910>`_ del documento di architettura, con i link alle rispettive schede di dettaglio. La matrice Tipologie/Tassonomie indica le relazioni tra le Tipologie di contenuto e le tassonomie.

Come si può vedere sulla schede dettaglio nel documento di architettura, le tassonomie presentano vari livelli di gerarchia e granularità. Nel classificare i contenuti (luoghi, eventi, notizie, etc.) bisogna usare il maggior livello di dettaglio possibile. Ad esempio, la pagina informativa di un convegno userà la tassonomia "Tipi di evento", e in particolare la voce di terzo livello "Convegno" ("Evento culturale" > "Conferenza e summit" > "Convegno").

Nelle pagine indice della categoria superiore è possibile, anzi consigliato, creare una sezione "In evidenza" dove riportare le voci delle categorie o delle sottocategorie che si ritengono più importanti, o le più recenti. Questa soluzione è utile sia nelle circostanze in cui nella categoria vi siano molte voci, per mettere in primo piano quelle considerate appunto più importanti, sia quando vi siano numerose sottocategorie con poche voci, in modo da permettere alle persone di trovarle senza dover cercare categoria per categoria.

Il content management system dovrebbe nascondere le categorie (temporaneamente) vuote.


Navigazione e alberatura
------------------------
La navigazione del sito del Comune è  definita nel `foglio Coreografia: sistema di navigazione <https://docs.google.com/spreadsheets/d/1D4KbaA__xO9x_iBm08KvZASjrrFLYLKX/edit#gid=1853196915>`_. È organizzata in forma gerarchica ed è chiamata *alberatura*, in quanto formata da una radice (l'homepage) da cui si diramano le varie sezioni, organizzate in pagine lista e pagine di dettaglio.

La struttura del sito è presentata agli utenti sotto forma di *menu di navigazione*.

La **navigazione principale** è formata dalle 4 sezioni in cui è organizzato il sito del comune: "Amministrazione", "Servizi", "Novità", "Vivere il comune", più "Area personale".

Le varie sezioni presentano, a loro volta, una struttura interna di secondo, terzo e, in alcuni casi, quarto e quinto livello. Per facilitare la navigazione degli utenti, si suggerisce di non andare oltre al terzo livello a meno che non sia strettamente necessario. 


La navigazione di secondo livello della sezione **Amministrazione** è suddivisa in:

- "Organi di governo", "Aree amministrative", "Uffici" ed "Enti e fondazioni", le cui sottostrutture sono definite dalla tassonomia "Tipi di unità organizzativa";
- "Politici" e "Personale amministrativo", le cui sottostrutture sono definite dalla tassonomia "Tipi di incarico";
- "Documenti e dati", la cui sottostuttura è definita dalla tassonomia "Tipi di documento".

La navigazione di secondo livello della sezione **Novità** è suddivisa in: "Notizie" e "Comunicati", le cui sottostrutture sono definite dalla tassonomia "Tipi di notizia";


La navigazione di secondo livello della sezione **Servizi** è suddivisa in una serie di pagine categoria e la struttura è informata dalla tassonomia "Categorie di servizi". Sotto ogni categoria, sono presenti le singole schede servizio, che vanno a formare il terzo livello.


La navigazione di secondo livello della sezione **Vivere il comune** è suddivisa in:

- "Luoghi", la cui sottostruttura è informata dalla tassonomia "Tipi di luogo".
- "Eventi", la cui struttura è informata dalla tassonomia "Tipi di evento".

L'etichetta di navigazione può essere, a scelta dei Comuni, o "Vivere il comune" o "Vivere <nomecomune>". Per i Comuni con nomi lunghi, è necessario usare la forma abbreviata (es. per il Comune di San Valentino in Abruzzo Citeriore, l'etichetta di navigazione sarà "Vivere San Valentino").


La navigazione di secondo livello dell'**Area personale** è suddivisa in: "Le mie pratiche", "Pagamenti", "Documenti", "Messaggi", "Scadenze" e "Profilo".

.. attention::
  Le tassonomie presenti nel documento di architettura hanno vari livelli, utili alla classificazione più o meno granulare dei contenuti e pensate per dare un ampio ventaglio di scelta. È possibile che un Comune non abbia contenuti che ricadano in tutte le voci delle tassonomie. In questi casi, soprattutto quando le tassonomie vengono usate per strutturare l'alberatura e la navigazione, bisogna eliminare le voci delle categorie che non presentano contenuti, in modo da non creare voci di navigazione e pagine vuote. 


Tipi di pagine
----------------------

Nel modello possiamo identificare i seguenti tipi di pagine:

- **pagine miste**, tra cui l'homepage e le pagine di primo livello della navigazione, che hanno lo scopo di indirizzare gli utenti ai vari contenuti del sito o della sezione specifica;
- **pagine lista**, che presentano una lista di contenuti simili o interrelati, come le pagine argomenti, novità e documenti.
- **pagine di dettaglio** o pagine foglia, ovvero le pagine che presentano contenuti specifici (persone, luoghi, servizi e così via).

Nell'area riservata, l'area del sito a cui si può accedere attraverso l'autenticazione, sono previste:

- l'homepage dell'area riservata;
- le pagine lista dei messaggi, delle pratiche e dei pagamenti.


Le pagine argomento
--------------------

La struttura flessibile basata sulla lista degli argomenti di un Comune permette di superare la
necessità di sviluppare e mantenere la maggior parte dei siti tematici
che spesso proliferano a fianco del sito istituzionale creando
problematiche di gestione, sviluppo e aggiornamento.

I contenuti già presenti nell’architettura del sito, infatti, possono
essere taggati con un argomento in modo da generare una pagina tematica
che li presenta. Ad esempio, se utilizziamo l’argomento “raccolta
differenziata” avremo una pagina che presenta agli utenti tutti i
contenuti relativi: servizi, documenti, notizie, uffici di riferimento.
Per arricchire la pagina di ulteriori contenuti sarà sufficiente
pubblicare nuovi contenuti usando le tipologie di contenuto già disponibili sul
sito (ad esempio una notizia, un documento, un servizio).

La pagina può essere ulteriormente personalizzata anche nell’aspetto
grafico con un’immagine di sfondo, un eventuale marchio e, se
necessario, una serie di pagine in evidenza. Ciascuna delle pagine
relative a un argomento è associata a un ufficio-area
dell’Amministrazione comunale, punto di riferimento per la qualità e la
correttezza delle informazioni offerte.

Un altro caso d’uso per un sito tematico è quello di dare voce agli
uffici che compongono l’amministrazione. Gli argomenti offrono agli
uffici la possibilità di gestire i propri contenuti e condividere le
proprie iniziative.


Struttura delle pagine
----------------------

Sebbene i componenti e i contenuti delle pagine siano diversi, la struttura principale è in buona parte comune. Tutte le pagine, infatti, sono formate da una intestazione (header), un'area principale (main) e da un'area piè di pagina (footer).

L'**intestazione (header)** è formata da tre componenti:

- l'intestazione iniziale (slim header) che deve contenere a sinistra l'ente di appartenenza (per i comuni, la regione o provincia autonoma di appartenenza) e a destra il link di accesso all'area personale, con l'etichetta "Accedi all'area personale". Una volta fatto l'accesso, verrà presentato l'avatar e il nome e cognome della persona autenticata, con la possibilità di accedere al profilo.
- l 'intestazione principale (header centrale) deve contenere il nome dell'istituzione (nel caso dei comuni, "Comune di nomecomune") eventualmente preceduta dal logo/stemma, può contenere le icone con il collegamento ai social network dell'ente, e deve contenere il link al motore di ricerca;
- l'intestazione di navigazione (header nav) deve contenere le voci di primo livello della navigazione e può contenere 4 ulteriori collegamenti (ad esempio, a pagine argomento). Il tema "Bootstrap Italia 2.0" definisce la visualizzazione e il comportamento dell'intestazione di navigazione sia in modalità desktop che mobile.


L'**area principale (main)** è composta da:

- una intestazione di pagina (ad eccezione dell'homepage, che ne è priva) che presenta le breadcrumb di navigazione, il titolo della pagina e un eventuale sottotitolo o descrizione breve, e gli argomenti con cui è stato taggato il contenuto. Può inoltre contenere la funzione di condivisione della pagina ed un menu che abilita altre azioni (ad esempo "Scarica", "Stampa", "Invia").

- la sezione con i contenuti principali, navigabili da un indice di pagina posto sulla sinistra.


Il **piè di pagina (footer)** deve contenere obbligatoriamente i contenuti e i collegamenti previsti dalla `normativa <https://www.normattiva.it/atto/caricaDettaglioAtto?atto.dataPubblicazioneGazzetta=2013-04-05&atto.codiceRedazionale=13G00076>`_:

- indirizzo, codice fiscale/partita IVA, contatti (compresa la posta elettronica certificata);
- riferimenti all'`amministrazione trasparente;
- l'informativa al trattamento dei dati personali;
- eventuali note legali;
- `la dichiarazione di accessibilità <https://www.agid.gov.it/it/design-servizi/accessibilita/dichiarazione-accessibilita>`_.

Inoltre, per i Comuni che accedono ai finanziamenti previsti nell'ambito della misura 1.4.1 per l'aggiornamento del sito, nel caso di performance negativa del sito secondo quanto calcolato e verificato dalla piattaforma PAdigitale2026 tramite le `librerie Lighthouse <https://web.dev/performance-scoring/>`_, il footer dovrà contenere:

- un piano di miglioramento del sito che mostri, per ciascuna voce che impatta negativamente la performance, le azioni future di miglioramento della performance stessa e le relative tempistiche di realizzazione attese.
