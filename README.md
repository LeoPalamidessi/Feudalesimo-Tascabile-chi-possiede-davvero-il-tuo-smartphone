# Feudalesimo Tascabile: chi possiede davvero il tuo smartphone?

## L'illusione del possesso: lo compri, ma non ti appartiene mai

**Autore:** Leonardo Palamidessi (leonardo.palamidessi@proton.me)

**Data:** Ottobre 2026 \| **Versione:** 1.0

**Licenza:** [<u>CC BY
4.0</u>](https://creativecommons.org/licenses/by/4.0/deed.it)

**10.5281/zenodo.23457811**

**Nota redazionale:** Elaborazione testuale condotta con il supporto di
LLM per revisione strutturale; tesi, analisi e responsabilità dei
contenuti restano esclusive dell'autore.

## Executive Summary

Ho deciso di chiamare questo documento **"Feudalesimo Tascabile"**
perché secondo me non esiste un'immagine migliore per descrivere il
rapporto che abbiamo oggi con i nostri dispositivi. Nel Medioevo il
contadino pagava a caro prezzo gli attrezzi per lavorare la terra, ma
quel terreno non era mai davvero suo: apparteneva al signore feudale,
che decideva le regole, riscuoteva i pedaggi e poteva revocargli i
diritti in qualsiasi momento.

Con lo smartphone che abbiamo in tasca succede esattamente la stessa
cosa. Spendiamo centinaia o migliaia di euro convinti di aver comprato
un computer in miniatura, ma in realtà abbiamo pagato solo il metallo e
il vetro della scocca. Il cuore della macchina resta nelle mani del
produttore: attraverso licenze, bootloader blindati, fusibili fisici nel
processore (eFuse), controlli a distanza (*Remote Attestation*), blocchi
all'installazione libera delle app (*sideloading*) e pezzi di ricambio
serializzati (*parts pairing*), le grandi aziende tech si comportano
come i padroni assoluti del nostro hardware, riducendoci a semplici
ospiti in affitto a casa nostra. In nome di una finta sicurezza, ci
obbligano a tenere sui nostri dispositivi i loro sistemi operativi
proprietari, spesso appesantiti da software preinstallato non richiesto
(bloatware), servizi di telemetria invasivi e codice chiuso. Il
paradosso è che queste ROM commerciali finiscono per essere meno sicure
e meno longeve rispetto a sistemi operativi open source indipendenti,
progettati con codice verificabile e difese avanzate ma trattati
dall'industria come corpi estranei da bloccare.

Questa anomalia smette di essere un semplice problema per appassionati
di informatica nel momento in cui tocca i diritti fondamentali dei
cittadini. Oggi lo Stato e il sistema bancario ci obbligano a usare lo
smartphone per accedere alla sanità pubblica, per gestire i nostri
risparmi, per studiare, lavorare e usare i documenti d'identità digitali
(SPID, CIE, IT Wallet), ma invece di costruire queste piattaforme su
standard pubblici e aperti hanno delegato i controlli di sicurezza agli
ecosistemi privati di Google e Apple. Il risultato è un ricatto: se
decidi di esercitare la proprietà sul tuo telefono sbloccandolo o
installando un sistema operativo libero, vieni punito con l'esclusione
dalla vita civile ed economica. Per uscire da questo feudalesimo
digitale servono scelte tecniche e politiche nette: l'obbligo di sblocco
universale dei bootloader con la possibilità di caricare le proprie
chiavi crittografiche personali, la neutralità tecnologica della
Pubblica Amministrazione basata su protocolli davvero aperti e uno stop
definitivo ai blocchi sulle riparazioni e all'obsolescenza software
programmata.

## Indice dei Contenuti

[<u>Feudalesimo Tascabile: chi possiede davvero il tuo
smartphone?</u>](#feudalesimo-tascabile-chi-possiede-davvero-il-tuo-smartphone)

> [<u>L'illusione del possesso: lo compri, ma non ti appartiene
> mai</u>](#lillusione-del-possesso-lo-compri-ma-non-ti-appartiene-mai)
>
> [<u>Executive Summary</u>](#executive-summary)
>
> [<u>Indice dei Contenuti</u>](#indice-dei-contenuti)

[<u>Capitolo 1: Cosa Compriamo
Davvero?</u>](#capitolo-1-cosa-compriamo-davvero)

> [<u>1.1 Uno scontrino, due pesi e due
> misure</u>](#uno-scontrino-due-pesi-e-due-misure)
>
> [<u>1.2 Il ricatto della prima
> accensione</u>](#il-ricatto-della-prima-accensione)
>
> [<u>1.3 Dal PC aperto al silicio
> blindato</u>](#dal-pc-aperto-al-silicio-blindato)

[<u>Capitolo 2: Architettura Chiusa (Bootloader, DRM e Remote
Attestation)</u>](#capitolo-2-architettura-chiusa-bootloader-drm-e-remote-attestation)

> [<u>2.1 La catena di avvio e il bootloader
> blindato</u>](#la-catena-di-avvio-e-il-bootloader-blindato)
>
> [<u>2.2 Un processore diviso in due: TrustZone, TEE ed
> eFuse</u>](#un-processore-diviso-in-due-trustzone-tee-ed-efuse)
>
> [<u>2.3 L'attestazione remota: quando il telefono fa la spia contro il
> proprietario</u>](#lattestazione-remota-quando-il-telefono-fa-la-spia-contro-il-proprietario)
>
> [<u>2.4 Il ribaltamento del modello di sicurezza: l'utente trattato
> come un
> hacker</u>](#il-ribaltamento-del-modello-di-sicurezza-lutente-trattato-come-un-hacker)

[<u>Capitolo 3: La Cittadinanza Digitale e i Vincoli di Piattaforma
(CIE, SPID e Servizi
Pubblici)</u>](#capitolo-3-la-cittadinanza-digitale-e-i-vincoli-di-piattaforma-cie-spid-e-servizi-pubblici)

> [<u>3.1 Quando lo Stato delega i controlli alle
> multinazionali</u>](#quando-lo-stato-delega-i-controlli-alle-multinazionali)
>
> [<u>3.2 Il cortocircuito con la Costituzione e con il Codice
> dell'Amministrazione
> Digitale</u>](#il-cortocircuito-con-la-costituzione-e-con-il-codice-dellamministrazione-digitale)
>
> [<u>3.3 Tagliati fuori dalla vita quotidiana: banche, studio e
> lavoro</u>](#tagliati-fuori-dalla-vita-quotidiana-banche-studio-e-lavoro)

[<u>Capitolo 4: Il Mercato Bloccato e l'Impatto Reale (Concorrenza,
Obsolescenza ed
E-waste)</u>](#capitolo-4-il-mercato-bloccato-e-limpatto-reale-concorrenza-obsolescenza-ed-e-waste)

> [<u>4.1 La stretta sul sideloading e l'iniziativa
> \#KeepAndroidOpen</u>](#la-stretta-sul-sideloading-e-liniziativa-keepandroidopen)
>
> [<u>4.2 L'obsolescenza software programmata e la produzione forzata di
> rifiuti
> elettronici</u>](#lobsolescenza-software-programmata-e-la-produzione-forzata-di-rifiuti-elettronici)
>
> [<u>4.3 L'accoppiamento crittografico dei componenti (Parts Pairing) e
> il blocco della
> riparazione</u>](#laccoppiamento-crittografico-dei-componenti-parts-pairing-e-il-blocco-della-riparazione)

[<u>Capitolo 5: Soluzioni Tecnico-Normative e Proposte di
Policy</u>](#capitolo-5-soluzioni-tecnico-normative-e-proposte-di-policy)

> [<u>5.1 Le soluzioni tecniche e normative
> praticabili</u>](#le-soluzioni-tecniche-e-normative-praticabili)
>
> [<u>1. Portare il modello dei PC sugli smartphone: sblocco e chiavi
> personali (User Key
> Enrollment)</u>](#portare-il-modello-dei-pc-sugli-smartphone-sblocco-e-chiavi-personali-user-key-enrollment)
>
> [<u>2. Neutralità tecnologica della Pubblica Amministrazione e
> standard
> aperti</u>](#neutralità-tecnologica-della-pubblica-amministrazione-e-standard-aperti)
>
> [<u>3. Stop ai blocchi crittografici sui ricambi e calibrazione
> libera</u>](#stop-ai-blocchi-crittografici-sui-ricambi-e-calibrazione-libera)
>
> [<u>5.2 Risposta alle obiezioni
> dell'industria</u>](#risposta-alle-obiezioni-dellindustria)
>
> [<u>Obiezione 1: «Sbloccare il telefono e avere i permessi di root
> espone agli attacchi e mette a rischio le
> banche»</u>](#obiezione-1-sbloccare-il-telefono-e-avere-i-permessi-di-root-espone-agli-attacchi-e-mette-a-rischio-le-banche)
>
> [<u>Obiezione 2: «L'attestazione remota serve per proteggere il
> diritto d'autore e lo streaming
> (DRM)»</u>](#obiezione-2-lattestazione-remota-serve-per-proteggere-il-diritto-dautore-e-lo-streaming-drm)
>
> [<u>Obiezione 3: «Quelli che cambiano sistema operativo sullo
> smartphone sono pochissimi, non vale la pena fare una
> legge»</u>](#obiezione-3-quelli-che-cambiano-sistema-operativo-sullo-smartphone-sono-pochissimi-non-vale-la-pena-fare-una-legge)
>
> [<u>5.3 Proposte concrete per le Autorità di
> regolazione</u>](#proposte-concrete-per-le-autorità-di-regolazione)
>
> [<u>1. Cosa dovrebbe fare l'Antitrust
> (AGCM)</u>](#cosa-dovrebbe-fare-lantitrust-agcm)
>
> [<u>2. Cosa dovrebbero fare AgID e il Dipartimento per la
> Trasformazione
> Digitale</u>](#cosa-dovrebbero-fare-agid-e-il-dipartimento-per-la-trasformazione-digitale)
>
> [<u>3. Cosa dovrebbe fare il Garante per la
> Privacy</u>](#cosa-dovrebbe-fare-il-garante-per-la-privacy)
>
> [<u>4. Cosa dovrebbe fare la Commissione
> Europea</u>](#cosa-dovrebbe-fare-la-commissione-europea)
>
> [<u>Nota metodologica e sviluppi
> futuri</u>](#nota-metodologica-e-sviluppi-futuri)

[<u>Archivio Fonti e Riferimenti</u>](#archivio-fonti-e-riferimenti)

# Capitolo 1: Cosa Compriamo Davvero?

Chiunque studi informatica o abbia aperto almeno una volta un PC sa bene
che tra un computer e uno smartphone, a livello logico, non c'è alcuna
differenza. Dentro uno smartphone ci sono un processore, della memoria
RAM, uno storage e un sistema operativo che, nel caso di Android, si
basa persino sul kernel Linux. È un computer in miniatura, spesso più
potente dei portatili di qualche anno fa.

Però, nel momento in cui lo tiriamo fuori dalla scatola e lo accendiamo,
ci accorgiamo subito che qualcosa non torna. Pur avendo pagato per
intero ogni singolo grammo di silicio, vetro e alluminio, non abbiamo
quasi nessun controllo su cosa quel processore possa o non possa
eseguire. Senza che la maggior parte degli utenti se ne renda conto, il
mercato mobile ha svuotato dall'interno il concetto stesso di proprietà:
compriamo la macchina, ma a casa nostra ci comportiamo come semplici
inquilini in affitto.

## 1.1 Uno scontrino, due pesi e due misure

Quando compri un telefono, sullo scontrino c'è una voce sola e un prezzo
unico. A prima vista non c'è differenza rispetto all'acquisto di una
sedia, di un libro o di un elettrodomestico. Sul piano legale, però, non
appena il telefono si avvia quell'acquisto si spacca in due mondi
separati.

Da una parte c'è l'hardware, quindi il telefono vero e proprio: quello è
tuo al cento per cento. La legge ti riconosce il diritto di farne ciò
che vuoi, che sia smontarlo, rivenderlo o chiuderlo in un cassetto
[<u>\[1\]</u>](https://www.brocardi.it/codice-civile/libro-terzo/titolo-ii/capo-i/art832.html).
Dall'altra parte, però, ci sono il sistema operativo e il firmware
preinstallati. Quelli l'azienda non te li ha venduti: te li concede
soltanto in "licenza d'uso" attraverso un contratto scritto da lei
(l'EULA)
[<u>\[2\]</u>](https://eur-lex.europa.eu/legal-content/IT/TXT/?uri=CELEX:32009L0024).
In pratica il produttore resta il vero padrone del software e decide a
quali condizioni puoi usare il telefono che hai appena pagato
profumatamente.

## 1.2 Il ricatto della prima accensione

Il trucco sta nel fatto che queste due metà non possono essere separate.
Un processore senza il codice che lo avvia è solo un sasso metallico
costoso, tanto che oggi anche le leggi europee chiamano questi prodotti
«beni con elementi digitali», proprio perché senza il software l'oggetto
fisico smette di avere qualsiasi utilità
[<u>\[3\]</u>](https://eur-lex.europa.eu/eli/dir/2019/771/oj?locale=it).

Questo legame forzato trasforma la prima configurazione del telefono in
una finta scelta. Davanti alla schermata dei termini di servizio puoi
solo cliccare su "Accetto", cedendo il controllo sul dispositivo,
autorizzando la raccolta di telemetria a detta loro per “migliorare il
dispositivo” e sottoscrivendo condizioni talmente sbilanciate che spesso
sfiorano quelle che il Codice del Consumo chiama clausole vessatorie
[<u>\[4\]</u>](https://www.brocardi.it/codice-del-consumo/parte-iii/titolo-i/art33.html).

Sulla carta, i contratti dicono sempre che se non sei d'accordo con la
licenza puoi rifiutarla e restituire il dispositivo. Ma sfido chiunque
ad andare alla cassa con i sigilli della scatola aperti e il dispositivo
già acceso dicendo: «non sono d’accordo con quello che dice il contratto
del software», sai già come va a finire: nessuno ti ridà i soldi. Non
esiste nemmeno la possibilità di dire al produttore: «Tieniti pure il
tuo sistema operativo e lasciami il telefono vuoto così ci installo
quello che voglio io». O accetti le regole della casa, o il telefono
resta bloccato sulla schermata di benvenuto.

## 1.3 Dal PC aperto al silicio blindato

La cosa paradossale è che nel mondo dei PC questa battaglia era già
stata affrontata e vinta. Nel 2014, in Italia, una sentenza della Corte
di Cassazione ha stabilito che chi compra un computer con Windows
preinstallato ha tutto il diritto di rifiutare la licenza del sistema
operativo, tenersi il PC funzionante e farsi rimborsare il prezzo del
software
[<u>\[5\]</u>](https://www.aduc.it/generale/files/file/allegati/cassazione-rimborso-windows.pdf).

Ma al di là dei tribunali, sui PC tradizionali è l'architettura a essere
rimasta libera: su un fisso o su un portatile chiunque può entrare nel
BIOS, disattivare il Secure Boot (o caricare le proprie chiavi) e
installare da zero una distribuzione Linux. Sul computer l'utente è
l'amministratore di sistema, e la macchina esegue gli ordini di chi l'ha
comprata.

Con gli smartphone (esattamente come con le console da gioco)
l'industria ha capito che i contratti non bastavano più per tenere buoni
gli utenti. Basta guardare cosa succede oggi (16 ottobre 2026) con una
PlayStation 5: per impedire agli utenti di sbloccare il sistema (il
cosiddetto *jailbreak*), Sony sta utilizzando gli aggiornamenti di
sistema per rendere inutile (o quasi) la tua PS, perché se decidi di non
installare l'ultimo firmware, il dispositivo viene paralizzato: ti viene
bloccato l'accesso alla rete, non puoi più riscaricare i giochi che hai
regolarmente acquistato (o per meglio dire non puoi usare la licenza
d’uso che hai pagato), i titoli più recenti si rifiutano di partire e,
sui modelli più nuovi, non puoi nemmeno attivare il lettore Blu-ray
fisico appena montato, perché richiede per forza di collegarsi ai server
di Sony con l'ultimo aggiornamento installato. Se rifiuti
l'aggiornamento per mantenere il controllo sulla tua macchina, ti
ritrovi con un soprammobile inutilizzabile.

Sugli smartphone i produttori hanno spostato il divieto direttamente
dentro i circuiti: programmano i telefoni in fabbrica per rifiutare
qualsiasi codice che non abbia il loro timbro digitale
[<u>\[6\]</u>](https://source.android.com/docs/security/features/verifiedboot/avb?hl=it),
arrivando persino a inserire nel processore dei microscopici fusibili
fisici che si bruciano per sempre se provi a sbloccare i permessi di
root
[<u>\[7\]</u>](https://docs.samsungknox.com/admin/fundamentals/whitepaper/samsung-knox-mobile-security/system-security/hw-backed-security/).
Il risultato è un controsenso: per la legge sei il proprietario del tuo
smartphone, ma per il processore sei un estraneo non autorizzato.

# Capitolo 2: Architettura Chiusa (Bootloader, DRM e Remote Attestation)

Per capire come ci hanno tolto la proprietà dei nostri dispositivi non
basta leggere i contratti: bisogna guardare cosa succede dentro il
processore. Negli ultimi quindici anni i produttori di smartphone hanno
progettato l'hardware attorno a un obiettivo preciso: impedire
materialmente all'utente di modificare il software di basso livello,
anche quando ha il telefono fisicamente in mano.

## 2.1 La catena di avvio e il bootloader blindato

Quando premiamo il tasto di accensione di uno smartphone, il sistema
operativo non parte subito. Si avvia invece una catena di eventi
crittografici chiamati catena di fiducia (*Chain of Trust*).

La prima cosa che parte è un minuscolo programma inciso direttamente nel
silicio durante la fabbricazione del chip, dentro una memoria di sola
lettura chiamata Boot ROM. Nessuno può modificarlo o cancellarlo, e al
suo interno sono stampate le chiavi crittografiche del produttore
[<u>\[8\]</u>](https://support.arm.com/documentation/dai0527/a/). La
Boot ROM controlla la firma digitale del primo stadio del bootloader: se
la firma è quella ufficiale del costruttore lo fa partire, altrimenti
rimane in uno stato di continuo riavvio. Il bootloader fa esattamente la
stessa cosa con lo stadio successivo, fino ad arrivare al caricamento in
RAM del kernel. Anche qui, prima di far partire il sistema, il
bootloader calcola l'impronta crittografica (l'hash) dei file di avvio e
verifica che coincida con le firme salvate in una partizione speciale
chiamata vbmeta
[<u>\[9\]</u>](https://source.android.com/docs/security/features/verifiedboot/boot-flow?hl=it).

Finché il bootloader resta bloccato questa catena non ammette eccezioni:
se provi a caricare un kernel compilato da te o un sistema operativo
diverso da quello originale, il controllo della firma fallisce e il
telefono si rifiuta di avviarsi.

Per installare un sistema alternativo bisogna quindi sbloccare il
bootloader. Ed è proprio qui che si vede tutta la differenza tra un PC e
uno smartphone. Su un computer tradizionale questo meccanismo si chiama
Secure Boot, ma è il proprietario a decidere il da farsi: basta entrare
nel BIOS per disattivarlo o per inserire le proprie chiavi personali.
Nel mondo degli smartphone, invece, decidono i produttori. Alcuni marchi
vietano del tutto lo sblocco, non lasciando agli utenti altra scelta se
non cercare falle di sicurezza (exploit) per aggirare il blocco sul
proprio dispositivo. Altri trasformano lo sblocco in una gentile
concessione pressoché impossibile dall'alto: ti obbligano a creare un
account proprietario, a collegare il telefono ai loro server, aspettare
un mese intero e sperare che ti diano l’ok per sbloccare il tuo
telefono. Solo pochissimi produttori (come OnePlus, Pixel o Nothing)
permettono ancora di sbloccare il bootloader in modo pulito con un
semplice comando dal computer, lasciando in rari casi anche la
possibilità di caricare le proprie chiavi crittografiche
[<u>\[10\]</u>](https://source.android.com/docs/security/features/verifiedboot/device-state?hl=it).

Ma anche quando trovi un telefono sbloccabile e riesci a installare il
sistema operativo che vuoi, la libertà costa caro... I produttori hanno
infatti spostato la trappola un gradino più in alto: il telefono accetta
pure di avviarsi, ma segna la modifica nei suoi registri interni e ti
taglia fuori dai servizi di tutti i giorni.

## 2.2 Un processore diviso in due: TrustZone, TEE ed eFuse

Chi mastica un po' di informatica sa che nei sistemi operativi
tradizionali (come Linux sui PC) ottenere i permessi di root
(amministratore) significa avere il potere assoluto sulla macchina. Con
i permessi di root puoi leggere qualsiasi area della memoria, fermare
qualsiasi processo e modificare ogni singolo file del sistema. Sugli
smartphone moderni non funziona più così.

I processori ARM che troviamo nei telefoni di oggi sono letteralmente
divisi in due mondi separati a livello hardware grazie a una tecnologia
chiamata TrustZone
[<u>\[11\]</u>](https://developer.arm.com/-/media/Arm%20Developer%20Community/PDF/Learn%20the%20Architecture/TrustZone%20for%20Armv8-A.pdf).
Da una parte c'è “la superficie” (*Rich Execution Environment* o REE),
che è lo spazio in cui girano il kernel Linux, Android (o la nostra
custom ROM) e tutte le app che usiamo ogni giorno. Dall'altra parte,
dentro lo stesso chip, c'è il “sottosuolo” (*Trusted Execution
Environment* o TEE): una vera e propria cassaforte isolata nel silicio,
con una sua porzione di memoria dedicata e un suo mini-sistema operativo
separato e invisibile al resto dello smartphone
[<u>\[12\]</u>](https://globalplatform.org/wp-content/uploads/2022/05/GPD_SPE_009-GPD_TEE_SystemArchitecture_v1.3_PublicRelease_signed.pdf).

Quando fai il root sul telefono o installi una ROM alternativa, diventi
amministratore soltanto della superficie. Il sottosuolo continua a
tenerti fuori: il kernel non può leggere la memoria del TEE, non può
vedere cosa sta calcolando e non può toccare le chiavi crittografiche
chiuse là dentro, perché sono i circuiti stessi della scheda madre a
bloccare elettricamente l'accesso.

Come se non bastasse, a fare la guardia a questo confine ci sono i
cosiddetti **eFuse**, cioè dei microscopici fusibili fisici integrati
nel processore che possono essere bruciati con un impulso elettrico
[<u>\[13\]</u>](https://docs.samsungknox.com/admin/fundamentals/whitepaper/samsung-knox-mobile-security/system-security/hw-backed-security/).
L'esempio più famoso è Knox sugli smartphone Samsung: nel preciso
istante in cui sblocchi il bootloader e avvii un sistema non firmato da
Samsung, il telefono manda una piccola scarica che brucia fisicamente
quel fusibile, facendo scattare il valore da 0x0 a 0x1. Da quel momento
non c'è ritorno: anche se rimetti il software originale di fabbrica e
riblocchi tutto, il fusibile bruciato non si ripara. Il telefono
continua ad accendersi, ma funzioni come Samsung Wallet o l'Area
Personale smettono di funzionare per sempre.

## 2.3 L'attestazione remota: quando il telefono fa la spia contro il proprietario

A questo punto si potrebbe pensare: «Va bene, rinuncio alle app del
produttore, sblocco il telefono, ci metto un sistema operativo
alternativo e sto tranquillo». È qui che entra in gioco l'arma più
efficace contro di noi: l'attestazione remota (*Remote Attestation*).

Su un computer, se un programma vuole sapere se il sistema è stato
modificato, deve chiederlo al sistema operativo stesso; e visto che
l'utente sul proprio PC è amministratore, può sempre configurare il
sistema per rispondere che è tutto a posto. Per togliere all'utente
questa possibilità sugli smartphone, la verifica è stata spostata dentro
il chip di sicurezza (il TEE o un processore separato chiamato *Secure
Element* / *StrongBox*)
[<u>\[14\]</u>](https://source.android.com/docs/security/features/keystore?hl=it).
Quando il telefono viene assemblato in fabbrica, dentro questa
cassaforte hardware viene salvata una chiave crittografica privata che
non può mai uscire dal chip, accompagnata da un certificato firmato alla
radice dal produttore del processore.

Ogni volta che apri un'app bancaria, un wallet digitale o un servizio
che usa i controlli di Google (come le **Play Integrity API** o la *Key
Attestation*), dietro le quinte avviene un interrogatorio: il server
dell'app manda al telefono un codice casuale (un *nonce*), il chip di
sicurezza va a leggere direttamente nei registri hardware se il
bootloader è sbloccato e chi ha firmato il sistema operativo in uso,
dopodiché firma questo controllo con la sua chiave privata di fabbrica e
la spedisce ai server esterni
[<u>\[15\]</u>](https://developer.android.com/google/play/integrity/overview?hl=it).

Tu, da proprietario del telefono, non puoi intrometterti né falsificare
quella risposta, perché anche avendo i permessi di root non hai accesso
alla chiave privata chiusa nel silicio. Se hai installato un sistema
operativo non approvato o hai sbloccato i permessi di amministratore,
l'attestazione fallisce e scatta la “punizione”: le app delle banche si
rifiutano di partire, i pagamenti contactless con Google Wallet vengono
disattivati, le app dei servizi pubblici ti bloccano l'accesso dicendo
che il dispositivo è "manomesso" e persino i sistemi di protezione video
(i DRM come Widevine) declassano il telefono dal livello hardware L1 al
livello L3, impedendoti di guardare un film in alta definizione sulle
piattaforme di streaming a cui sei regolarmente abbonato
[<u>\[16\]</u>](https://source.android.com/docs/core/media/drm?hl=it).

La cosa più grave è che questo sistema di verifica non si basa su uno
standard pubblico, aperto o controllato da un ente indipendente: passa
interamente per le regole e per i server privati di Google
[<u>\[17\]</u>](https://source.android.com/docs/compatibility/cdd?hl=it).
Nessun altro può certificare che un sistema operativo alternativo è
sicuro.

L'assurdità di questo monopolio si vede benissimo con progetti come
**GrapheneOS**, un sistema operativo open source progettato
specificamente per la massima sicurezza
[<u>\[18\]</u>](https://grapheneos.org/articles/attestation-compatibility-guide).
GrapheneOS non dà di default i permessi di root e permette di ribloccare
il bootloader del telefono usando le proprie chiavi crittografiche e
inoltre ha difese contro i malware molto più avanzate rispetto ai
sistemi preinstallati dai produttori. Quindi, nonostante l'hardware sia
perfettamente integro e il bootloader sia chiuso, le Play Integrity API
(a ottobre 2026) gli negano il bollino di conformità del dispositivo
(MEETS_DEVICE_INTEGRITY) semplicemente perché non monta il pacchetto
proprietario certificato da Google. Ricapitolando: uno smartphone
aggiornatissimo, con codice open source e blindato con GrapheneOS viene
respinto dalle app bancarie come "non sicuro", mentre un telefono
economico abbandonato dal produttore tre anni fa e pieno di falle non
corrette passa i controlli senza problemi, solo perché ha ancora il
software commerciale di fabbrica. E nel frattempo banche, aziende e
pubbliche amministrazioni, invece di farsi carico della sicurezza delle
proprie app, si limitano a delegare tutto a Google, lasciando che sia
una singola multinazionale a decidere chi può usare i servizi digitali e
chi no.

## 2.4 Il ribaltamento del modello di sicurezza: l'utente trattato come un hacker

Nella storia dell'informatica, la sicurezza ha sempre avuto uno scopo
chiaro: difendere il proprietario del computer dagli attacchi esterni.
Nei sistemi classici l'utente amministratore ha il controllo totale e le
difese servono a impedire che un virus o un criminale gli rubino il
controllo della macchina.

Con gli smartphone moderni e con quella filosofia industriale che prende
il nome di *Trusted Computing*, questo principio è stato letteralmente
capovolto
[<u>\[19\]</u>](https://www.cl.cam.ac.uk/archive/rja14/tcpa-faq.html).
Oggi, per il telefono che hai in tasca, il nemico da cui difendersi non
è solo l'hacker esterno, **ma tu stesso che lo hai comprato**. Tutto
l'arsenale che abbiamo visto fin qui (dalla Boot ROM blindata al TEE,
dai fusibili che si bruciano fino all'attestazione remota) non è stato
progettato solo per proteggere i tuoi dati, ma soprattutto per
proteggere gli interessi dei produttori dalle tue mani
[<u>\[20\]</u>](https://youtu.be/HUEvRyemKSg?si=SAFIU8EPaNtVbNsk).

Basta guardare come sono cambiate le parole. Se sul tuo portatile prendi
i permessi di amministratore, stai semplicemente gestendo il tuo
computer; se fai la stessa identica cosa sul tuo smartphone, il sistema
dichiara il dispositivo "compromesso" (*tampered*) e inizia a spegnere
le funzioni una dopo l'altra. Persino la parola "fiducia" (*trust*) ha
cambiato significato: per l'industria tech un dispositivo "fidato" non è
un computer di cui il proprietario può fidarsi, ma un terminale di cui
le aziende possono fidarsi perché sanno che disobbedirà a chi ci ha
speso soldi. Così lo smartphone smette di essere un vero computer nelle
nostre mani e diventa un terminale controllato a distanza, di cui noi
siamo soltanto gli utilizzatori finali.

# Capitolo 3: La Cittadinanza Digitale e i Vincoli di Piattaforma (CIE, SPID e Servizi Pubblici)

Finché il blocco di uno smartphone ti impedisce di usare un'app privata
o di vedere una serie TV in alta definizione, la questione può sembrare
solo un litigio di basso conto tra chi compra il telefono e chi lo
produce. Il problema cambia completamente scala quando di mezzo ci
finiscono i diritti fondamentali del cittadino.

Negli ultimi anni lo Stato ha spostato online quasi tutti i suoi
sportelli: oggi lo smartphone non è più un semplice oggetto di svago, ma
è diventato lo strumento indispensabile per dialogare con la Pubblica
Amministrazione. Serve per aprire il Fascicolo Sanitario Elettronico,
per controllare i contributi all'INPS, per pagare le tasse e per
dimostrare la propria identità online. Il guaio è che le istituzioni,
invece di appoggiare questa infrastruttura pubblica su standard aperti e
indipendenti, hanno iniziato a delegare i controlli di sicurezza delle
app di Stato ai sistemi proprietari di due multinazionali americane:
Google e Apple. Così facendo, l'esercizio dei diritti di cittadinanza
finisce per dipendere dal permesso di un'azienda privata che liberamente
decide cosa possiamo o non possiamo fare con il nostro hardware.

## 3.1 Quando lo Stato delega i controlli alle multinazionali

In Italia l'accesso ai servizi pubblici digitali passa ormai da due
chiavi principali: lo SPID e la Carta d'Identità Elettronica (CIE), che
per i livelli di sicurezza più alti richiedono l'uso di app per
smartphone come CieID o quelle dei vari gestori accreditati
[<u>\[21\]</u>](https://github.com/italia/cieid-android-sdk). A queste
si è aggiunta l'App IO, che con l'introduzione dell'IT Wallet permette
di portare direttamente sul telefono i documenti digitali con valore
legale, come la patente di guida e la tessera sanitaria.

Dal punto di vista informatico, per garantire la sicurezza di queste
operazioni basterebbe usare protocolli crittografici aperti e
standardizzati a livello internazionale (come FIDO2 o WebAuthn). Invece,
nello sviluppo dell'IT Wallet dentro l'App IO, si è scelto di prendere
la scorciatoia più semplice e closed source: integrare direttamente le
Google Play Integrity API e i controlli di attestazione hardware di
Apple. Come è emerso chiaramente nelle discussioni pubbliche sul codice
sorgente di App IO su GitHub, l'applicazione interroga i server di
Google per verificare il telefono e blocca l'attivazione dei documenti
nell'IT Wallet su qualsiasi dispositivo con permessi di root, bootloader
sbloccato o con un sistema operativo alternativo come GrapheneOS
[<u>\[22\]</u>](https://github.com/pagopa/io-app/issues/6327). E non si
tratta di un caso isolato italiano: la stessa identica impostazione
tecnica si sta facendo strada anche a livello europeo nello sviluppo del
nuovo portafoglio digitale continentale (l'European Digital Identity
Wallet o EUDI)
[<u>\[23\]</u>](https://github.com/eu-digital-identity-wallet/eudi-app-android-wallet-ui/issues/287).

Basta fermarsi un attimo a riflettere sulla dinamica per capire quanto
sia assurda questa cosa. Un cittadino italiano possiede un documento
d'identità valido, rilasciato dal Ministero dell'Interno e dotato di un
chip crittografico che da solo basterebbe a garantire chi sei. Eppure,
nel momento in cui prova a usare le funzioni digitali legate ai suoi
documenti su uno smartphone di sua proprietà, l'app pubblica chiede il
permesso ai Google Play Services. Se l'utente ha deciso di sbloccare il
proprio telefono o di usare un sistema operativo libero, Google non dà
l’ok e l'app di Stato gli sbarra la porta in faccia. In pratica abbiamo
privatizzato la validità dei documenti pubblici: non è più lo Stato a
certificare che la tua identità digitale è valida, ma è un'azienda
privata californiana a decidere se il tuo telefono merita o meno di far
girare i tuoi documenti.

## 3.2 Il cortocircuito con la Costituzione e con il Codice dell'Amministrazione Digitale

Appaltare i controlli d'ingresso dei servizi pubblici a piattaforme
commerciali private non è solo una pessima scelta ingegneristica: crea
uno scontro frontale con le leggi italiane e con la nostra stessa
Costituzione.

Il primo problema riguarda proprio l'articolo 3 della Costituzione, cioè
il principio di uguaglianza
[<u>\[24\]</u>](https://www.senato.it/istituzione/la-costituzione/principi-fondamentali/articolo-3).
Il secondo comma dice chiaramente che è compito della Repubblica
rimuovere gli ostacoli economici e sociali che limitano di fatto la
libertà e l'uguaglianza dei cittadini e la loro partecipazione alla vita
del Paese. Se lo Stato rende obbligatoria l'identità digitale per
accedere alla sanità, al fisco o alla previdenza, ma poi permette di
usarla solo su telefoni "benedetti" da Google o da Apple, sta creando
lui stesso un ostacolo artificiale e una discriminazione. Da un lato
taglia fuori chi, per tutelare la propria privacy, decide legittimamente
di non firmare un contratto con Google o Apple e di non farsi profilare
dalla loro telemetria; dall'altro punisce chi usa software libero e
trasparente sul proprio dispositivo, trattandolo come un utente di serie
B.

Come se non bastasse, questa scelta contraddice proprio la legge che
dovrebbe regolare l'informatica pubblica in Italia, cioè il Codice
dell'Amministrazione Digitale (D.Lgs. 82/2005)
[<u>\[25\]</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2005-03-07;82).
L'articolo 3 del Codice garantisce infatti a tutti i cittadini il
diritto di usare le tecnologie per dialogare con la Pubblica
Amministrazione, un diritto che perde senso se per esercitarlo devi
sottostare a blocchi tecnici imposti da terzi. Ancora più esplicito è
l'articolo 68, che impone alle pubbliche amministrazioni il principio
della neutralità tecnologica: lo Stato deve scegliere soluzioni basate
su standard aperti, garantendo l'interoperabilità ed evitando di
affidarsi completamente a un ente terzo
[<u>\[26\]</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2005-03-07;82).

Oggi ci troviamo davanti a un paradosso difficile da accettare in uno
Stato di diritto: per poter esercitare i nostri diritti di cittadini
digitali siamo costretti a rinunciare alla libertà sul nostro hardware e
ad accettare in silenzio le condizioni commerciali di due colossi
privati.

## 3.3 Tagliati fuori dalla vita quotidiana: banche, studio e lavoro

Questa dipendenza forzata non riguarda solo il rapporto con lo Stato, ma
tocca ormai ogni aspetto della vita quotidiana, a partire dalla gestione
dei nostri soldi.

Negli ultimi anni la direttiva europea sui pagamenti digitali (la PSD2)
ha imposto alle banche di usare sistemi di autenticazione forte del
cliente (*Strong Customer Authentication* o SCA) per proteggere conti e
bonifici
[<u>\[27\]</u>](https://eur-lex.europa.eu/legal-content/IT/TXT/?uri=CELEX:32015L2366).
La legge europea non ha mai vietato le classiche chiavette fisiche (i
token hardware che generano il codice numerico), ma quasi tutte le
banche le hanno eliminate o rese a pagamento per risparmiare sui costi
di produzione e spedizione, scaricando tutto sull'app per smartphone.

Chiunque abbia un conto corrente oggi conosce bene la procedura: anche
se vuoi fare un bonifico comodamente dal browser del tuo PC fisso, il
sito della banca non ti fa andare avanti se non apri l'app sul telefono
per approvare una notifica push o per inquadrare un codice QR sullo
schermo. Il problema è che quell'app bancaria usa quasi sempre i
controlli di Play Integrity o sistemi anti-root proprietari. Se sul tuo
smartphone hai installato un sistema operativo alternativo, l'app della
banca crasha; quindi anche l'accesso dal computer ti viene negato. La
scusa secondo cui «tanto puoi sempre usare il sito web dal PC» nella
pratica non regge più, e il risultato è che una modifica software sul
tuo telefono può letteralmente impedirti di usare i tuoi soldi, andando
a sbattere contro lo stesso diritto europeo che garantisce a ogni
cittadino l'accesso non discriminatorio a un conto di pagamento di base
[<u>\[28\]</u>](https://www.astrid-online.it/static/upload/Dire/Directive_Payment-Accounts_23_07_14.pdf).

Da lì in poi l'effetto domino travolge tutto il resto della giornata. Se
il tuo telefono non supera l'esame di Google, diventa un percorso a
ostacoli scaricare un referto medico o una ricetta dal Fascicolo
Sanitario Elettronico. Per chi studia, significa rischiare di non poter
accedere ai portali universitari per verbalizzare un esame o controllare
la domanda per la borsa di studio, visto che richiedono tutti l'accesso
con SPID o CIE. Lo stesso vale sul lavoro e negli spostamenti di tutti i
giorni, tra app aziendali obbligatorie per timbrare il cartellino da
remoto, sistemi di fatturazione e biglietti o abbonamenti digitali
dell'autobus che smettono di funzionare sui dispositivi sbloccati.

Quella che fino a dieci anni fa era una semplice scelta da appassionati
di informatica (decidere quale sistema operativo far girare sul proprio
dispositivo) oggi viene punita con una forma di esclusione sociale. Per
vivere, studiare e lavorare nella società di oggi ti obbligano ad avere
uno smartphone, ma per poterlo usare davvero ti obbligano a lasciarne il
controllo nelle mani dei produttori.

# Capitolo 4: Il Mercato Bloccato e l'Impatto Reale (Concorrenza, Obsolescenza ed E-waste)

Tutti i blocchi tecnici e contrattuali che abbiamo visto finora non
servono solo a togliere libertà all'utente finale: hanno un impatto
enorme sull'economia, sulla concorrenza e sull'ambiente. Controllando
con il contagocce come vengono distribuite le app, decidendo a tavolino
quando far invecchiare i telefoni e ostacolando le riparazioni
indipendenti, i grandi produttori si sono costruiti un mercato blindato
a spese dei consumatori e del pianeta.

## 4.1 La stretta sul sideloading e l'iniziativa \#KeepAndroidOpen

Per anni, nelle discussioni tra appassionati di tecnologia, Android è
sempre stato difeso come l'alternativa libera e aperta rispetto alla
"gabbia dorata" di Apple. La differenza fondamentale stava in una
funzione semplicissima chiamata *sideloading*: la libertà di scaricare
un file di installazione (.apk) dal sito di uno sviluppatore o da uno
store alternativo (come F-Droid o GitHub) e installarlo direttamente sul
telefono, senza dover passare per forza dal Google Play Store.

Negli ultimi anni, però, Google ha iniziato a smantellare questa libertà
passo dopo passo, usando la scusa della sicurezza per alzare muri
tecnici e psicologici sempre più alti
[<u>\[29\]</u>](https://www.eff.org/deeplinks/2025/11/application-gatekeeping-ever-expanding-pathway-internet-censorship).

Il primo ostacolo è psicologico e passa per Google Play Protect: quando
provi a installare un'app da fuori, il sistema ti sbatte in faccia
schermate di blocco a tutto schermo, avvisi rossi allarmistici e
pulsanti per continuare nascosti nei sottomenu, trattando qualsiasi
programma open source non registrato da Google alla stregua di un virus
pericoloso [<u>\[30\]</u>](https://keepandroidopen.org/it/). Se non ti
fai spaventare e installi comunque l'app, scatta il secondo blocco: a
partire da Android 13, il sistema operativo ha introdotto le cosiddette
"impostazioni con restrizioni" (*Restricted Settings*), che disattivano
d'ufficio i permessi più importanti (come i servizi di accessibilità o
la lettura delle notifiche) a tutte le app installate fuori dallo store
ufficiale. In questo modo programmi del tutto legittimi (come i gestori
di password indipendenti, gli strumenti di automazione o le app per chi
ha disabilità non presenti nello store) smettono di funzionare, a meno
che l'utente non sappia come andare a sbloccare manualmente dei menu
nascosti nelle impostazioni di sistema.

Come se non bastasse, Google ha inserito dentro le Play Integrity API un
controllo che verifica da quale store proviene il file installato: così
gli sviluppatori possono configurare le proprie app per rifiutarsi di
partire se si accorgono di non essere state scaricate dal Play Store,
anche quando il file .apk è originale al cento per cento e non è stato
toccato da nessuno. A chiudere il cerchio sono arrivati gli obblighi di
registrazione e verifica dell'identità per chi sviluppa app Android
(avviati tra il 2025 e il 2026 anche per chi distribuisce fuori dal Play
Store, in vista del blocco globale): chi vuole pubblicare software deve
pagare una quota e inviare i propri documenti personali a Google, mentre
per gli studenti e gli hobbisti che non si registrano vengono imposti
limiti assurdi (come un tetto massimo di poche decine di installazioni o
procedure di sblocco che costringono l'utente a riavviare il telefono e
ad aspettare 24 ore prima di poter installare il file .apk).

Contro questa chiusura è nata la campagna internazionale
**\#KeepAndroidOpen**, lanciata proprio dalla comunità di F-Droid e da
diverse organizzazioni per i diritti digitali per denunciare come il
pretesto della sicurezza venga usato per eliminare ogni canale
alternativo al Play Store
[<u>\[30\]</u>](https://keepandroidopen.org/it/). Tra l'altro, in Europa
questo comportamento va a scontrarsi con il Digital Markets Act (il
Regolamento UE 2022/1925)
[<u>\[31\]</u>](https://eur-lex.europa.eu/eli/reg/2022/1925/oj?locale=it).
Nel settembre 2023 la Commissione Europea ha infatti inserito
ufficialmente Alphabet (Google) nella lista dei *gatekeeper* per Android
e Google Play (Decisione C(2023) 6105): l'articolo 6, paragrafo 4 del
regolamento obbliga queste grandi piattaforme a permettere
l'installazione e l'uso normale di app di terze parti e di store
concorrenti, ammettendo solo misure di sicurezza strettamente
proporzionate. Trasformare l'installazione di un'app esterna in una
corsa a ostacoli serve solo a soffocare sul nascere la concorrenza. Che
un modello aperto sia possibile lo dimostrano realtà come Fairphone e
Murena, oltre al fatto che persino un sistema storicamente blindato come
quello di Apple è stato costretto ad aprirsi al sideloading in Europa
proprio grazie al DMA.

## 4.2 L'obsolescenza software programmata e la produzione forzata di rifiuti elettronici

Se guardiamo a come invecchiano i nostri dispositivi, gli smartphone
rappresentano un caso unico e assurdo nel mondo dell'informatica. Un
computer fisso o un portatile lo cambiamo quando si rompe un pezzo
importante o quando il processore non ce la fa più a far girare i
programmi nuovi; uno smartphone, invece, muore quasi sempre a tavolino
il giorno in cui il produttore decide di smettere di aggiornarlo.

Dal punto di vista fisico, l'hardware dei telefoni moderni potrebbe
durare tranquillamente più di dieci anni: gli schermi OLED, le memorie
flash e i moderni processori a 4 o 5 nanometri hanno una potenza che
supera di gran lunga quello che serve per navigare sul web, mandare
messaggi o usare le app di tutti i giorni. Eppure, in Europa la vita
media di uno smartphone si ferma intorno ai 3 o 4 anni, tagliata corta
proprio dalla fine degli aggiornamenti software
[<u>\[32\]</u>](https://www.eea.europa.eu/en/analysis/publications/europes-consumption-in-a-circular-economy-the-benefits-of-longer-lasting-electronics).

Per chiunque ne capisca di informatica, il motivo di questo blocco è
chiarissimo. Sui PC esiste uno standard hardware comune e i driver
finiscono direttamente nel kernel Linux ufficiale (*mainline*): per
questo puoi prendere un portatile di dieci anni fa, formattarlo e
installarci l'ultima versione di una distribuzione Linux in venti
minuti. Sugli smartphone non funziona così: chi produce i chip (come
Qualcomm o MediaTek) e chi assembla i telefoni non usa il kernel Linux
standard, ma delle versioni modificate e chiuse chiamate *downstream
kernel*, accompagnate da pacchetti di driver proprietari per la scheda
madre (i *Board Support Packages* o BSP). Quando il produttore smette di
aggiornare quel pacchetto per il tuo modello di processore, il telefono
resta inchiodato per sempre a una vecchia versione del kernel e non può
più ricevere le nuove versioni di Android.

Da quel momento inizia un lento (ma non troppo) declino: nel giro di
poco tempo le app delle banche, i servizi di pagamento e i portali
pubblici alzano la versione minima richiesta di Android o irrigidiscono
i controlli delle Play Integrity API. Anche se il telefono funziona
ancora benissimo, le app smettono di aprirsi una dopo l'altra. E se
l'utente o la comunità open source volessero salvarlo installando un
sistema operativo aggiornato, si trovano la strada sbarrata dal
bootloader bloccato, dalle firme crittografiche e dalla mancanza dei
driver sorgenti
[<u>\[33\]</u>](https://fsfe.org/activities/upcyclingandroid/).

Tutto questo ha un costo ambientale enorme. Gli studi sul ciclo di vita
degli smartphone realizzati dal centro di ricerca Fraunhofer IZM e dal
Joint Research Centre (JRC) della Commissione Europea spiegano che fino
all'80% delle emissioni totali di gas serra di un telefono non viene
prodotto mentre lo usiamo e lo ricarichiamo, ma nella fase iniziale in
cui si estraggono le terre rare dalle miniere e si stampano i microchip
in fabbrica
[<u>\[34\]</u>](https://publications.jrc.ec.europa.eu/repository/handle/JRC124077).
Obbligare milioni di persone a buttare via telefoni perfettamente
funzionanti solo perché il software è scaduto significa sprecare litio,
silicio e metalli preziosi, alimentando una montagna di rifiuti
elettronici (RAEE).

Proprio per arginare questo spreco l'Unione Europea ha iniziato a
muoversi, sia con il Regolamento Ecodesign per smartphone e tablet (UE
2023/1670), che impone ai produttori di garantire almeno cinque anni di
aggiornamenti dopo l'uscita dal mercato del modello
[<u>\[35\]</u>](https://eur-lex.europa.eu/eli/reg/2023/1670/oj), sia con
la Direttiva sulla transizione verde (UE 2024/825), che punisce come
pratiche commerciali scorrette i trucchi usati per nascondere i limiti
alla durata dei prodotti
[<u>\[36\]</u>](https://eur-lex.europa.eu/eli/dir/2024/825/oj?locale=it).
Finché però il software resterà saldato con la crittografia al
processore, impedendo agli utenti di installare sistemi operativi liberi
quando finisce il supporto ufficiale, i produttori avranno sempre in
mano l'interruttore per decidere quando mandare in pensione il nostro
hardware.

## 4.3 L'accoppiamento crittografico dei componenti (Parts Pairing) e il blocco della riparazione

Come se non bastasse il controllo sul software, negli ultimi anni i
produttori hanno trovato il modo di usare la crittografia anche per
impedirci di riparare i pezzi fisici del telefono, attraverso una
tecnica chiamata *parts pairing* (o serializzazione hardware)
[<u>\[37\]</u>](https://susproc.jrc.ec.europa.eu/product-bureau/sites/default/files/2021-12/JRC_Report_Repair_Score_Smartphone_Tablets_v2.pdf).

Negli smartphone di oggi quasi ogni singolo componente interno (lo
schermo, la batteria, il modulo delle fotocamere e persino la porta di
ricarica) contiene un minuscolo chip o una memoria su cui è registrato
un numero di serie unico. Quando il telefono esce dalla catena di
montaggio, la scheda madre salva tutti questi codici dentro la sua
memoria sicura.

Ad ogni accensione, il processore controlla che i numeri di serie dei
pezzi montati siano ancora gli stessi registrati in fabbrica. Se ti cade
il telefono, si rompe il vetro e decidi di cambiarlo da solo (o di
portarlo da un tecnico sotto casa), il controllo crittografico fallisce
anche se usi un pezzo di ricambio originale al cento per cento, magari
smontato da un altro smartphone identico al tuo.

Appena il sistema si accorge che il numero di serie non è quello
"autorizzato", inizia a sabotare il telefono. Prima di tutto disattiva
via software una serie di funzioni: cambiando lo schermo o la fotocamera
perdi la calibrazione automatica dei colori, la frequenza di
aggiornamento alta del display, la messa a fuoco avanzata o lo sblocco
con l'impronta digitale. In secondo luogo, il sistema operativo inizia a
mostrare notifiche e avvisi fissi nelle impostazioni che dicono che il
componente "non è verificabile" o "potrebbe non essere originale",
facendo credere all'utente che il tecnico gli abbia montato un pezzo
difettoso. Per togliere questi blocchi non basta montare bene il pezzo:
serve lanciare una procedura di calibrazione software che funziona solo
collegandosi ai server centrali del produttore, a cui ovviamente hanno
accesso solo i centri di assistenza ufficiali del marchio.

Con questo sistema i produttori riescono a uccidere il mercato delle
riparazioni indipendenti e del recupero dei pezzi usati (la cosiddetta
cannibalizzazione dei ricambi da telefoni rotti). Se per cambiare uno
schermo o una batteria sei obbligato ad andare per forza dall'assistenza
ufficiale a prezzi altissimi, spesso la riparazione costa quasi quanto
il valore del telefono usato; e così l'utente finisce per buttare il
vecchio e comprare il modello nuovo.

Anche su questo fronte lo scontro con le nuove regole europee è
evidente: sia la Direttiva sul Diritto alla Riparazione (UE 2024/1799,
appena recepita in Italia a ottobre 2026 con il D.Lgs. 176/2026 che ha
modificato il Codice del Consumo)
[<u>\[38\]</u>](https://eur-lex.europa.eu/eli/dir/2024/1799/oj?locale=it),
sia il Regolamento Ecodesign (UE 2023/1670)
[<u>\[39\]</u>](https://eur-lex.europa.eu/eli/reg/2023/1670/oj) vietano
ai produttori di usare trucchi hardware o software ingiustificati per
ostacolare le riparazioni indipendenti e l'uso di ricambi usati o
compatibili. La partita però è tutt'altro che chiusa: le nuove norme
lasciano infatti dei margini per "giustificazioni legittime e
oggettive", e il rischio concreto è che le aziende continuino a
difendere i blocchi crittografici sui ricambi nascondendosi ancora una
volta dietro il pretesto della sicurezza.

# Capitolo 5: Soluzioni Tecnico-Normative e Proposte di Policy

Tutto il sistema di blocchi che abbiamo analizzato fin qui non è una
conseguenza inevitabile del progresso tecnologico e non è nemmeno una
misura indispensabile per garantire la sicurezza informatica. È una
scelta industriale pensata per difendere modelli di business basati sul
controllo delle piattaforme, sulla raccolta dei dati e sull'obsolescenza
programmata.

Restituire agli utenti il controllo sui propri dispositivi e proteggere
i diritti dei cittadini non significa tornare indietro sulla sicurezza,
ma portare finalmente anche sugli smartphone quei principi di apertura,
modularità e neutralità che hanno reso grande l'informatica fin dalla
nascita dei personal computer.

## 5.1 Le soluzioni tecniche e normative praticabili

Per aprire l'hardware degli smartphone senza abbassare le difese contro
i malware non serve inventare nulla da zero: basta applicare ai telefoni
le soluzioni tecniche che usiamo già da anni sui computer e far
rispettare sul serio le norme europee.

#### 1. Portare il modello dei PC sugli smartphone: sblocco e chiavi personali (User Key Enrollment)

L'idea che uno smartphone debba essere per forza blindato dal produttore
per essere sicuro è un falso mito tecnico. Sui personal computer, lo
standard UEFI con Secure Boot permette a chiunque sia proprietario della
macchina di sostituire o affiancare le chiavi crittografiche di fabbrica
con le proprie chiavi personali (*User Key Enrollment*): in questo modo
la catena di avvio resta protetta e verificata al cento per cento anche
quando si installa una distribuzione Linux indipendente.

Questa stessa architettura dovrebbe diventare obbligatoria per legge su
tutti gli smartphone venduti sul mercato. Prima di tutto, ogni utente
deve avere il diritto di sbloccare il bootloader del proprio telefono in
modo universale e senza condizioni, cioè con un semplice comando locale,
senza dover chiedere il permesso ai server del produttore, senza code di
attesa e senza dover cedere i propri dati personali. Una volta
sbloccato, il telefono deve permettere di registrare la propria chiave
crittografica personale dentro il chip di sicurezza (usando la funzione
standard di Android chiamata avb_custom_key), così da poter richiudere
il bootloader e mantenere l'avvio verificato (*Verified Boot*) anche con
un sistema operativo alternativo
[<u>\[40\]</u>](https://source.android.com/docs/security/features/verifiedboot/avb?hl=it).

Ovviamente questo meccanismo va protetto dagli attacchi fisici (quelli
che in sicurezza informatica si chiamano attacchi *Evil Maid*, cioè
quando un malintenzionato prende in mano il tuo telefono per pochi
minuti): per questo lo sblocco del bootloader e il cambio delle chiavi
non devono mai poter partire via software da remoto o di nascosto, ma
devono richiedere una combinazione fisica di tasti e una conferma sullo
schermo, cancellando automaticamente le chiavi di crittografia della
memoria utente (*Cryptographic Wipe*) ad ogni cambio di firma, così che
nessuno possa mai leggere i dati personali già presenti sul telefono.
Infine, deve essere vietato qualsiasi danneggiamento fisico punitivo:
sbloccare il proprio dispositivo non deve bruciare fusibili elettronici
irreversibili (eFuse) né disattivare le fotocamere o altre funzioni
hardware, e deve essere sempre possibile tornare indietro rimettendo le
chiavi di fabbrica.

#### 2. Neutralità tecnologica della Pubblica Amministrazione e standard aperti

I diritti civili e l'accesso ai servizi pubblici non possono dipendere
dalle API proprietarie di due multinazionali straniere. L'Agenzia per
l'Italia Digitale (AgID) e l'Istituto Poligrafico e Zecca dello Stato
dovrebbero intervenire subito sullo sviluppo delle app pubbliche (come
App IO, CieID e il sistema SPID) per eliminare qualsiasi dipendenza
dalle Google Play Integrity API e dai sistemi equivalenti di Apple.

Al posto di questi controlli, lo Stato deve adottare esclusivamente
standard di sicurezza aperti e riconosciuti a livello internazionale
come WebAuthn e FIDO2
[<u>\[41\]</u>](https://www.w3.org/TR/webauthn-3/). Dal punto di vista
crittografico, la sicurezza di un accesso pubblico deve basarsi sulla
chiave del cittadino (come il chip NFC dentro la Carta d'Identità
Elettronica o una chiavetta di sicurezza FIDO), e non sul fatto che il
sistema operativo del telefono piaccia o meno alla multinazionale di
turno. Allo stesso tempo, va garantita per legge la piena parità di
accesso tramite browser web, permettendo ai cittadini di svolgere
qualsiasi pratica dal proprio computer senza essere costretti a
installare un'applicazione mobile proprietaria.

#### 3. Stop ai blocchi crittografici sui ricambi e calibrazione libera

Sfruttando il quadro della Direttiva europea sul Diritto alla
Riparazione (UE 2024/1799) e del Regolamento Ecodesign (UE 2023/1670),
bisogna fermare l'abuso del *parts pairing*. Da una parte va vietato ai
produttori di usare blocchi crittografici legati al numero di serie per
impedire di sostituire uno schermo, una batteria o una fotocamera con
pezzi funzionanti presi da un altro dispositivo identico. Dall'altra, se
un componente sostituito ha davvero bisogno di una ricalibrazione
software per funzionare bene, i produttori devono essere obbligati a
rendere pubblici e gratuiti gli strumenti di calibrazione, permettendo a
qualsiasi riparatore o utente di eseguire la procedura senza dover
passare dai server cloud dell'azienda.

## 5.2 Risposta alle obiezioni dell'industria

Ogni volta che si chiede di aprire l'hardware ai proprietari, i
produttori e i gestori delle grandi piattaforme si difendono tirando
fuori sempre le stesse scuse legate alla sicurezza e al mercato. Sia
chiaro: nessuno nega che i chip di sicurezza e l'attestazione hardware
possano essere utili contro le truffe o contro certi malware che cercano
di sovrapporre schermate false (*overlay attack*); il problema non è lo
strumento crittografico in sé, ma il fatto che venga gestito come un
monopolio chiuso per tagliare fuori chi usa software libero.

#### Obiezione 1: «Sbloccare il telefono e avere i permessi di root espone agli attacchi e mette a rischio le banche»

Questa è la scusa più diffusa, ma dal punto di vista informatico
confonde la sicurezza del sistema con il controllo commerciale della
piattaforma. Nei sistemi operativi moderni, la protezione delle app non
dipende dal blocco del bootloader, ma dal fatto che ogni applicazione
gira isolata nella propria gabbia (*sandboxing*), che i file sulla
memoria sono protetti dalla crittografia (FBE, *File-Based Encryption*)
e che i permessi sono blindati da regole rigide del kernel (come
SELinux): tutte difese che funzionano benissimo a prescindere da chi
abbia firmato il sistema operativo all'avvio.

Spesso le banche rispondono che su un telefono con i permessi di root un
programma malevolo potrebbe usare strumenti di manipolazione della
memoria in tempo reale (come Frida o moduli Xposed/LSPosed) per alterare
l'app bancaria mentre è aperta. Ma questo ragionamento parte da un
errore di fondo: la sicurezza di un'operazione bancaria non può reggersi
sulla speranza che il sistema operativo dell'utente sia impenetrabile,
ma deve basarsi su protocolli crittografici asimmetrici e sulla conferma
sicura di ciò che si sta firmando (*What You See Is What You Sign*),
affidata a interfacce protette direttamente dal chip di sicurezza
(*Trusted UI*), alla lettura NFC della carta o a un fattore esterno
indipendente.

La prova più evidente che questa obiezione non sta in piedi ce l'abbiamo
sotto gli occhi tutti i giorni: i computer tradizionali. Da decenni le
banche ci fanno accedere al conto corrente e fare bonifici da PC con
Windows, macOS o Linux su cui siamo amministratori, dove potremmo aprire
un debugger o leggere la memoria RAM di qualsiasi processo in
esecuzione, eppure il sistema bancario non è mai crollato. Tra l'altro,
togliere i permessi di root al proprietario del telefono non ferma
affatto i malware più pericolosi, che per prendere il controllo del
sistema sfruttano falle segrete del kernel (*zero-day*) senza certo
chiedere il permesso all'utente. Al contrario, sistemi operativi liberi
e progettati per la sicurezza come GrapheneOS dimostrano che togliere il
bloatware e la telemetria di fabbrica rende il telefono molto più sicuro
rispetto al software originale dei produttori.

#### Obiezione 2: «L'attestazione remota serve per proteggere il diritto d'autore e lo streaming (DRM)»

Usare la tutela del copyright dei film in streaming per giustificare il
blocco hardware di un intero computer tascabile ribalta completamente la
gerarchia dei diritti. Il diritto di proprietà di chi ha comprato il
bene fisico (tutelato dall'articolo 832 del Codice Civile) riguarda la
libertà di usare al massimo le capacità del proprio hardware e non può
essere sacrificato per fare un favore ai distributori di contenuti
multimediali (come i sistemi DRM Widevine o FairPlay).

Inoltre c'è una differenza enorme tra un servizio commerciale privato e
un diritto del cittadino: se una piattaforma di streaming decide nel suo
contratto di abbassare la risoluzione video su un telefono sbloccato, fa
una scelta commerciale discutibile ma limitata al suo servizio. Usare
quello stesso identico meccanismo di blocco per impedire a un cittadino
di usare la Carta d'Identità Elettronica, lo SPID o il proprio conto in
banca significa trasformare un filtro pensato per il copyright in uno
strumento di esclusione civile ed economica.

#### Obiezione 3: «Quelli che cambiano sistema operativo sullo smartphone sono pochissimi, non vale la pena fare una legge»

Dire che c'è poca domanda di sistemi operativi alternativi quando si fa
di tutto per renderli inutilizzabili è un ragionamento fallace. Se oggi
solo una nicchia di appassionati ed esperti installa ROM alternative, è
proprio perché l'industria ha costruito un muro altissimo: sapere che
sbloccando il telefono rischi di perdere l'app della banca, l'identità
digitale, i pagamenti contactless e magari pure la garanzia scoraggia
sul nascere il 99% degli utenti normali e impedisce a qualsiasi
concorrente di crescere.

Nel diritto europeo della concorrenza (dall'articolo 102 del TFUE fino
al Digital Markets Act) le regole antitrust non si applicano contando
quanti utenti riescono oggi a sopravvivere fuori dal monopolio, ma
servono a garantire che il mercato sia aperto e contendibile da nuovi
arrivati
[<u>\[42\]</u>](https://eur-lex.europa.eu/legal-content/IT/TXT/?uri=CELEX:12012E/TXT).
E quando parliamo di servizi pubblici, i numeri di mercato non contano
nulla: il principio di uguaglianza della Costituzione (art. 3) e la
neutralità tecnologica dello Stato (art. 68 del CAD) valgono per tutti i
cittadini, anche se a scegliere un sistema operativo libero fosse una
minoranza.

## 5.3 Proposte concrete per le Autorità di regolazione

Alla luce di tutto quello che abbiamo visto sul piano tecnico, legale ed
economico, ci sono quattro fronti su cui i garanti nazionali e le
istituzioni europee dovrebbero intervenire direttamente.

#### 1. Cosa dovrebbe fare l'Antitrust (AGCM)

L'Autorità Garante della Concorrenza e del Mercato dovrebbe aprire
un'indagine sul mercato degli smartphone per sanzionare la vendita
abbinata forzata di hardware e software in base al Codice del Consumo
(D.Lgs. 206/2005), obbligando i produttori a separare i due contratti e
a rimborsare la licenza del sistema operativo preinstallato a chi non
vuole usarla
[<u>\[43\]</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2005-09-06;206).
Allo stesso tempo, l'AGCM dovrebbe vietare le clausole che fanno
decadere automaticamente la garanzia legale di due anni sull'hardware
solo perché l'utente ha sbloccato il bootloader o cambiato sistema
operativo: come prevede la legge, deve essere il produttore a dimostrare
che un guasto fisico è stato causato davvero dalla modifica software.
Infine, sul fronte delle riparazioni, l'Antitrust dovrebbe colpire l'uso
del *parts pairing* sia come abuso di posizione dominante (Legge
287/1990, art. 3) pensato per tagliare fuori i tecnici indipendenti
[<u>\[44\]</u>](https://www.bosettiegatti.eu/info/norme/statali/1990_0287.htm),
sia come abuso di dipendenza economica (Legge 192/1998, art. 9) ai danni
dei piccoli centri di riparazione
[<u>\[45\]</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:1998-06-18;192!vig=).

#### 2. Cosa dovrebbero fare AgID e il Dipartimento per la Trasformazione Digitale

Chi governa l'informatica pubblica in Italia deve fissare linee guida
vincolanti per imporre l'eliminazione delle Google Play Integrity API (e
dei blocchi analoghi di Apple) da tutte le applicazioni della Pubblica
Amministrazione e dei gestori di identità digitale (App IO, CieID,
SPID). La sicurezza dei servizi pubblici va spostata interamente su
protocolli aperti come WebAuthn e FIDO2, legando la verifica ai
certificati crittografici del cittadino invece che al sistema operativo
dello smartphone, e garantendo sempre la possibilità di fare tutto da un
normale browser web su computer. Lo stesso principio va difeso sui
tavoli europei per l'IT Wallet e il futuro EUDI Wallet, impedendo che le
regole tecniche dell'Unione finiscano per regalare un monopolio di fatto
alle attestazioni proprietarie americane.

#### 3. Cosa dovrebbe fare il Garante per la Privacy

Il Garante per la Protezione dei Dati Personali dovrebbe verificare
quanto siano compatibili questi blocchi con il GDPR. Da una parte,
costringere i cittadini (o i clienti di una banca) a non poter usare il
browser web sul PC per obbligare a scaricare un'app mobile piena di
tracker e librerie telemetriche proprietarie viola i principi di
minimizzazione dei dati e di libertà del consenso (articoli 5 e 6 del
GDPR). Dall'altra, alla luce del principio di *Privacy by Design e by
Default* (articolo 25 del GDPR), bisogna limitare la lettura continua e
non disattivabile di codici identificativi hardware permanenti (come lo
stato degli eFuse, i registri del TEE o i numeri di serie dei
componenti) quando non c'è una base giuridica proporzionata.

#### 4. Cosa dovrebbe fare la Commissione Europea

A livello europeo, la Commissione ha già gli strumenti normativi per
intervenire e deve applicarli fino in fondo. Con il Digital Markets Act
(Regolamento UE 2022/1925), deve imporre ai *gatekeeper* il rispetto
reale dell'articolo 6, paragrafo 4, fermando le schermate allarmistiche
di Play Protect, il blocco automatico dei permessi (*Restricted
Settings*) e i controlli sull'origine dell'installazione usati per
sabotare il *sideloading*, spingendo inoltre per l'apertura standard dei
bootloader tramite lo *User Key Enrollment*. Infine, nell'attuazione
della Direttiva sul Diritto alla Riparazione (UE 2024/1799) e del
Regolamento Ecodesign (UE 2023/1670), la Commissione dovrebbe mettere
nero su bianco che il blocco crittografico dei pezzi di ricambio (*parts
pairing*) è un ostacolo illegittimo alla riparazione, imponendo
l'apertura gratuita dei software di calibrazione.

## Nota metodologica e sviluppi futuri

Questo documento mantiene aperti alcuni filoni di verifica tecnica e
giuridica che verranno approfonditi nei prossimi aggiornamenti del
progetto:

Sul piano legale, resta da esplorare fino a che punto il principio
fissato dalla Cassazione (sentenza n. 19161/2014 sul rimborso del
sistema operativo sui PC) possa essere applicato dai tribunali anche
agli smartphone e ai dispositivi mobili attuali. Sul piano delle
applicazioni pubbliche, mentre l'uso di Play Integrity e Key Attestation
è già confermato e documentato per alcune funzioni di App IO, prosegue
l'analisi tecnica del codice e del traffico di rete sulle altre app
dell'ecosistema pubblico (come CieID e le varie app SPID). Sul fronte
europeo, sarà fondamentale monitorare l'applicazione pratica delle norme
su Diritto alla Riparazione ed Ecodesign nei singoli Stati membri per
vedere come verranno sanzionati i blocchi del *parts pairing*.

Infine, è bene ribadire il senso di questa critica: questo lavoro non
mette in discussione l'utilità della crittografia hardware (come il
Trusted Execution Environment) né il bisogno di difendersi dalle frodi
informatiche, ma contesta il fatto che questi strumenti vengano chiusi a
chiave dai produttori, impedendo al legittimo proprietario dello
smartphone di inserire le proprie chiavi crittografiche e di avere
l'ultima parola sul proprio “computer tascabile”.

# Archivio Fonti e Riferimenti

### Capitolo 1

**\[1\] Codice Civile Italiano:** [<u>Articolo 832 (Contenuto del
diritto di
proprietà)</u>](https://www.brocardi.it/codice-civile/libro-terzo/titolo-ii/capo-i/art832.html).

**\[2\] Parlamento Europeo e Consiglio:** [<u>Direttiva 2009/24/CE sulla
tutela giuridica dei programmi per
elaboratore</u>](https://eur-lex.europa.eu/legal-content/IT/TXT/?uri=CELEX:32009L0024).

**\[3\] Parlamento Europeo e Consiglio:** [<u>Direttiva (UE) 2019/771
sui contratti di vendita di beni (art. 2, punto 5: beni con elementi
digitali)</u>](https://eur-lex.europa.eu/eli/dir/2019/771/oj?locale=it)
*(recepita in Italia dal D.Lgs. 170/2021 che ha modificato l'art. 128
del Codice del Consumo)*.

**\[4\] Codice del Consumo (D.Lgs. 206/2005):** [<u>Articolo 33
(Clausole vessatorie nel contratto tra professionista e
consumatore)</u>](https://www.brocardi.it/codice-del-consumo/parte-iii/titolo-i/art33.html).

**\[5\] Corte Suprema di Cassazione, sentenza dell'11 settembre 2014, n.
19161:** Testo integrale e sintesi sul rimborso del sistema operativo
preinstallato (archivio ADUC: [<u>documento
PDF</u>](https://www.aduc.it/generale/files/file/allegati/cassazione-rimborso-windows.pdf)
e
[<u>comunicato</u>](https://www.aduc.it/comunicato/sistema+operativo+windows+indesiderato+cassazione_22477.php)).

**\[6\] Android Open Source Project (AOSP):** [<u>Android Verified Boot
(AVB)
Architecture</u>](https://source.android.com/docs/security/features/verifiedboot/avb?hl=it).
Documentazione ufficiale sul controllo crittografico della catena di
avvio e sulla verifica delle partizioni.

**\[7\] Samsung Knox Documentation:** [<u>Hardware-Backed Security &
Knox Warranty
Bit</u>](https://docs.samsungknox.com/admin/fundamentals/whitepaper/samsung-knox-mobile-security/system-security/hw-backed-security/).
Specifiche tecniche sul fusibile elettronico monouso (*e-fuse / OTP*)
che scatta in modo irreversibile da 0 a 1 quando rileva l'avvio di un
software o di un kernel non autorizzato.

### Capitolo 2

**\[8\] ARM Limited:** [<u>Bare-metal Boot Code for ARMv8-A
Processors</u>](https://support.arm.com/documentation/dai0527/a/).
Documentazione ufficiale dell'architettura ARM sulla sequenza di avvio a
partire dalla Boot ROM primaria (*Reset Vector* e *Trusted Boot*).

**\[9\] Android Open Source Project (AOSP):** [<u>Verified Boot Flow and
Partitions
Verification</u>](https://source.android.com/docs/security/features/verifiedboot/boot-flow?hl=it).
Specifica tecnica sulla verifica crittografica a catena delle partizioni
durante l'avvio.

**\[10\] Android Open Source Project (AOSP):** [<u>Managing the Root of
Trust (Custom AVB
Keys)</u>](https://source.android.com/docs/security/features/verifiedboot/device-state?hl=it).
Documentazione ufficiale che descrive il comando standard fastboot flash
avb_custom_key per caricare chiavi crittografiche personali sui
dispositivi che supportano una Root of Trust alternativa.

**\[11\] ARM Limited:** [<u>TrustZone Technology for
Armv8-A</u>](https://developer.arm.com/-/media/Arm%20Developer%20Community/PDF/Learn%20the%20Architecture/TrustZone%20for%20Armv8-A.pdf).
Documentazione ufficiale sull'isolamento hardware della memoria tra
Normal World (Non-secure) e Secure World.

**\[12\] GlobalPlatform:** [<u>TEE System Architecture
Specification</u>](https://globalplatform.org/wp-content/uploads/2022/05/GPD_SPE_009-GPD_TEE_SystemArchitecture_v1.3_PublicRelease_signed.pdf).
Standard industriale sui requisiti di isolamento e funzionamento degli
ambienti Trusted Execution Environment (TEE).

**\[13\] Samsung Electronics:** [<u>Samsung Knox Mobile Security
Whitepaper: Hardware-Backed
Security</u>](https://docs.samsungknox.com/admin/fundamentals/whitepaper/samsung-knox-mobile-security/system-security/hw-backed-security/).
Specifica tecnica sui fusibili elettronici (One-Time Programmable /
eFuse) e sulla disattivazione permanente delle funzioni legate a Knox.

**\[14\] Android Open Source Project (AOSP):** [<u>Hardware-backed
Keystore and StrongBox
Keymaster</u>](https://source.android.com/docs/security/features/keystore?hl=it).
Documentazione ufficiale sui moduli di sicurezza hardware e
sull'isolamento crittografico delle chiavi.

**\[15\] Google Developers:** [<u>Play Integrity API
Overview</u>](https://developer.android.com/google/play/integrity/overview?hl=it).
Documentazione tecnica sul funzionamento dei controlli di integrità
firmati dall'hardware e sui livelli MEETS_DEVICE_INTEGRITY e
MEETS_STRONG_INTEGRITY.

**\[16\] Android Open Source Project (AOSP):** [<u>Modular DRM and
Widevine Security
Levels</u>](https://source.android.com/docs/core/media/drm?hl=it).
Specifica tecnica sui livelli di sicurezza DRM e sulla differenza tra
decrittazione gestita nel TEE (Livello L1) e declassamento via software
(Livello L3).

**\[17\] Google / Open Handset Alliance:** [<u>Android Compatibility
Definition Document (CDD) & Compatibility Test Suite
(CTS)</u>](https://source.android.com/docs/compatibility/cdd?hl=it).
Requisiti con cui Google stabilisce quali dispositivi e sistemi
operativi possono ottenere la certificazione per i Google Mobile
Services (GMS) e superare le verifiche di attestazione remota.

**\[18\] GrapheneOS Project:** [<u>Attestation and Verified Boot
Architecture</u>](https://grapheneos.org/articles/attestation-compatibility-guide).
Documentazione tecnica sull'uso di chiavi AVB personalizzate con
bootloader ribloccato e sui limiti imposti dai controlli proprietari di
Play Integrity.

**\[19\] Ross Anderson (University of Cambridge):** [<u>'Trusted
Computing' Frequently Asked
Questions</u>](https://www.cl.cam.ac.uk/archive/rja14/tcpa-faq.html)
(2003). Analisi storica sul ribaltamento del concetto di fiducia
informatica e sull'uso della crittografia hardware per togliere al
proprietario del computer il controllo sul software.

**\[20\] Cory Doctorow:** [<u>The Coming War on General Purpose
Computing</u>](https://youtu.be/HUEvRyemKSg?si=SAFIU8EPaNtVbNsk).
Intervento al 28° Chaos Communication Congress (28C3, 2011) sul
passaggio dai computer universali ai dispositivi chiusi e controllati
dai produttori.

### Capitolo 3

**\[21\] Istituto Poligrafico e Zecca dello Stato (IPZS):** [<u>CieID
Mobile Application
Architecture</u>](https://github.com/italia/cieid-android-sdk).
Repository ufficiale dell'SDK e del codice sorgente per l'autenticazione
tramite Carta d'Identità Elettronica su Android.

**\[22\] PagoPA S.p.A.:** [<u>Issue \#6327 sul repository ufficiale
GitHub</u>
<u>pagopa/io-app</u>](https://github.com/pagopa/io-app/issues/6327).
Discussione pubblica che conferma l'uso delle Play Integrity API e della
Key Attestation per bloccare l'attivazione dei documenti nell'IT Wallet
sui dispositivi sbloccati o con sistemi non certificati da Google.

**\[23\] European Digital Identity Wallet (EUDI):** [<u>Issue \#287 sul
repository ufficiale GitHub</u>
<u>eu-digital-identity-wallet/eudi-app-android-wallet-ui</u>](https://github.com/eu-digital-identity-wallet/eudi-app-android-wallet-ui/issues/287).
Discussione sull'implementazione dei controlli Play Integrity nei
portafogli di identità digitale europei e nazionali (inclusi Italia e
Francia).

**\[24\] Costituzione della Repubblica Italiana:** [<u>Articolo 3
(Principio di uguaglianza formale e
sostanziale)</u>](https://www.senato.it/istituzione/la-costituzione/principi-fondamentali/articolo-3).
Compito della Repubblica di rimuovere gli ostacoli economici e sociali
che limitano l'uguaglianza dei cittadini e la partecipazione alla vita
del Paese.

**\[25\] Decreto Legislativo 7 marzo 2005, n. 82:** [<u>Codice
dell'Amministrazione Digitale (CAD), Art. 3 (Diritto all'uso delle
tecnologie)</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2005-03-07;82).
Norma che garantisce a tutti i cittadini il diritto di accedere ai
servizi della Pubblica Amministrazione in modalità digitale.

**\[26\] Decreto Legislativo 7 marzo 2005, n. 82:** [<u>Codice
dell'Amministrazione Digitale (CAD), Art. 68 (Analisi comparativa delle
soluzioni e neutralità
tecnologica)</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2005-03-07;82).
Obbligo per la Pubblica Amministrazione di garantire la neutralità
tecnologica, usare standard aperti ed evitare la dipendenza da un
singolo fornitore.

**\[27\] Parlamento Europeo e Consiglio:** [<u>Direttiva (UE) 2015/2366
sui servizi di pagamento nel mercato interno
(PSD2)</u>](https://eur-lex.europa.eu/legal-content/IT/TXT/?uri=CELEX:32015L2366).
Normativa europea che introduce l'obbligo di autenticazione forte del
cliente (SCA, Art. 97), applicata dalla maggior parte delle banche
tramite le proprie app per smartphone.

**\[28\] Parlamento Europeo e Consiglio:** [<u>Direttiva 2014/92/UE
sull'accesso al conto di pagamento con caratteristiche di
base</u>](https://www.astrid-online.it/static/upload/Dire/Directive_Payment-Accounts_23_07_14.pdf)
*(recepita in Italia dal D.Lgs. 37/2017)*. Norma che garantisce a tutti
i consumatori il diritto di accedere e operare su un conto di pagamento
di base senza discriminazioni.

### Capitolo 4

**\[29\] Electronic Frontier Foundation (EFF):** [<u>Application
Gatekeeping: An Ever-Expanding Pathway to Internet
Censorship</u>](https://www.eff.org/deeplinks/2025/11/application-gatekeeping-ever-expanding-pathway-internet-censorship).
Analisi sulle crescenti restrizioni introdotte per ostacolare il
sideloading e l'installazione di software indipendente.

**\[30\] F-Droid / Open Source Community:** [<u>Keep Android Open
Campaign Declaration</u>](https://keepandroidopen.org/it/). Appello e
documentazione tecnica promossa da F-Droid e dalla comunità open source
contro gli avvisi allarmistici di Play Protect, le *Restricted Settings*
e gli obblighi di registrazione imposti agli sviluppatori.

**\[31\] Parlamento Europeo e Consiglio:** [<u>Regolamento (UE)
2022/1925 relativo a mercati equi e contendibili nel settore digitale
(Digital Markets
Act)</u>](https://eur-lex.europa.eu/eli/reg/2022/1925/oj?locale=it). In
particolare l'Articolo 6, paragrafo 4, che obbliga i *gatekeeper*
designati a permettere l'installazione e l'uso effettivo di app di terze
parti e di store alternativi.

**\[32\] European Environment Agency (EEA):** [<u>Europe's circular
economy: Smartphones and consumer
electronics</u>](https://www.eea.europa.eu/en/analysis/publications/europes-consumption-in-a-circular-economy-the-benefits-of-longer-lasting-electronics).
Studio sull'impatto ambientale del ciclo di vita ridotto degli
smartphone in Europa e sulla sostituzione anticipata causata da limiti
software.

**\[33\] Free Software Foundation Europe (FSFE):** [<u>Upcycling
Android: The Right to Install Any Software on Any
Device</u>](https://fsfe.org/activities/upcyclingandroid/). Iniziativa
europea che spiega perché il diritto di sbloccare i telefoni e
installare sistemi operativi liberi è fondamentale per combattere
l'obsolescenza programmata.

**\[34\] Fraunhofer IZM / Commissione Europea (JRC), Cordella et al.:**
[<u>Reducing the carbon footprint of ICT products through material
efficiency strategies: A life cycle analysis of
smartphones</u>](https://publications.jrc.ec.europa.eu/repository/handle/JRC124077)
*(vedi anche Fraunhofer IZM, [<u>Carbon savings reuse of ICT
equipment</u>](https://www.izm.fraunhofer.de/content/dam/izm/de/documents/Abteilungen/Environmental_Reliability_Engineering/Projekte/Carbon%20savings%20reuse%20of%20ICT%20equipment%20November_2022.pdf))*.
Studio sul ciclo di vita (LCA) che dimostra come fino all'80% delle
emissioni totali di gas serra di uno smartphone derivi dalla produzione
e dall'estrazione delle materie prime, rendendo il prolungamento della
vita del telefono la misura ecologica più importante.

**\[35\] Commissione Europea:** [<u>Regolamento (UE) 2023/1670 che
stabilisce i requisiti di progettazione ecocompatibile per smartphone e
tablet</u>](https://eur-lex.europa.eu/eli/reg/2023/1670/oj). Regolamento
europeo sull'Ecodesign che impone almeno 5 anni di aggiornamenti
software e di sicurezza, oltre alla disponibilità dei pezzi di ricambio.

**\[36\] Parlamento Europeo e Consiglio:** [<u>Direttiva (UE) 2024/825
sulla responsabilizzazione dei consumatori per la transizione
verde</u>](https://eur-lex.europa.eu/eli/dir/2024/825/oj?locale=it).
Normativa europea contro le pratiche commerciali scorrette legate alla
durata dei prodotti e agli aggiornamenti software.

**\[37\] Joint Research Centre (JRC) / Commissione Europea:**
[<u>Analysis of the impact of parts pairing on the repair and reuse of
mobile
phones</u>](https://susproc.jrc.ec.europa.eu/product-bureau/sites/default/files/2021-12/JRC_Report_Repair_Score_Smartphone_Tablets_v2.pdf).
Rapporto tecnico della Commissione Europea sull'indice di riparabilità
degli smartphone e sugli ostacoli creati dalla serializzazione dei
componenti (*parts pairing*).

**\[38\] Parlamento Europeo e Consiglio:** [<u>Direttiva (UE) 2024/1799
recante norme comuni che promuovono la riparazione dei
beni</u>](https://eur-lex.europa.eu/eli/dir/2024/1799/oj?locale=it).
Direttiva europea sul Diritto alla Riparazione (in particolare
l'Articolo 5 sul divieto di ostacolare l'uso di pezzi di ricambio usati,
compatibili o riparati tramite blocchi hardware o software).

**\[39\] Commissione Europea:** [<u>Regolamento (UE) 2023/1670
(Ecodesign per smartphone e tablet), Allegato
II</u>](https://eur-lex.europa.eu/eli/reg/2023/1670/oj). Requisiti
specifici sull'accesso alle riparazioni, sulla sostituzione dei
componenti e sulle informazioni per la manutenzione.

### Capitolo 5

**\[40\] Android Open Source Project (AOSP):** [<u>Android Verified Boot
(AVB): Architecture and Custom Key
Support</u>](https://source.android.com/docs/security/features/verifiedboot/avb?hl=it).
Specifiche tecniche ufficiali di AOSP sulla firma crittografica del
bootloader e sul supporto per l'installazione di una chiave di verifica
personale (avb_custom_key) su sistemi operativi di terze parti.

**\[41\] W3C / FIDO Alliance:** [<u>Web Authentication: An API for
accessing Public Key Credentials (WebAuthn Level
3)</u>](https://www.w3.org/TR/webauthn-3/). Standard aperto
internazionale per l'autenticazione crittografica forte, progettato per
funzionare su qualsiasi piattaforma e browser senza dipendere da sistemi
operativi proprietari.

**\[42\] Trattato sul Funzionamento dell'Unione Europea (TFUE):**
[<u>Articolo 102 (Divieto di abuso di posizione
dominante)</u>](https://eur-lex.europa.eu/legal-content/IT/TXT/?uri=CELEX:12012E/TXT).
Norma cardine del diritto antitrust europeo contro l'abuso di posizione
dominante, le vendite abbinate forzate (*tying*) e le barriere tecniche
alla concorrenza.

**\[43\] Decreto Legislativo 6 settembre 2005, n. 206:** [<u>Codice del
Consumo, Artt. 20-22 (Pratiche commerciali scorrette e
ingannevoli)</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2005-09-06;206).
Norme sulla trasparenza verso il consumatore, sull'omissione di
informazioni rilevanti e sulle pratiche che limitano la libertà di
scelta dell'acquirente.

**\[44\] Legge 10 ottobre 1990, n. 287:** [<u>Norme per la tutela della
concorrenza e del mercato, Art. 3 (Abuso di posizione
dominante)</u>](https://www.bosettiegatti.eu/info/norme/statali/1990_0287.htm).
Divieto nazionale di imporre condizioni ingiustificatamente gravose o di
bloccare l'accesso al mercato a concorrenti e riparatori indipendenti.

**\[45\] Legge 18 giugno 1998, n. 192:** [<u>Art. 9 (Abuso di dipendenza
economica)</u>](https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:legge:1998-06-18;192!vig=).
Norma che tutela le imprese e i professionisti che si trovano in una
posizione di dipendenza economica da un produttore e subiscono
condizioni contrattuali o tecniche arbitrarie.
