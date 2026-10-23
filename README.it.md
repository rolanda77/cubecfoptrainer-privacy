# Note legali e informativa sulla privacy – CFOP Trainer

[Deutsch (versione vincolante)](README.md) · [English](README.en.md) · [Français](README.fr.md) · **Italiano** · [Español](README.es.md)

*Traduzione di cortesia. In caso di discrepanze fa fede esclusivamente la versione tedesca.*

## Note legali (Impressum)

Informazioni ai sensi del § 5 DDG (legge tedesca sui servizi digitali, in precedenza § 5 TMG):

Roland Albrecht
Im Jägeracker 42
79312 Emmendingen
Germania

Contatto: rca@quantentunnel.de

## Informativa sulla privacy

Data: 18/10/2026

### 1. Titolare del trattamento

Roland Albrecht
E-mail: rca@quantentunnel.de

La persona sopra indicata, in qualità di sviluppatore dell'app "CFOP/Fridrich-Algorithmen-Trainer" (di seguito "l'app"), è titolare ai sensi del Regolamento generale sulla protezione dei dati (GDPR) dei trattamenti descritti di seguito.

### 2. In sintesi

L'app non raccoglie, non conserva e non trasmette **alcun dato personale allo sviluppatore o a terzi**. Non ci sono:

- account utente né accesso,
- connessione a internet (l'app non richiede la relativa autorizzazione e non comunica con alcun server),
- servizi di analisi, tracciamento o pubblicità (nessun Google Analytics, nessun SDK di segnalazione degli arresti anomali o pubblicitario),
- trasmissioni di dati a terzi, dato che nessun dato lascia il dispositivo.

Tutti i dati generati nell'app restano esclusivamente in locale sul dispositivo dell'utente. Lo stesso vale per il collegamento Bluetooth facoltativo a uno smart cube: avviene solo direttamente tra dispositivo e cubo, senza accesso alla posizione (sezione 5).

### 3. Quali dati vengono salvati in locale sul dispositivo?

Per svolgere le sue funzioni di allenamento (allenamento degli algoritmi, corso guidato, ripasso con ripetizione dilazionata), l'app salva i seguenti dati **esclusivamente in locale, in un database sul dispositivo**:

- statistiche di allenamento ed esercizio per ogni caso di algoritmo (ad es. numero di tentativi, percentuale di successo),
- dati di pianificazione e scadenza dei ripassi con ripetizione dilazionata (data del prossimo ripasso di ogni caso),
- progressi nel corso guidato (livelli e casi già sbloccati o consolidati),
- varianti di sequenze di mosse salvate dall'utente per singoli casi,
- lingua scelta per l'app (tedesco, inglese, francese, italiano o spagnolo) e altre impostazioni dell'app (ad es. impostazione predefinita della vista adesivi, visualizzazione della serie giornaliera).
- in caso di uso di uno smart cube (sezione 5): nome e indirizzo Bluetooth dell'ultimo cubo collegato con le relative impostazioni (collegamento automatico, uso dell'orientamento del cubo) e, per ogni tentativo, se è stato eseguito con il tocco o con lo smart cube.

Questi dati sono memorizzati sul dispositivo tramite un database Room locale (SQLite) e la memorizzazione locale delle impostazioni (SharedPreferences). Non si tratta di una trasmissione allo sviluppatore: nessuno, oltre alla persona che usa il dispositivo, ha accesso a questi dati.

### 4. Funzione di backup (file di backup locale)

Nelle impostazioni l'app offre la possibilità facoltativa di creare un file di backup locale con le statistiche di successo, la cronologia dei tentativi con pianificazione e scadenze dei ripassi, i progressi nel corso, le varianti di algoritmo preferite e gli algoritmi salvati dall'utente, e di ricaricare un file di backup creato in precedenza. Il file viene salvato o letto esclusivamente tramite la finestra di selezione dei file fornita dal sistema operativo, in una posizione scelta dall'utente: l'app non sceglie automaticamente alcuna posizione e non trasmette mai il file allo sviluppatore o a terzi. Se l'utente sceglie come posizione una cartella sincronizzata con un servizio cloud (ad es. un'integrazione Drive o OneDrive del dispositivo), l'ulteriore trattamento del file è soggetto all'informativa sulla privacy del rispettivo fornitore cloud, non a quella di questa app.

### 5. Collegamento Bluetooth a uno smart cube (facoltativo)

Da Android 12 l'app può essere collegata in modo facoltativo a un cubo di Rubik Bluetooth ("smart cube", attualmente GAN i4 e GoCube) che comunica all'app le mosse eseguite sul cubo. La funzione è volontaria; senza di essa l'app resta completamente utilizzabile con il tocco.

- **Collegamento solo locale:** l'app cerca smart cube nelle vicinanze tramite Bluetooth Low Energy e si collega direttamente al cubo scelto. Non sono coinvolti server, account del produttore o connessioni internet.
- **Dati trattati:** dal cubo l'app riceve esclusivamente eventi di mossa (quale faccia è stata girata e in quale verso, con indicazione temporale), eventi di orientamento (posizione del cubo nello spazio), il livello della batteria e nome del dispositivo, modello e informazioni hardware. Questi dati servono solo per l'esercizio in corso; ne vengono salvati solo i normali dati di allenamento della sezione 3 (sequenza di mosse, tempo e valutazione di un tentativo, con in più la fonte di input).
- **Cubo salvato:** per potersi ricollegare allo stesso cubo all'avvio successivo, l'app salva in locale sul dispositivo il suo nome e il suo indirizzo Bluetooth. Questa voce può essere eliminata in qualsiasi momento con "Rimuovi" nel menu smart cube. Queste informazioni non fanno parte del file di backup (sezione 4).
- **Nessun accesso alla posizione:** l'app usa solo l'autorizzazione "Dispositivi nelle vicinanze" (sezione 8) e dichiara espressamente al sistema di non ricavare alcuna posizione dalla ricerca Bluetooth. Gli altri dispositivi Bluetooth trovati non vengono né mostrati né salvati.
- **Nessuna trasmissione:** né i dati del cubo né l'indirizzo Bluetooth salvato lasciano il dispositivo.

### 6. Nessuna trasmissione di dati, nessun server, nessun account

L'app non richiede e non possiede l'autorizzazione di accesso a internet. Pertanto, attraverso l'app non avviene mai alcuna trasmissione di dati allo sviluppatore, a Google o ad altri terzi. Non ci sono account utente, registrazione né sincronizzazione cloud.

### 7. Nessun servizio di analisi, tracciamento o pubblicità

L'app non contiene software di analisi (ad es. Firebase Analytics), servizi di segnalazione degli arresti anomali (ad es. Crashlytics) né SDK pubblicitari. Non vengono creati profili di utilizzo, non viene determinata la posizione e non viene letto l'ID pubblicitario.

### 8. Autorizzazioni dell'app

L'app non richiede particolari autorizzazioni di accesso al dispositivo (ad es. nessun accesso a fotocamera, posizione, contatti, microfono o internet), con un'eccezione: per il collegamento facoltativo a uno smart cube (sezione 5) usa da Android 12 l'autorizzazione "Dispositivi nelle vicinanze" (`BLUETOOTH_SCAN` con l'indicazione che non viene ricavata alcuna posizione, e `BLUETOOTH_CONNECT`). Viene richiesta solo quando l'utente cerca o collega un cubo nel menu smart cube e può essere revocata in qualsiasi momento nelle impostazioni Android; il resto dell'app funziona anche senza. La funzione di backup (sezione 4) usa la finestra di selezione dei file del sistema (Storage Access Framework), che non richiede autorizzazioni aggiuntive.

### 9. Durata della conservazione e cancellazione

I dati indicati nella sezione 3 restano salvati in locale sul dispositivo finché:

- vengono azzerati tramite le funzioni integrate nell'app (ad es. "Azzera" nelle statistiche o "Elimina i tuoi algoritmi" nelle impostazioni), oppure
- vengono rimossi completamente dal dispositivo disinstallando l'app.

Lo smart cube salvato (sezione 5) può inoltre essere eliminato in qualsiasi momento con "Rimuovi" nel menu smart cube.

Poiché nessun dato viene salvato al di fuori del dispositivo, dopo la disinstallazione non esiste più alcuna copia dei dati – ad eccezione di un file di backup creato dall'utente (sezione 4), che rimane nella posizione scelta indipendentemente dall'app e può essere eliminato dall'utente stesso in caso di necessità.

### 10. Diritti dell'interessato

Poiché l'app non trasmette dati personali allo sviluppatore, tutti i dati indicati nella sezione 3 sono esclusivamente sotto l'accesso diretto e il pieno controllo dell'utente (accesso, rettifica e cancellazione avvengono direttamente tramite l'app o disinstallandola). Per domande sulla protezione dei dati relative all'app è comunque possibile usare in qualsiasi momento il contatto indicato nella sezione 1.

### 11. Minori

L'app non si rivolge specificamente ai bambini e non raccoglie alcun dato personale, indipendentemente dall'età dell'utente.

### 12. Modifiche alla presente informativa

La presente informativa sulla privacy può essere aggiornata se necessario, ad esempio quando nuove funzioni dell'app lo richiedono. La versione in vigore è disponibile all'indirizzo indicato nella scheda del Play Store.

### 13. Contatto

Per domande su questa informativa sulla privacy o sull'app scrivi a:

rca@quantentunnel.de
