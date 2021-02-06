
# Progetto: (Yet Another) Product Ontology

### Docente: Prof.ssa Rossana Damiano

### Studenti: Ivan Spada e Federico Torrielli

---

# PARTE I

# Motivazioni

> Rilevanza del dominio scelto dal punto di vista culturale, professionale, sociale, ecc.

## Argomento scelto

Catalogo di prodotti e servizi di una generica azienda nell'ambito di vendita e noleggio di prodotti tecnologici. In
particolare, nel seguente documento analizziamo il caso di una multinazionale e la gestione del suo catalogo. Di
seguito, mostriamo una breve descrizione e la principale motivazione di sviluppo:

> Prendiamo in analisi i principali prodotti dell'azienda Apple, collocata nell'ambito tecnologico.

Sono trattati alcuni prodotti progettati e venduti in Italia a partire dall'anno 2016.

Alcuni esempi di prodotti venduti sono:

- iPhone
- iPad
- MacBook air & pro
- Apple Watch
- Accessori più venduti (vd. AirPods)

## Motivazione 1: catalogare per vendere più in fretta

All'interno di una grande azienda come Apple, che principalmente ha il focus di produrre **pochi** dispositivi con
simile design ma funzioni nettamente separate è utile avere un punto di riferimento dal punto di vista
dell'organizzazione della conoscenza per svariate motivazioni:

- Guidare il potenziale *buyer* a comprare il prodotto
- Evitare la confusione che è naturalmente generata dalla nomenclatura dei prodotti
- Offrire la possibilità di consultare l'archivio del prodotti

La motivazione principale della creazione di questa ontologia nasce, in verità, da qualcosa che Apple **non** mette a
disposizione dell'utente: un tool per confrontare dispositivi simili. Per essere più chiari, proponiamo un esempio:
> L'utente *x* ha la necessità di comprare un telefono iPhone ma ha a disposizione un budget limitato e ha il desiderio
> di alcune specifiche che solo la serie iPhone X propone: si trova però davanti ad al bivio che nasce dalla
> possibilità di comprare l'iPhone XS oppure XR. Oggi come oggi, non esiste alcun tool (che non sia una ricerca
> manuale) per effettuare questo tipo di confronto, nonostante la loro accurata catalogazione che provvedono a dare
> sul sito. Ovvero, sul sito Apple il confronto avviene esclusivamente in maniera testuale ma non è possibile, ad
> esempio, filtrare i contenuti per CPU.

Se il povero utente avesse avuto la possibilità di confrontare i prodotti per prezzo, si sarebbe accorto che l'azienda
vende il modello XR ad una cifra minore con (più o meno) la stessa qualità di prodotto.

## Motivazione 2: aggiornamento del catalogo

L'azienda ha deciso di riproporre i propri dispositivi anche gli anni successivi mutando la fascia di clientela a cui
erano precedentemente venduti. Alcuni dispositivi top di gamma dell'anno N risultano appartenenti alla fascia media
dell'anno N+1 permettendo il riutilizzo dei *vecchi device* allungando la vita degli articoli e riducendo le scorte
avanzate in magazzino allo stesso tempo. L'organizzazione del catalogo attraverso una rappresentazione della conoscenza,
aggiornabile nel tempo, permette la riorganizzazione delle proposte degli anni successivi in base alle scelte di *
marketing* stabilite dal *team* addetto all'interno dell'azienda.

# Requirements

> Requisiti per la creazione dell'ontologia: finalità, task, contesto e tipo di utenti a cui si rivolge

## Finalità

> Finalità generali della codifica formale del dominio

La costruzione del dominio della seguente ontologia ha come finalità l'utilizzo della stessa al fine di creare cataloghi
di prodotti facilmente aggiornabili, flessibili alle modifiche e su cui si possano effettuare delle operazioni di
ricerca (sia come applicazione, sia simil-DB). Dal punto di vista aziendale, diventa sempre più complicato gestire
cataloghi di prodotti, soprattutto se risultano simili se non identici: organizzando i dati secondo un'ontologia
gerarchica consultabile non solo si può usufruire più facilmente del catalogo (da cliente) ma diventa altrettanto
aggiornabile.

## Task e contesto

> I task specifici a cui è orientata e il contesto in cui si collocano

Il catalogo permette l'organizzazione dei prodotti venduti dall'azienda, tiene in considerazione le fasce di clientela a
cui gli articoli sono indirizzati e le possibili variazioni nel tempo seguendo le scelte commerciali e rispettando le
relazioni fra *items*. È possibile la consultazione della raccolta da parte dei clienti usufruendo di filtri in grado di
semplificare la ricerca, la lettura e il confronto con i *competitor*. Il contesto è la vendita e la consultazione dei
prodotti delle aziende.

## Utenti target

> Il tipo di utenti a cui si rivolge

- Utenti che devono consultare cataloghi ed effettuare ricerche su prodotti
- Aziende che devono catalogare prodotti e verificare/aggiornare la loro presenza in stock
- Altri utenti che devono confrontare prodotti diversi in base a specifiche caratteristiche dei singoli

# Descrizione

> Descrizione del dominio, con riferimenti bibliografici e/o sitografia

## Dominio

> Descrizione del dominio

Il dominio, collocato nell'ambito commerciale, ha come fine la rappresentazione dei prodotti delle aziende mettendoli in
relazione tra loro in base a prestazioni, qualità e *target*. Contiene le descrizioni degli articoli e le specifiche
tecniche, permette il confronto dei prodotti e la loro organizzazione utile alle aziende e ai clienti. Infine, mantiene
traccia delle proposte annuali disponibili sul mercato.

## Fonti

> Riferimenti bibliografici e sitografia

### Sitografia

Apple (Italy). Available at: *https://www.apple.com/it/*

Asus (Italy). Available at: *https://www.asus.com/it/*

Samsung (Italy). Available at: *https://www.samsung.com/it/*

# Documentazione sul dominio

> Qua verranno mostrati documenti informali, specifiche e standard esistenti ed
> un esempio reale che mostri il funzionamento della nostra ontologia.

## Ontologie similari ed ispirazione

Per trarre ispirazione della Simple IT Product Catalog si è partiti dalla già nota necessità di avere un ontologia dei
prodotti, di fantasia, che potesse esplicare concetti come "catalogo", "prodotto" e "device". Ci si è quindi accorti che
durante la costruzione della stessa si stava virando sempre più verso il concetto di
"ontologia per l'e-commerce": è stato quindi preso spunto da esempi come la
[Good Relations](http://www.heppnetz.de/projects/goodrelations/) ontology, un vocabolario web appositamente creato per
questo genere di utilizzi, sia da aziende che da altre ontologie che ne fanno utilizzo.

Nonostante Good Relations fosse un buon punto di partenza, si palesava il fatto che fosse nata principalmente a scopo di
SEO Tool per siti web che possedevano CMS (ad esempio un SEO per Wordpress!).

Figlia della già nota Good Relations, la [Product Ontology](http://www.productontology.org/) un'ontologia,
autoesplicativa nel nome, che fa riferimento a Wikipedia per esplicare i singoli prodotti, cui si è deciso di allinare
parecchie nostre definizioni per avere anche un punto di vista interessante su una ontologia pre-esistente. La Product
Ontology è davvero particolare in quanto non ha bisogno di manualmente "integrare" la sua T-BOX ed A-BOX per
l'ontologia, ma, come già accennato, prende in prestito le sue definizioni da Wikipedia, e le ordina come la comunità ha
deciso di allineare i concetti di partenza.

## Documenti informali

### Apple

La creazione dell'ontolgia si è ispirata all'organizzazione dei prodotti in catalogo di aziende come Apple, di cui è
possibile trovare sotto alcuni esempi

![Accessori1](https://i.ibb.co/K5mc9rH/image-2021-01-10-17-05-25.png)

> Macbook e iMac

![Accessori2](https://i.ibb.co/XLzLPdB/image-2021-01-10-17-06-16.png)

> iPad

![Accessori3](https://i.ibb.co/s68d5M7/image-2021-01-10-17-06-32.png)

> iPhone

![Accessori4](https://i.ibb.co/jJf4c8c/image-2021-01-10-17-06-43.png)

> Accessori e Apple Watch

Si può chiaramente vedere come la prima divisione fatta sia tramite "tipologia" di prodotto: i computer, poi i laptop, e
ancora gli iPad, iPhone ed infine gli accessori come Apple Watch e AirPods.

Accanto ad ogni categoria è poi possibile confrontare tipi equivalenti di prodotto
(ad es. laptop con laptop) tramite il menù "Confronta". Non è invece possibile fare confronti di prezzo sulle intere
categorie (che sarebbe uno degli obiettivi della nostra ontologia!).

È stato notato che la classificazione dei prodotti data da Apple è confusa e chiaramente tende a far notare a primo
impatto i prodotti più nuovi invece che i più venduti, cosa che invece siti come MediaWorld fanno, non essendo legati ad
un marchio soltanto.

### Samsung

![Samsung1](https://i.postimg.cc/SsFCmm95/image-2021-01-10-17-20-49.png)

Sul sito di Samsung si può già notare la differenziazione tra dispositivi portatili e non, cosa presente anche
all'interno della nostra ontologia e che chiaramente rende più semplice la visualizzazione di un catalogo di Prodotti
elettronici.

Il fatto che Samsung abbia un'organizzazione di questo tipo fa pensare che, a differenza di Apple, i suoi prodotti non
sono pensati per essere iconici, e che, ovviamente, il loro catalogo sia ben più vasto della già citata azienda di
Cupertino.

### Asus

![Asus1](https://i.postimg.cc/xCvHCByd/image-2021-01-10-17-22-25.png)

Qua è possibile visionare la divisione di vari computer da lavoro (sia fissi, che portatili, che ibridi). Più o meno si
adatta lo stesso pattern di Samsung, in quanto il modello di azienda è equiparabile.

## Organizzazione aziendale

La presenza di molteplici compagnie che hanno preso parte al ciclo produttivo degli articoli ha ispirato la
classificazione delle stesse per ruolo: progettazione e produzione.

Ogni azienda, nel ramo IT, o:

- Rappresenta la company che commissiona produzione e design
- Progetta solamente i prodotti
- Produce solamente i prodotti

Un esempio già citato è la Apple, che commissiona il design dei prodotti a Foxconn e la sua produzione di Chipset a
Qualcomm (non attualmente, ma è un buon esempio).

## Organizzazione user

I prodotti IT vengono spesso realizzati avendo in mente una tipologia (o target)
di clientela, come ad esempio la divisione delle serie (J,Z,M,A...) di Samsung.

In un catalogo di prodotti IT, più di altri, è importante ricordare che si tratta di vendere prodotti che solitamente
sono costosi: un catalogo che permetta la visualizzazione per fascia di prezzo è spesso apprezzato e aiuta la clientela
a scegliere prodotti per feature/prezzo e qualità/prezzo.

## Comparare i prodotti

![GalaxyZ](https://i.postimg.cc/k5p0Yhkf/image-2021-01-10-17-55-26.png)

Nel mondo dei device tecnologici forse il più importante fattore di scelta di un prodotto piuttosto che un altro sono le
sue specifiche tecniche. Nella precedente immagina possiamo notare come le diverse caratteristiche si dividano, a
seconda del dispositivo, nelle sue componenti interne.

Le stesse vengono anche utilizzate per proporre "comparison" (confronti)
tra dispositivi in modo da poter fare una scelta più accurata.

![Comparison](https://i.postimg.cc/pT5gwJvx/image-2021-01-10-18-04-35.png)

# Lode

[Qui il report LODE](http://150.146.207.114/lode/extract?url=https%3A%2F%2Fevilscript.altervista.org%2Fyapo.owl&lang=en)

# Visualizzazione

## Tassonomia delle classi

![Tassonomia di progetto](https://i.postimg.cc/yd7kxbw8/Modsem-taxonomy.png)

## Template utilizzati per i dati (GraphDB)

![Apple template](https://i.postimg.cc/13cL31hx/firefox-T1q-YKb-W2-Aj.png)

![iPhone12 64GB template](https://i.postimg.cc/QMFkncq6/firefox-BYsgoai6o-C.png)

## Triple di esempio

Si sono voluti selezionare due esempi (rispettivamente *yapo:Apple* e *yapo:iPhone12_64*)
per mostrare alcune delle triple più utilizzate nel progetto per descrivere istanze dell'ontologia: gli esempi sono *incompleti* di tutti i dati dell'ontologia.

![Apple](https://i.imgur.com/jwJfsSi.png)

Sono state incluse, come si può notare, anche alcune delle inferenze che tramite GraphDB vengono esplicitate qui in tabella.

Per quanto riguarda la colonna del contesto, è stata riportata ma il contesto accluso è quello di default
dell'applicazione.

![Apple2](https://i.imgur.com/bZ7zy0o.png)

## Esportazione Turtle

[L'esportazione Turtle si trova QUI](https://github.com/federicotorrielli/yapo/raw/master/Protege/turtle/yapo.owl)

---

# PARTE II

# Flusso d'iterazione utente

## Iterazione Utente

![Operazioni utente](https://i.postimg.cc/pVcdKR4V/iteration-schema.png)

## Schema di interfaccia: CLI

![CLI](https://i.postimg.cc/fWYPWhhw/cli.png)

## Esempio su terminale sipcp

[Esempio - ASCIINEMA](https://asciinema.org/a/58fTGH48YAQ50INdwq4rX4VlO)

## SPARQL

### Operazione 1

Descrizione:
dato il nome dell'azienda, restituisce tutti i prodotti che vende.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>

SELECT ?prod WHERE{
	?prod rdf:type yapo:Product.	
	?company rdf:type yapo:Company;
		yapo:sells ?prod.
	FILTER(?company = yapo:Apple)
}
```

Return:

- yapo:AirPods_wirelessCharge
- yapo:AppleWatchSeries6_40mm_GPS_Cellular_Nike
- yapo:Lightning_cable
- yapo:IpadAir_2020
- yapo:Iphone11_64
- yapo:MacBookAir_M1
- yapo:iMac_27_RetinaDisplay_5k_256
- yapo:iPhone12_64
- yapo:iPhoneX_64
- yapo:Beats_cuffie

### Operazione 2

Descrizione:
data una soglia di prezzo base P, restituisce tutti gli smartphone con prezzo >= P e relativi azienda e prezzo prodotto
ordinati per prezzo ASC.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>
PREFIX price: <http://www.ontologydesignpatterns.org/cp/owl/price.owl#>

SELECT ?prod ?brand ?price WHERE { 
	?brand rdf:type yapo:Company.
	?price rdf:type price:Price;
		price:hasValue ?v.
	?prod rdf:type yapo:Smartphone;
		yapo:hasBrand ?brand;
		price:hasPrice ?price.
	FILTER (?v >= '600'^^xsd:float)
}
ORDER BY ?price
```

Return:

- yapo:Iphone11_64 yapo:Apple yapo:600Euro
- yapo:iPhone12_64 yapo:Apple yapo:800Euro
- yapo:SamsungGalaxyS20_5G_global yapo:Samsung yapo:800Euro

### Operazione 3

Descrizione:
restituisce gli smartwatch che sono compatibili con uno smartphone, visualizza smartwatch, brand smartwatch, prezzo
smartwatch, smartphone compatibile.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>
PREFIX price: <http://www.ontologydesignpatterns.org/cp/owl/price.owl#>

SELECT ?smartw ?brand ?pricesmartw ?smartp WHERE { 
	?brand rdf:type yapo:Company.
	?pricesmartw rdf:type price:Price.
	?smartp rdf:type yapo:Smartphone.
	?smartw rdf:type yapo:Smartwatch;
		yapo:compatibleWith ?smartp;
		yapo:hasBrand ?brand;
		price:hasPrice ?pricesmartw.
}
```

Return:

- yapo:AppleWatchSeries6_40mm_GPS_Cellular_Nike yapo:Apple yapo:500Euro yapo:
  Iphone11_64
- yapo:AppleWatchSeries6_40mm_GPS_Cellular_Nike yapo:Apple yapo:500Euro yapo:
  iPhone12_64
- yapo:AppleWatchSeries6_40mm_GPS_Cellular_Nike yapo:Apple yapo:500Euro yapo:
  iPhoneX_64

### Operazione 4

Descrizione:
dato un prezzo base P per gli smarphone, restituisce gli smartwatch compatibili con gli smartphone con prezzo >= P, il
brand dello smartwatch e i prezzi dei due dispositivi. Ordinato per prezzo smartphone crescente.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>
PREFIX price: <http://www.ontologydesignpatterns.org/cp/owl/price.owl#>

SELECT ?smartw ?brand ?pricesmartw ?smartp ?pricesmartp WHERE { 
	?brand rdf:type yapo:Company.
	?pricesmartw rdf:type price:Price.
	?pricesmartp rdf:type price:Price;
		price:hasValue ?vsmartp.
	?smartp rdf:type yapo:Smartphone;
		price:hasPrice ?pricesmartp.
	?smartw rdf:type yapo:Smartwatch;
		yapo:compatibleWith ?smartp;
		yapo:hasBrand ?brand;
		price:hasPrice ?pricesmartw.
	FILTER (?vsmartp >= "600"^^xsd:float)
}
```

Return:

- yapo:AppleWatchSeries6_40mm_GPS_Cellular_Nike yapo:Apple yapo:500Euro yapo:
  Iphone11_64 yapo:600Euro
- yapo:AppleWatchSeries6_40mm_GPS_Cellular_Nike yapo:Apple yapo:500Euro yapo:
  iPhone12_64 yapo:800Euro

### Operazione 5

Descrizione:
data la scelta di uno smartphone in particolare, restituisce il cavo che è contenuto all'interno della confezione di
vendita.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>

SELECT ?smartp ?cable WHERE { 
	?cable rdf:type yapo:Cable.
	?smartp rdf:type yapo:Smartphone;
		yapo:containsInBox ?cable.
	FILTER(?smartp = yapo:Iphone11_64)
}
```

Return:

- yapo:Iphone11_64 yapo:Lightning_cable

### Operazione 6

Descrizione:
restituisce se nel catalogo Apple ci sono anche cuffie della BeatsAudio.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>

ASK {
	?company rdf:type yapo:Company;
	    yapo:sells ?earPlugs.
    ?earPlugs rdf:type yapo:EarPlugs.	
	?brand rdf:type yapo:Company;
		yapo:isBrandOf ?earPlugs.
	FILTER(?company = yapo:Apple && ?brand = yapo:BeatsAudio).
}
```

Return:

- YES

### Operazione 7

Descrizione:
data la scelta di uno device in particolare, restituisce gli altri dispositivi che hanno montata la medesima cpu.

Query:

```SPARQL
PREFIX wd: <http://www.wikidata.org/entity/>
PREFIX wdt: <http://www.wikidata.org/prop/direct/>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>

SELECT ?prodLabel WHERE {      
    ?device rdf:type yapo:Device;
          yapo:CpuType ?cpu.
    SERVICE <https://query.wikidata.org/sparql> {       
        ?chip wdt:P31 wd:Q610398;
          rdfs:label ?label;
          wdt:P1535 ?prod.
        ?prod rdfs:label ?prodLabel.
        FILTER (?device = yapo:Iphone11_64 && lang(?prodLabel) = "it" && lang(?label) = "it" && regex(?label, ?cpu)).
    } 
}
```

Return:

- "iPhone 11"@it
- "iPhone 11 Pro"@it
- "iPhone SE"@it

### Operazione 8

Descrizione:
data la scelta di un device in particolare, restituisce lo username Instagram del brand del device.

Query:

```SPARQL
PREFIX wd: <http://www.wikidata.org/entity/>
PREFIX wdt: <http://www.wikidata.org/prop/direct/>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>

SELECT ?usernameIG WHERE {      
    ?device rdf:type yapo:Device;
            yapo:hasBrand ?brand.
    ?brand rdf:type yapo:Company;
           rdfs:label ?labelbrand.
    SERVICE <https://query.wikidata.org/sparql> {       
        ?company wdt:P31 wd:Q4830453;
            wdt:P2003 ?usernameIG;
            rdfs:label ?labelCompany.
        FILTER (?device = yapo:Iphone11_64 && lang(?labelCompany) = "it" && STR(?labelCompany) = STR(?labelbrand)).
    } 
}
```

Return:

- "apple"

### Operazione 9

Descrizione:
dato un utente, restituisce i prodotti che ha acquistato.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>

SELECT ?prod WHERE{	
    ?prod rdf:type yapo:Product.
	?user rdf:type yapo:User;
		yapo:buysProduct ?prod.
	FILTER (?user = yapo:Giovanni_PowerUser)
}
```

Return:

- yapo:MacBookAir_M1
- yapo:iPhone12_64

---

## Altre query

### Query 1

Descrizione:
data un'azienda, restituisce le aziende che lavorano con la prima.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>

SELECT ?companyTo WHERE{
	?companyTo rdf:type yapo:Company.	
	?company rdf:type yapo:Company;
		yapo:manufacturesTo ?companyTo.
	FILTER(?company = yapo:Apple)
}
```

Return:

- yapo:BeatsAudio
- yapo:Foxconn
- yapo:Qualcomm
- yapo:ShortFactory

### Query 2

Descrizione:
dato un utente e uno specifico prodotto, registra l'acquisto del prodotto.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>

INSERT { 
	?buyer yapo:buysProduct ?prod.
} WHERE {
	?buyer rdf:type yapo:User.
	?prod rdf:type yapo:Product.
	FILTER(?buyer = yapo:Giovanni_PowerUser && ?prod = yapo:Iphone11_64)
}
```

Return:

- Added 1 statements.

### Query 3

Descrizione:
dato un utente e uno specifico prodotto, rimuove l'acquisto del prodotto.

Query:

```SPARQL
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX yapo: <https://evilscript.altervista.org/yapo.owl#>

DELETE { 
	?buyer yapo:buysProduct ?prod.
} WHERE {
	?buyer rdf:type yapo:User.
	?prod rdf:type yapo:Product.
	FILTER(?buyer = yapo:Giovanni_PowerUser && ?prod = yapo:Iphone11_64)
}
```

Return:

- Removed 1 statements.

# Documentazione del programma

## Simple IT Product Catalog Program

Programma terminale "sipcp" che permette non solo di fare delle query al SIPC ma di utilizzare l'endpoint GraphDB per
interfacciarsi con SPARQL verso fonti esterne come WikiData etc.. etc..

Il programma è completamente fatto in Python e non include una GUI.

Per utilizzarlo basta installarlo con il comando `pip install sipcp` ed utilizzarlo direttamente nel terminale nel
seguente modo:

> NB: la prima esecuzione del programma chiederà all'utente di inizializzare un file
> config.ini che conterrà l'URL di GraphDB in locale (o su server), da quel momento
> in poi sarà registrato in locale *nella cartella in cui è stato eseguito*

- `sipcp query "query qui"` effettua una query in-line, non sono permessi caratteri come virgolette quindi l'utilizzo
  rimane limitato alle query veloci e tipo "listing"
- `sipcp query-from-text` effettua tutte le query prendendole da un file di testo chiamato "do.txt"
  il file deve essere nella directory in cui si sta attualmente per eseguire il programma sipcp
- `sipcp query-product Compagnia` interroga yapo alla ricerca di tutti i prodotti dalla compagnia
  Compagnia. es: `sipcp query-product Apple` restituisce tutti i prodotti venduti dalla Apple
- `sipcp query-subcompanies Compagnia` similare a quello prima, interroga yapo restituendo tutte le
  compagnie che lavorano per la compagnia Compagnia.
- `sipcp myproducts User` effettua la ricerca di tutti i prodotti comprati da un utente nel catalogo, molto utile
  per il comando seguente
- `sipcp cputype Prodotto` effettua la ricerca del tipo di cpu del prodotto Prodotto
- `sipcp compatible-cables Smartphone` cerca tutti i cavi compatibili con lo smartphone specificato
- `sipcp compatible-smartphones` cerca tutte le opzioni di compatibilità tra smartwatch e smartphones
- `sipcp query-smartphone Prezzo` cerca tutti gli smartphones che costano di piu' della cifra specificata e li ordina
  dal meno costoso al piu' costoso
- `sipcp query_smartwatch_smartphone Prezzo` cerca tutti i match per compatibilità fra smartphone e smartwatch
- `sipcp search-brand Company Brand` cerca tutti i Brand che vendono venduti sul sito di Company
- `sipcp search-from-cpu Device` cerca tutti i devices su Wikidata che hanno la stessa CPU del device in input
- `sipcp search-ig-profile Device` cerca la pagina instagram su Wikidata della compagnia che vende il device Device.

Per invocare un help in formato internazionale, basta digitare `sipcp --help`
Supporta Python3.6 e le versioni successive.

## Note di esecuzione

sipcp nasce per essere eseguito su un terminale UNIX-like (Linux, MacOS...) e supporta la maggior parte dei terminali in
circolazione, eseguendo anche output colorato. Su Windows funziona in ogni caso, ma le differenze principali sono:

- Non si possono incollare sul terminale Query multi-lines per il comando `sipcp query ""`
- L'output non è colorato (sembra banale ma rende l'interazione interessante)

# Omeka-S per yapo

## Motivazioni della scelta dell'estensione

Tra le estensioni disponibili è stata scelta quella di Omeka-S, una piattaforma CMS che è in tutto e per tutto una
Linked Data Platform.

A differenza di GraphDB, Omeka ci ha dato molta più liberta di "giocare" con i dati a disposizione e creare individui e
resource templates utilizzando ciò che avevamo già in input, ma con un grado di modificabilità e visibilità maggiore
rispetto a GraphDB.

Come GraphDB possiamo effettuare query semantiche sulla KB e utilizzarle nelle pagine.

## Specifiche

La piattaforma è stata installata manualmente su un server pubblico dotato di Ubuntu 20.10, fatto un setup di MySql,
phpmyadmin e tutti gli strumenti necessari alla piattaforma per far lavorare il server senza intoppi.

Il link è pubblicamente accessibile [QUI](http://51.210.104.53/omeka/s/yapo/)

Dalla versione di base è stato modificato il tema pre-installato, giusto per dare un "tocco più e-commerce" alla
piattaforma.

## Items e Item sets

In Omeka gli individuals sono chiamati "items": ognuno di questi item fa riferimento ad un template per la sua creazione
chiamato il "resource template".

Sono stati creati, nel nostro caso, tre resource template rispettivamente per:

- brand: ovvero, le aziende che fanno dei prodotti
- inStock: ovvero, un prodotto che è correntemente nella condizione di essere in stock
- outOfStock: il complementare del precedente

Sono quindi stati definiti degli Item sets rispettivamente:

- inStockList: la lista degli item che sono inStock
- OutOfStockList: la lista degli item che sono outOfStock
- Brands: la lista dei brand

E poi, aggiunti degli items, come si può vedere nell'immagine:

![Item list](https://i.imgur.com/fJt2obp.png)

## Pagine

Sono state create delle pagine per contenere ognuna di queste liste:

- [Brands page](http://51.210.104.53/omeka/s/yapo/page/brands)
- [OutOfStock page](http://51.210.104.53/omeka/s/yapo/page/out-of-stock)
- [InStock page](http://51.210.104.53/omeka/s/yapo/page/in-stock)

Come si può vedere, ogni pagina rimanda ad una lista di prodotti o brand che sono del dominio specificato.

![Brands page](https://i.imgur.com/DP0NbcM.png)
![InStock page](https://i.imgur.com/Xvdmk9s.png)
![OutOfStock page](https://i.imgur.com/FHyq2p2.png)

Infatti, ognuna di queste pagine invia una query in-real-time al CMS semantico chiedendo la lista dei prodotti (o dei
brand), senza mai mantenere una vera e propria cache.

## Conclusione

Questo strumento mostra come anche un'azienda, attrezzata di un CMS come Omeka S, possa usufruire di questa tecnologia
per pubblicare un catalogo completo di prodotti
(e molto altro) alla fruizione del pubblico intero.
