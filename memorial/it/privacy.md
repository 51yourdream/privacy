# Informativa sulla privacy di Virtual Memorial Space

**Data di entrata in vigore: 1° novembre 2026**

## 1. Introduzione

Virtual Memorial Space ("l'App", "noi") è un'app per iOS che consente di creare spazi commemorativi privati, celebrare riti di ricordo e scrivere lettere. Questa informativa sulla privacy spiega quali informazioni tratta l'App, dove vengono conservate e quali scelte hai a disposizione.

L'App non richiede un account. I tuoi contenuti commemorativi restano sul tuo dispositivo. Il nostro server viene usato solo per i gettoni commemorativi, gettoni facoltativi all'interno dell'App usati per stili di offerta più curati.

Usando l'App, confermi di aver letto e compreso questa informativa sulla privacy.

## 2. Informazioni che non raccogliamo

L'App non raccoglie né richiede:

- Il tuo nome, indirizzo email, numero di telefono o un account di accesso
- I nomi, le foto, le date, le descrizioni, le lettere o i messaggi dei tuoi spazi commemorativi
- L'accesso all'intera libreria foto, alla fotocamera, al microfono, ai contatti o alla posizione
- I dati della tua carta di pagamento
- Un identificatore pubblicitario (IDFA). L'App non ti traccia tra app o siti web di altre aziende e non mostra la richiesta di Trasparenza sul tracciamento delle app (ATT).
- Dati analitici o eventi di utilizzo. L'App non contiene alcun SDK di analisi né pubblicità.

## 3. Contenuti commemorativi conservati solo sul tuo dispositivo

Quanto segue viene salvato nello spazio di archiviazione privato dell'App sul tuo iPhone o iPad:

- Spazi commemorativi: nome, tipo (ad esempio una persona cara, partner, amico o animale domestico), descrizione, data di nascita, data di ricordo, tema e impostazione del promemoria
- Le foto che aggiungi a uno spazio commemorativo
- Registri dei riti: quale candela, fiore o offerta di carta è stata usata, il numero di gettoni spesi, l'ora e l'eventuale messaggio aggiunto
- Le lettere che scrivi, comprese le bozze
- Preferenze: lingua, effetti ridotti, visualizzazione o meno delle offerte di carta tradizionali, completamento dell'introduzione, un indicatore di sincronizzazione acquisti in sospeso e un contatore che limita le richieste di valutazione
- L'ultimo saldo di gettoni ricevuto dal nostro server, usato solo per la visualizzazione offline

Questi contenuti non vengono caricati sul nostro server, non sono usati per la pubblicità e non sono usati per alcuna funzione o addestramento di intelligenza artificiale (IA). Se il backup di iCloud è attivo, iOS può includere questi dati nel backup del dispositivo, gestito da Apple con il tuo ID Apple. L'App non ha una propria sincronizzazione cloud.

**Foto.** Scegli le foto tramite il selettore foto di sistema. L'App riceve solo le foto selezionate e non accede all'intera libreria foto. Una copia compressa di ogni foto selezionata viene salvata nello spazio di archiviazione dell'App.

## 4. Gettoni commemorativi e il nostro server

I gettoni commemorativi sono acquisti in-app di tipo consumabile. Perché il saldo resti disponibile anche dopo aver reinstallato l'App, viene conservato sul nostro server ("appapi"), ospitato su Vercel, che archivia i dati in Vercel KV (Upstash Redis).

Il server conserva solo:

- Un ID utente generato casualmente, non collegato al tuo nome, al tuo indirizzo email o al tuo ID Apple
- Un'impronta (hash) del token di accesso emesso per quell'ID utente. Il token vero e proprio non viene conservato sul server.
- Il tuo saldo di gettoni
- Registri di acquisto: ID prodotto, ID transazione Apple, numero di gettoni e ora
- Registri di spesa: ID dell'offerta (ad esempio un tipo di candela), numero di gettoni, la chiave di richiesta che evita un doppio addebito, saldo successivo e ora
- Uno storico di accrediti, spese e rimborsi con importi e ID di transazione o di spesa correlati

Ogni richiesta al server include anche la versione dell'App e un identificatore del dispositivo (l'identifierForVendor di iOS), usati per verificare la firma della richiesta. Come per qualsiasi servizio web, il nostro fornitore di hosting può trattare il tuo indirizzo IP nei normali log delle richieste per fornire e proteggere il servizio.

Il server non conserva il tuo nome, il tuo indirizzo email né alcuna informazione sulle persone o sugli animali che ricordi: nessun nome, foto, lettera o messaggio commemorativo.

L'ID utente e il token sono conservati nel portachiavi iOS del tuo dispositivo. Possono essere sincronizzati tramite il portachiavi iCloud, così il saldo resta disponibile dopo aver reinstallato l'App o su un altro dispositivo con lo stesso ID Apple.

## 5. Acquisti

- **Apple (App Store)** elabora tutti i pagamenti tramite il tuo ID Apple. Non riceviamo mai i dati della tua carta di pagamento. Informativa sulla privacy di Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** convalida le transazioni. RevenueCat riceve l'ID utente casuale sopra indicato, informazioni sulla transazione (come ID prodotto, ID transazione Apple e ora di acquisto) e informazioni tecniche di base come versione dell'App, versione del sistema operativo e paese dell'App Store. Il nostro server chiede a RevenueCat di confermare gli acquisti e RevenueCat comunica al nostro server acquisti e rimborsi, così i gettoni vengono accreditati una sola volta e ritirati dopo un rimborso. Informativa sulla privacy di RevenueCat: https://www.revenuecat.com/privacy

I gettoni commemorativi non hanno alcun valore monetario reale. I rimborsi sono gestiti da Apple secondo le sue regole. I termini d'uso sono il contratto di licenza standard di Apple: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Notifiche (facoltative)

Se attivi un promemoria per la data di ricordo di uno spazio, l'App chiede il permesso per le notifiche e programma notifiche locali sul tuo dispositivo. I promemoria non passano dal nostro server. Puoi disattivarli nell'App o nelle Impostazioni di iOS.

## 7. Come usiamo le informazioni

Usiamo le informazioni sopra indicate solo per:

- Mostrare e conservare sul tuo dispositivo spazi commemorativi, riti e lettere
- Creare il tuo portafoglio di gettoni, accreditare i gettoni acquistati una sola volta per transazione, scalare gettoni quando scegli un'offerta premium e ritirare gettoni dopo un rimborso
- Verificare le richieste e prevenire frodi o accrediti doppi
- Rispondere alle tue richieste di assistenza

Non vendiamo né affittiamo informazioni personali, non le usiamo per la pubblicità e non creiamo profili pubblicitari.

## 8. Condivisione

Condividiamo informazioni solo con i fornitori necessari al funzionamento dell'App (Apple, RevenueCat e Vercel / Upstash per hosting e archiviazione), oppure quando richiesto dalla legge o da un valido procedimento legale.

## 9. Eliminare i tuoi dati

Nelle Impostazioni dell'App:

- **Elimina tutti i dati (Delete All Data)** elimina tutti i contenuti commemorativi su questo dispositivo: spazi commemorativi, foto, registri dei riti, lettere e messaggi.
- **Elimina dati dei gettoni (Delete Token Data)** elimina il tuo portafoglio sul nostro server: il record dell'ID utente, l'hash del token, il saldo, i registri di acquisto e di spesa e lo storico. Il saldo viene azzerato e non può essere ripristinato. Per evitare che lo stesso acquisto venga accreditato di nuovo, conserviamo solo l'ID transazione Apple (con il relativo ID prodotto), senza l'ID utente. Successivamente l'ID utente e il token vengono rimossi anche dal portachiavi.

Eliminare l'App rimuove i suoi contenuti locali dal dispositivo, ma **non** elimina il tuo portafoglio sul nostro server. Per eliminarlo, usa "Elimina dati dei gettoni" prima di eliminare l'App oppure contattaci. I dati locali eliminati possono rimanere in backup iCloud precedenti del dispositivo finché Apple non li sostituisce o li elimina.

Puoi anche chiederci di richiedere a RevenueCat la cancellazione del record di acquisto che conserva.

## 10. Sicurezza e conservazione

Le connessioni con il nostro server, Apple e RevenueCat usano HTTPS cifrato. Le richieste sono firmate, il server conserva solo un hash del tuo token e la tua identità è custodita nel portachiavi iOS. Nessun metodo di archiviazione o trasmissione è completamente sicuro.

- I contenuti locali restano finché non li elimini o elimini l'App.
- I dati del portafoglio sul server restano finché non usi "Elimina dati dei gettoni" o ci chiedi di eliminarli.
- Gli ID transazione Apple senza ID utente vengono conservati per evitare accrediti doppi.
- Apple e RevenueCat conservano i registri di acquisto secondo le proprie politiche e i propri obblighi di legge.

## 11. Privacy dei minori

Virtual Memorial Space non è rivolta ai minori. Non raccogliamo consapevolmente informazioni personali da minori di 13 anni (o dell'età minima prevista nel tuo paese). Se ritieni che un minore ci abbia fornito informazioni personali, contattaci e le elimineremo.

## 12. Trattamento internazionale

I nostri fornitori di hosting e archiviazione e RevenueCat possono trattare dati negli Stati Uniti o in paesi diversi dal tuo. Per tale trattamento ci affidiamo alle garanzie di questi fornitori.

## 13. I tuoi diritti

A seconda di dove vivi, potresti avere il diritto di accedere, rettificare, cancellare o limitare il trattamento delle tue informazioni personali. La maggior parte dei dati si trova sul tuo dispositivo ed è sotto il tuo controllo. Per i dati sul nostro server, usa "Elimina dati dei gettoni" o contattaci. Potremmo chiederti informazioni utili a individuare i record interessati.

## 14. Modifiche alla presente informativa

Potremmo aggiornare questa informativa sulla privacy. In tal caso la data in alto cambierà. Se l'App inizierà a raccogliere nuovi tipi di dati, aggiorneremo prima questa informativa.

## 15. Contatti

Per domande su questa informativa sulla privacy, contattaci:

- Email: lpjustdoit@163.com

---

## Altre lingue

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
