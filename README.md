<div align="center">

<a href="https://investfood.it"><img src="https://static.wixstatic.com/media/cb2700_2b9dbe5db69f4506b8e416bcf20269f6~mv2.png" height="60" alt="Invest Food"/></a>

# Engineering Portfolio

**Full-stack engineering across web, mobile, backend, data and AI for a multi-brand food group**

<p>
<img src="https://img.shields.io/badge/status-in_production-success?style=flat-square" alt="status"/>
<img src="https://img.shields.io/badge/platforms-web%20%C2%B7%20iOS%20%C2%B7%20Android%20%C2%B7%20Wear_OS%20%C2%B7%20Kiosk-blue?style=flat-square" alt="platforms"/>
<img src="https://img.shields.io/badge/cloud-Google_Cloud%20%C2%B7%20Firebase-orange?style=flat-square" alt="cloud"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-purple?style=flat-square" alt="AI"/>
<img src="https://img.shields.io/badge/lang-IT%20%C2%B7%20EN-lightgrey?style=flat-square" alt="lang"/>
</p>

<p>
<a href="#italiano"><b>Italiano</b></a> · <a href="#english"><b>English</b></a>
</p>

</div>

---

<a id="investfood-tech-system"></a>

<div align="center">

<a href="https://investfood.tech/">
<picture>
<source media="(prefers-color-scheme: dark)" srcset="https://investfood.tech/assets/img/mark-white.png"/>
<img src="https://onebooking-app.web.app/logo-icon.png" height="72" alt="InvestFood Tech System"/>
</picture>
</a>

</div>

## InvestFood Tech System

> **Il sistema operativo completo per la ristorazione** · <a href="https://investfood.tech/"><b>investfood.tech</b></a>

Nove gestionali, un solo dato. Ogni prodotto funziona da solo, ma parlano tutti la stessa lingua: ogni scontrino battuto in K-POS diventa un numero in AtomicBI, i consumi scendono in SupplyONE, i turni si chiudono in Platform ONE. Cinque lingue, multi-locale e multi-brand, permessi per ruolo, confronti fra locali. Costruito sui sette brand del gruppo e provato ogni giorno in servizio.

---

## Indice / Index

> **Italiano**
>
> 1. [K-POS](#k-pos) · sistema di cassa cloud multi-azienda per bar, ristoranti e catene
> 2. [InvestAI](#investai) · piattaforma di intelligenza artificiale per il food and beverage
> 3. [AtomicBI](#atomicbi) · piattaforma BI multi-canale per la ristorazione multi-brand
> 4. [BiteOS](#biteos) · sistema operativo della ristorazione (loyalty, ordini, pagamenti, kiosk)
> 5. [Platform ONE](#platform-one) · HR all-in-one multi-tenant per ristorazione e retail
> 6. [SupplyONE](#supplyone) · ERP cloud-native per food cost, magazzino e HACCP
> 7. [OneBooking](#onebooking) · gestione prenotazioni e sala per ristoranti
> 8. [TicketOS](#ticketos) · assistenza tecnica e manutenzione per reti di locali
> 9. [Bite Radio](#bite-radio) · la radio del gruppo, in onda 24 ore su 24
>
> **English**
>
> 1. [K-POS](#k-pos-en) · multi-company cloud POS for bars, restaurants and chains
> 2. [InvestAI](#investai-en) · artificial intelligence platform for food and beverage
> 3. [AtomicBI](#atomicbi-en) · multi-channel BI platform for multi-brand restaurant chains
> 4. [BiteOS](#biteos-en) · the operating system of restaurants (loyalty, ordering, payments, kiosk)
> 5. [Platform ONE](#platform-one-en) · all-in-one multi-tenant HR for hospitality and retail
> 6. [SupplyONE](#supplyone-en) · cloud-native ERP for food cost, inventory and HACCP
> 7. [OneBooking](#onebooking-en) · reservation and front-of-house management for restaurants
> 8. [TicketOS](#ticketos-en) · technical support and maintenance for venue networks
> 9. [Bite Radio](#bite-radio-en) · the group's radio station, on air 24 hours a day

---

<a id="italiano"></a>

## Italiano

> Nove prodotti complementari progettati e sviluppati per **InvestFood SRL**. Un sistema di cassa cloud, una piattaforma di intelligenza artificiale, una piattaforma BI multi-canale, una piattaforma di loyalty / ordini / kiosk, una piattaforma HR all-in-one, un ERP cloud-native per food cost e magazzino, la gestione delle prenotazioni, l'assistenza tecnica e la radio del gruppo. Quasi tutti in produzione, con client nativi iOS, Android, Wear OS e web in parità feature.

---

<a id="k-pos"></a>

### 1. K-POS

> **Sistema di cassa cloud multi-azienda per bar, ristoranti e catene**

<p>
<img src="https://cdn.simpleicons.org/nestjs/E0234E" height="22" alt="NestJS"/>&nbsp;
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/prisma/2D3748" height="22" alt="Prisma"/>&nbsp;
<img src="https://cdn.simpleicons.org/nextdotjs/000000" height="22" alt="Next.js"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/kotlin/7F52FF" height="22" alt="Kotlin"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/redis/DC382D" height="22" alt="Redis"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

#### Cosa risolve

Un locale non batte solo scontrini: stampa comande in cucina, incassa su terminale, emette documenti fiscali e fatture elettroniche, e nello stesso servizio riceve ordini da Glovo, Just Eat, Deliveroo, dal QR sul tavolo e dal menu digitale. Ognuno di questi flussi, preso da solo, ha il suo sistema e la sua verità. **K-POS** li tiene tutti sulla stessa: un backend cloud, un pannello web dove si configura una volta per tutti i locali, e un'app iPad nativa che continua a lavorare anche quando la rete cade.

#### Architettura

- **Backend** NestJS 10 su Express 5, TypeScript in modalità rigorosa senza `any`, Prisma 6
- **Database** Cloud SQL PostgreSQL in schema dedicato, dietro PgBouncer in transaction pool, raggiunto via connettore Cloud SQL senza IP pubblico
- **Code e cache** Redis con BullMQ per stampa, sincronizzazione canali e pubblicazioni pianificate
- **Pannello web** Next.js 15 App Router, React 19, TailwindCSS, TanStack Query
- **App iPad nativa** SwiftUI (iPadOS 16+) con database locale GRDB e coda di sincronizzazione idempotente
- **K-Display** app Android per lo schermo rivolto al cliente, **K-POS Sala** app Wear OS per chi porta i piatti
- **Cloud Run** in regione europea, log strutturati e tracciamento errori con Sentry

#### Moduli

**Cassa e sala**
- Presa ordine per tavolo, asporto e consegna, con piantina della sala
- Conti separati, spostamento e unione dei tavoli, sconti, mancia e resto
- Comande su stampanti ESC/POS di rete e schermo di cucina (KDS)
- Chiamate al bracciale di sala: piatto pronto, asporto completo, tavolo da pulire
- Modalità mancino, tema scuro, pannelli riposizionabili, quattro lingue

**Fiscale**
- Documento commerciale sul registratore telematico via LAN, con reso e annullo
- Fattura elettronica con canale diretto SDICoop verso l'Agenzia delle Entrate
- Sezionali, corrispettivi e archivio dei documenti emessi
- Blocco loyalty stampato in coda al preconto e al documento fiscale

**Catalogo e listini**
- Categorie, varianti, componibili, allergeni e sospensione a tempo dei prodotti
- Cinque listini per canale e nomi diversi per menu, brand, locale e canale
- Il menu salvato nel pannello arriva in cassa nell'istante, senza ripubblicare nulla

**Canali di vendita**
- Connettori propri per Glovo, Just Eat e Deliveroo, più il ponte Deliverect
- Menu digitale, Ordine al Tavolo e Paga al Tavolo da QR, con conto che si divide
- Pubblicazione dei menu e apertura dei negozi pianificate per orario, giorni e fuso

**Pagamenti**
- Terminali Satispay, SumUp, Stripe, Revolut, Nexi e VRP, con credenziali per locale
- Buoni pasto a valore facciale che per legge non danno resto, resi e storni riconciliati

**Piattaforma**
- Multi-azienda con brand e locali, licenze e permessi granulari per ruolo
- Apparecchi attivati con codice e PIN operatore, revocabili in un tocco
- Control plane remoto per correggere il comportamento dell'app senza attendere un rilascio
- Audit log, sincronizzazione offline e scritture idempotenti arbitrate dal database

#### Integrazioni

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/Deliverect_Logo_Primary.svg/3840px-Deliverect_Logo_Primary.svg.png" height="28" alt="Deliverect"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/165162/1753464414-glovo-on-demand-deliverect-logo.svg" height="26" alt="Glovo"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.simpleicons.org/deliveroo/00CCBC" height="24" alt="Deliveroo"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.simpleicons.org/justeat/FF8000" height="24" alt="Just Eat"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/133951/1720164277-group-1321316881.svg" height="24" alt="Satispay"/>&nbsp;&nbsp;&nbsp;
<img src="https://1000logos.net/wp-content/uploads/2021/05/Stripe-logo.png" height="28" alt="Stripe"/>&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/MultiSafepay/MultiSafepay-icons/master/methods/revolut%403x.png" height="24" alt="Revolut"/>&nbsp;&nbsp;&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Nexi_Logo.svg/250px-Nexi_Logo.svg.png" height="20" alt="Nexi"/>
</p>

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/Edenred.svg/250px-Edenred.svg.png" height="22" alt="Edenred"/>&nbsp;&nbsp;&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfarepellegrini_bianco.svg"/><img src="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfare-pellegrini_colori.svg" height="26" alt="Welfare Pellegrini"/></picture>&nbsp;&nbsp;&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Sodexo_logo.svg/250px-Sodexo_logo.svg.png" height="20" alt="Sodexo"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.day.it/Media/Images/hp/UP-Day-logo.png" height="26" alt="Up Day"/>
</p>

Glovo · Just Eat · Deliveroo · Deliverect · BiteOS (loyalty, Paga al Tavolo, consigli al cameriere) · Platform ONE (timbrature da chiosco QR) · SupplyONE (giacenze in cassa) · OneBooking (agenda prenotazioni) · TicketOS (assistenza dalla cassa) · Agenzia delle Entrate (SDICoop) · registratori telematici Epson · stampanti ESC/POS di rete · terminali Satispay, SumUp, Stripe, Revolut, Nexi e VRP · buoni pasto Edenred, Welfare Pellegrini, Sodexo e Up Day · Firebase (Auth, FCM) · Google Cloud Storage

#### Sicurezza

- JWT Firebase per le persone, credenziale di apparecchio per iPad, schermi e orologi
- Ogni gestore di rotta dichiara il permesso richiesto, e uno script in integrazione continua verifica che nessuno se lo dimentichi
- Isolamento multi-azienda con suite end to end dedicata al perimetro
- Database senza IP pubblico, segreti in Secret Manager, chiavi di integrazione versionate
- Rate limiting, Helmet, CORS allowlist, audit log persistente
- Revoca istantanea dell'apparecchio, scritture idempotenti, nessuna cassa privilegiata sulle altre

#### Lingue supportate

Italiano · Inglese · Francese · Tedesco

#### Stack

<p>
<img src="https://img.shields.io/badge/NestJS-10-E0234E?style=flat-square&logo=nestjs&logoColor=white" alt="NestJS"/>
<img src="https://img.shields.io/badge/TypeScript-strict-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Prisma-6-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Redis-BullMQ-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
<img src="https://img.shields.io/badge/Next.js-15-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js"/>
<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/SwiftUI-iPadOS_16+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/GRDB-offline_first-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="GRDB"/>
<img src="https://img.shields.io/badge/Jetpack_Compose-Android%20%C2%B7%20Wear_OS-4285F4?style=flat-square&logo=android&logoColor=white" alt="Compose"/>
<img src="https://img.shields.io/badge/Cloud_Run-managed-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Run"/>
</p>

#### Ruolo

**Full-stack lead developer**. Architettura backend, pannello web, app iPad nativa, app Android per lo schermo cliente e per gli orologi di sala, connettori delivery, catena fiscale e fatturazione elettronica end-to-end.

---

<a id="investai"></a>

### 2. InvestAI

> **Piattaforma di intelligenza artificiale per il food and beverage**

<p>
<img src="https://img.shields.io/badge/AI-previsione_della_domanda-8E75B2?style=flat-square" alt="Forecasting"/>
<img src="https://img.shields.io/badge/AI-assistente_conversazionale-D97757?style=flat-square" alt="Conversational"/>
<img src="https://img.shields.io/badge/licenza-white_label-4285F4?style=flat-square" alt="White label"/>
<img src="https://img.shields.io/badge/uscita-2027-lightgrey?style=flat-square" alt="2027"/>
</p>

#### Cosa risolve

La domanda che un ristorante si pone ogni giorno è sempre la stessa: quanto serve, dove e quando. Oggi la risposta è intuito, e l'intuito sbaglia in un senso solo, verso lo spreco. **InvestAI** trasforma quella domanda in una previsione misurata, e la previsione in una proposta operativa: non un cruscotto da interpretare, ma un ordine fornitore già compilato, un turno già dimensionato, un piatto già segnalato come a rischio.

#### Tre livelli

- **AI operativa** per la gestione del locale: previsioni, ordini, turni, sprechi
- **AI conversazionale** rivolta direttamente al cliente finale
- **Piattaforma in licenza** white-label per catene esterne al gruppo

#### Moduli

**Previsione e approvvigionamento**
- Previsione della domanda per locale, articolo e fascia oraria, fino alla finestra di consegna da trenta minuti
- Margine di errore dichiarato accanto a ogni previsione, perché una stima senza incertezza non è una stima
- Ordini ai fornitori generati e allineati alle previsioni

**Margine e menu**
- Food cost e marginalità in tempo reale, sui prezzi effettivi
- Menu engineering che incrocia margine e popolarità
- Riduzione degli sprechi con segnalazione degli articoli a rischio

**Persone e clienti**
- Pianificazione del personale sul traffico atteso
- Assistente conversazionale per ordini in linguaggio naturale e domande sugli allergeni
- Personalizzazione e loyalty sullo storico del singolo cliente

#### Dati di addestramento

Oltre cento locali diretti, sette brand della ristorazione italiana, circa tredicimila clienti al giorno. Non un modello addestrato su dati di settore comprati, ma sull'operatività reale del gruppo che lo usa.

#### Destinatari

Catene e franchising · operatori delivery first · fornitori e produttori · travel retail e centri commerciali

#### Stato

In sviluppo, uscita prevista nel 2027.

#### Ruolo

**Full-stack lead developer**. Architettura della piattaforma, modelli di previsione, assistente conversazionale e integrazione con i sistemi operativi del gruppo.

---

<a id="atomicbi"></a>

### 3. AtomicBI

> **Piattaforma BI multi-canale per la ristorazione multi-brand**

<p>
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/android/3DDC84" height="22" alt="Android"/>&nbsp;
<img src="https://cdn.simpleicons.org/python/3776AB" height="22" alt="Python"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

#### Cosa risolve

Una catena multi-brand del food genera ogni giorno dati che vivono in silos: POS, delivery aggregator, sistemi HR, timbrature, ERP magazzino, pagamenti multi-PSP, contabilità. **AtomicBI** unifica tutto in un'unica fonte di verità, un data warehouse PostgreSQL, esposto via API e consumato da tre client nativi (web, iOS, Android) con un'estesa suite di moduli funzionali.

#### Architettura

- **Web** React 19 + Vite 7 + TailwindCSS su Firebase Hosting
- **iOS nativa** SwiftUI con architettura MVVM (iOS 15+)
- **Android nativa** Jetpack Compose + Material 3
- **Backend** Cloud Functions Python 3.11 in region europea
- **Data warehouse** Cloud SQL PostgreSQL con PgBouncer in transaction pool
- **Real-time** Firestore listener per RBAC, master data, alert e push token

#### Moduli

**Business Intelligence**
- Weekly e Monthly Business Review con trend storici, breakdown per canale e confronto YoY
- Report Store Manager con deep-dive AOV, payment mix e fasce orarie
- Investor Relations multilingua (IT, EN, FR, DE) con KPI YTD, EBITDA, headcount e data room
- Analytics per le piattaforme operative (loyalty, HR, supply chain)

**Operations & Finance**
- Chiusura giornaliera con formule canoniche, check di controllo e archivio foto
- Riconciliazione automatica fatture, corrispettivi e versamenti
- Moduli versamenti, fatture estere ed errori corrispettivi
- Menu engineering con suggerimenti di pricing

**AI & Automation**
- **AtomicAI Chat** conversazionale sul data warehouse che cita le query SQL eseguite
- **Daily Digest AI** su Slack con news food e QSR
- Report Builder drag and drop con formula editor ed export PDF, Excel, Word

**User Experience**
- Push notifications con scheduling e template variables
- Sidebar dinamica personalizzabile per utente senza redeploy

#### Integrazioni

Sistema POS · piattaforme di delivery aggregator (Deliveroo, Glovo, Uber Eats, JustEat, Deliverect) · Satispay · provider buoni pasto · sistema HR · sistema timbrature · ERP magazzino · Firebase (Auth, FCM, Storage) · LLM multi-provider · OpenMeteo · Gmail API · Slack Webhooks · OpenStreetMap

#### Sicurezza

- JWT Firebase con RBAC granulare per pagina, store e reparto
- Secret Manager e database senza IP pubblico
- HTTPS enforced e audit trail completo
- Soft delete sui dati sensibili
- Sincronizzazione provider auth e store dati su delete utente

#### Stack

<p>
<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Vite-7-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/>
<img src="https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind"/>
<img src="https://img.shields.io/badge/SwiftUI-iOS_15+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/Jetpack_Compose-Material_3-4285F4?style=flat-square&logo=android&logoColor=white" alt="Compose"/>
<img src="https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/PostgreSQL-15-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Google_Cloud-Functions%20%C2%B7%20SQL%20%C2%B7%20Firebase-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="GCP"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-D97757?style=flat-square" alt="LLM"/>
</p>

#### Ruolo

**Full-stack lead developer**. Architettura, backend, web, iOS, Android, data pipeline e AI integration end-to-end.

---

<a id="biteos"></a>

### 4. BiteOS

> **Il sistema operativo della ristorazione multi-brand**

<p>
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/fastify/000000" height="22" alt="Fastify"/>&nbsp;
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/android/3DDC84" height="22" alt="Android"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/redis/DC382D" height="22" alt="Redis"/>&nbsp;
<img src="https://cdn.simpleicons.org/stripe/635BFF" height="22" alt="Stripe"/>
</p>

#### Cosa risolve

Gestire più brand del food su decine di location significa coordinare POS, kiosk, app, ordini online, delivery di terze parti, loyalty, promo, gift card, eventi e pagamenti multi-PSP per location. **BiteOS** fa parlare tutti questi sistemi tra loro, mantenendo un'unica fonte di verità per cliente, ordine e punti fedeltà.

#### Architettura

- **Backend** Fastify + TypeScript ESM su Google Cloud Run
- **PostgreSQL** Cloud SQL + PgBouncer in transaction pool
- **Redis** per cache di locations, menu e transazioni
- **VPC privata** backend e database senza esposizione su IP pubblico
- **Webhook PSP isolati** in sub-plugin con raw body parser dedicato per signature verification

#### App native

**iOS, Loyalty Club** (SwiftUI, iOS 16+)
- Catalogo prodotti multi-brand
- Carrello con punti, gift card e promo
- Cinque flussi di ordine: Dine-in, Pickup, Delivery, Paga al Tavolo via QR, Eventi e Masterclass
- Mappa locali con clustering
- Esperienze gamificate e programma referral
- Pagamenti in-app con multi-PSP, tracking ordine, push

**Android, Loyalty Club** (Jetpack Compose, Android 8+)
- Parità feature con iOS, Material 3, Hilt
- Coroutines + Flow
- Stripe Terminal SDK per Tap-to-Pay sui device merchant

**Kiosk Android proprietario** (hardware Elo Pay 22)
- Firmware in-house per i kiosk in store, modalità kiosk 24/7
- Stripe Terminal SDK Tap-to-Pay nativo
- Self-update OTA via Cloud Storage
- MDM e VPN mesh per fleet management
- Menu dinamico e loyalty integrata
- Crash reporter e telemetria heartbeat su dashboard dedicata
- Mini-giochi durante l'attesa

#### Dashboard web

**CRM & Loyalty**
- CRM clienti loyalty
- Programma loyalty: punti, tier, regole flash, regole per prodotto, coupon, referral
- Codici studente con verifica dominio universitario e OTP

**Marketing & Engagement**
- Promo con QR batch, banner e push
- Esperienze gamificate
- Gift card con calcolo IVA automatico
- Eventi e masterclass

**Operations**
- Gestione locations con credenziali PSP per location
- Monitor flotta kiosk, release management e crash history
- Integrazione delivery
- Customer service e payments multi-PSP

**Insight**
- Social monitor competitor
- Analytics di vendita e loyalty

#### Integrazioni

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/Deliverect_Logo_Primary.svg/3840px-Deliverect_Logo_Primary.svg.png" height="28" alt="Deliverect"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/165162/1753464414-glovo-on-demand-deliverect-logo.svg" height="28" alt="Glovo OnDemand"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/133951/1720164277-group-1321316881.svg" height="24" alt="Satispay"/>&nbsp;&nbsp;&nbsp;
<img src="https://1000logos.net/wp-content/uploads/2021/05/Stripe-logo.png" height="28" alt="Stripe"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.simpleicons.org/revolut/000000" height="24" alt="Revolut"/>&nbsp;&nbsp;&nbsp;
<img src="https://voucherly.it/favicon.ico" height="24" alt="Voucherly"/>
</p>

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/Edenred.svg/250px-Edenred.svg.png" height="22" alt="Edenred"/>&nbsp;&nbsp;&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfarepellegrini_bianco.svg"/><img src="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfare-pellegrini_colori.svg" height="26" alt="Welfare Pellegrini"/></picture>&nbsp;&nbsp;&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Sodexo_logo.svg/250px-Sodexo_logo.svg.png" height="20" alt="Sodexo"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.day.it/Media/Images/hp/UP-Day-logo.png" height="26" alt="Up Day"/>
</p>

Deliverect · POS multi-tenant · Stripe (multi-tenant per location, calcolo IVA automatico) · Satispay · Voucherly (buoni pasto e carte di credito) · buoni pasto Edenred, Welfare Pellegrini, Sodexo e Up Day · Revolut Business · Glovo OnDemand · Wix · Firebase (Auth, FCM, Crashlytics) · Resend · monitor social via RSS · Slack · MDM · VPN mesh

#### Sicurezza

- JWT Firebase
- Admin API key con hashing SHA-256 in DB
- VPC privata
- Credenziali PSP per location separate
- Signature verification su ogni webhook
- Rate limiting, CORS allowlist, soft delete
- Sync provider auth e DB

#### Stack

<p>
<img src="https://img.shields.io/badge/Node.js-20-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/TypeScript-strict-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Fastify-ESM-000000?style=flat-square&logo=fastify&logoColor=white" alt="Fastify"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Redis-cache-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
<img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/SwiftUI-iOS_16+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/Jetpack_Compose-Android_8+-4285F4?style=flat-square&logo=android&logoColor=white" alt="Compose"/>
<img src="https://img.shields.io/badge/Stripe-Terminal_SDK-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
<img src="https://img.shields.io/badge/Cloud_Run-managed-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Run"/>
</p>

#### Ruolo

**Full-stack lead developer**. Architettura backend, webhook PSP, dashboard, app iOS, app Android e firmware kiosk Android end-to-end.

---

<a id="platform-one"></a>

### 5. Platform ONE

> **HR all-in-one multi-tenant per ristorazione e retail**

<p>
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/express/000000" height="22" alt="Express"/>&nbsp;
<img src="https://cdn.simpleicons.org/prisma/2D3748" height="22" alt="Prisma"/>&nbsp;
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/kotlin/7F52FF" height="22" alt="Kotlin"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>
</p>

#### Cosa risolve

Le aziende multi-sede della ristorazione e del retail gestiscono turni, presenze, ferie, buste paga, formazione, valutazioni e welfare su strumenti separati, spesso ancora su carta o WhatsApp. **Platform ONE** unifica tutto: turni, presenze, ferie, buste paga, formazione, performance review, welfare, gamification e comunicazione interna, sincronizzando in tempo reale web, iOS e Android.

#### Architettura

- **Backend** Node.js + Express + TypeScript su Google Cloud Run
- **Database** PostgreSQL gestito (Cloud SQL) con Prisma ORM
- **PgBouncer** in transaction mode per workload concorrente elevato
- **JWT** con refresh token e blacklist su logout
- **VPC privata** Cloud Run e database

#### Moduli

**Workforce Planning**
- Pianificazione turni con editor visuale settimanale, giornaliero e mensile
- Template, calcolo automatico ore contrattuali
- Workflow di approvazione a due livelli
- Vincoli automatici da CCNL
- Cambi turno peer-to-peer

**Time & Attendance**
- Timbrature mobile con un tap
- Modalità kiosk QR su iPad fisso
- Validazione GPS opzionale
- Riconciliazione turno pianificato vs ore effettive

**Leave Management**
- Ferie e ROL con calendario interattivo
- Saldi real-time in ore
- Workflow gerarchico e cancellazione automatica turni
- Regole di accrual configurabili

**Payroll & Expenses**
- Buste paga con upload massivo PDF e archivio sicuro
- Note spese con foto scontrino
- Calcolatore rimborsi km integrato con tabelle ACI e Google Maps Distance API

**Communication**
- Bacheca aziendale targettizzata
- Sistema notifiche unificato su tre canali: in-app, push, email
- Gestione documenti con alert di scadenza

**Training & Performance**
- Catalogo corsi video con percorsi per ruolo, quiz e attestati automatici
- Performance review con template configurabili e campagne periodiche
- **AI screening multi-provider** per sentiment, punti di forza, aree di miglioramento e red flag
- Link review pubblici per feedback da esterni senza login
- Feedback 360° con modalità anonima parziale o totale

**Onboarding & Org**
- Onboarding con template dinamici e form-builder drag and drop
- Organigramma interattivo drag and drop

**Wellbeing & Welfare**
- Gamification con HealthKit e Health Connect: XP, badge, classifiche
- Smart working con calendario di team
- Welfare e benefit self-service per ruolo

**Analytics**
- Costo del lavoro per store, brand e periodo

#### Multi-tenancy e ruoli

- Multi-tenancy nativa con isolamento logico per Company
- Gerarchia ruoli a sei livelli: Platform Admin, Super Admin, Area Manager, Store Manager, HQ, Employee
- Audit log completo e operazioni post-approvazione protette da PIN

#### Mobile native

- **iOS**: SwiftUI, HealthKit, Keychain, APNs e FCM
- **Android**: Kotlin, Jetpack Compose, Material 3, Hilt, Health Connect, CameraX (QR), FCM
- Parità feature con il web

#### Integrazioni

Firebase Auth (Google e Email, MFA opzionale) · Firebase Cloud Messaging · Firebase Storage · Resend · HealthKit e Health Connect · LLM multi-provider (AI screening review) · Google Maps Distance API · tabelle ACI rimborsi km

#### Sicurezza e compliance

- JWT con refresh e blacklist, bcrypt cost 12
- HTTPS ovunque, VPC privata, CORS allowlist
- Helmet con CSP, HSTS, X-Frame-Options
- Rate limiting su endpoint sensibili, audit log persistente
- PIN amministrativi, TLS in transito, encryption a riposo
- **GDPR compliant** con diritto all'oblio, export dati, audit accessi
- HealthKit e Health Connect solo con consenso esplicito

#### Stack

<p>
<img src="https://img.shields.io/badge/Node.js-Express-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/TypeScript-strict-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Prisma-ORM-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Swift-SwiftUI-orange?style=flat-square&logo=swift&logoColor=white" alt="Swift"/>
<img src="https://img.shields.io/badge/Kotlin-Compose-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin"/>
<img src="https://img.shields.io/badge/Firebase-Auth%20%C2%B7%20FCM%20%C2%B7%20Storage-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-purple?style=flat-square" alt="LLM"/>
</p>

#### Ruolo

**Full-stack lead developer**. Architettura multi-tenant, backend, frontend web, app iOS e Android, integrazione AI multi-provider, sistema notifiche unificato.

---

<a id="supplyone"></a>

### 6. SupplyONE

> **ERP cloud-native per food cost, magazzino e HACCP**

<p>
<img src="https://cdn.simpleicons.org/python/3776AB" height="22" alt="Python"/>&nbsp;
<img src="https://cdn.simpleicons.org/fastapi/009688" height="22" alt="FastAPI"/>&nbsp;
<img src="https://cdn.simpleicons.org/sqlalchemy/D71F00" height="22" alt="SQLAlchemy"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>&nbsp;
<img src="https://cdn.simpleicons.org/appstore/0D96F6" height="22" alt="App Store"/>
</p>

#### Cosa risolve

Un ristorante, o una catena, gestisce ogni giorno decine di flussi che senza un sistema unico vivono su carta, Excel e WhatsApp: ordini ai fornitori, DDT in arrivo con quantità e prezzi variabili, inventari multi-magazzino con costo medio ponderato, ricette con allergeni e food cost, controlli HACCP, scarti che incidono sul margine ma nessuno traccia davvero. **SupplyONE** mette tutto sotto un unico tetto, accessibile da tablet in cucina (iOS) e da desktop in ufficio (web), con la stessa fonte di verità sul DB.

#### Architettura

- **Backend** FastAPI (Python 3.10+) async su Google Cloud Run
- **SQLAlchemy 2.0** async, Alembic, Pydantic v2
- **Cloud SQL PostgreSQL** dietro PgBouncer in transaction pooling
- **VPC privata** backend e database
- **Web** vanilla (HTML + CSS + JavaScript) su Firebase Hosting
- **App iOS nativa** SwiftUI (iOS 16+) iPhone e iPad, **pubblicata su App Store**

#### Moduli

**Anagrafiche**
- Articoli con fornitori associati, prezzo storico, allegati
- Fornitori con condizioni, calendario consegne e SMTP per fornitore
- Gestione magazzini e sedi con permessi per utente
- Utenti con ruoli e scoping per magazzino

**Ordini e DDT**
- Ordini fornitori con creazione, invio email, template ricorrenti
- Suggerimenti automatici di riordino
- **DDT con OCR automatico** (Google Cloud Vision con fallback LLM multi-provider): foto del documento, auto-fill numero, data, quantità e prezzi per riga matchata
- Conferma DDT con riconciliazione quantità e prezzi e foto obbligatoria

**Magazzino**
- Inventario multi-warehouse con flusso bozza, conta, finalizzazione
- Costo medio ponderato automatico
- Movimenti: carico fornitore, scarico, trasferimento, rettifica
- Tracking sprechi con valorizzazione monetaria

**Ricette e Produzione**
- Ricette e menu con ingredienti, allergeni, food cost, margine
- Menu digitali pubblici
- Distinta base e semilavorati

**Compliance & HACCP**
- Controlli temperature e sanificazioni
- Scadenze lotti con logica FEFO

**Reporting**
- Dashboard KPI fatturato, ordini, scorte, alert scadenze, mappa punti vendita
- Analisi costi dettagliata per articolo, ricetta, periodo

**Periferiche**
- Driver per stampanti etichette industriali ZPL e EPL termici
- Attivazione device iOS via codice

#### App iOS nativa

L'app non è una versione ridotta del web: è uno strumento da **tablet in cucina** e **iPhone in magazzino**, ottimizzato per task rapidi e mani occupate. iPad usa `NavigationSplitView` con sidebar, iPhone usa `TabView` esteso.

- **Login senza password** con codice numerico generato dall'admin web. JWT lungo nel Keychain, un device alla volta per utente, revoca istantanea
- **Dashboard ricca** con header gradient, stat card animate, Apple Maps con pin punti vendita, meteo, alert scorte e scadenze, attività recenti, top selling
- **Selettore periodo** con Swift Charts (bar verticale spesa per bucket, bar orizzontale top fornitori, card Waste)
- **OCR DDT** al caricamento foto con auto-fill su righe matchate
- **Riordini suggeriti** con quantità editabili prima dell'invio
- **Template ordini ricorrenti** creabili da app
- **Conferma DDT** in parità feature con il web
- **Filtri condivisi** (sheet multi-select e range date) riusati su Ordini, DDT, Inventari, Movimenti, Sprechi

#### Lingue supportate

Italiano · Inglese · Spagnolo · Francese · Tedesco

#### Integrazioni

Google Cloud Vision (OCR DDT) · LLM multi-provider (fallback OCR semantico) · Google Cloud Storage (allegati per company) · Firebase Hosting e Auth · Acube (fatturazione elettronica SDI) · Freshdesk (ticketing) · Slack · n8n e Zapier (automazioni no-code) · Google Sheets API · OpenMeteo · Apple MapKit · POS · stampanti etichette industriali

#### Sicurezza e multi-tenant

- JWT Bearer firmati lato backend, bcrypt cost 12
- Scoping multi-tenant via header dedicato
- Ruoli a tre livelli e warehouse scoping per utente
- Device binding con revoca istantanea
- Rate limit sugli endpoint sensibili
- VPC privata
- API tokens server-to-server con lifetime dedicato
- Audit log e soft delete sui dati core

#### Stack

<p>
<img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/FastAPI-async-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
<img src="https://img.shields.io/badge/SQLAlchemy-2.0_async-D71F00?style=flat-square" alt="SQLAlchemy"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/SwiftUI-iOS_16+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/Google-Vision_OCR-4285F4?style=flat-square&logo=google&logoColor=white" alt="Vision"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-8E75B2?style=flat-square" alt="LLM"/>
<img src="https://img.shields.io/badge/App_Store-published-0D96F6?style=flat-square&logo=app-store&logoColor=white" alt="App Store"/>
</p>

#### Ruolo

**Full-stack lead developer**. Architettura backend, OCR pipeline (Vision e LLM), web vanilla i18n, app iOS nativa pubblicata su App Store, integrazioni e-invoicing, ticketing e automation.

---

<a id="onebooking"></a>

### 7. OneBooking

> **Gestione prenotazioni e sala per ristoranti**

<p>
<img src="https://cdn.simpleicons.org/nextdotjs/000000" height="22" alt="Next.js"/>&nbsp;
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/tailwindcss/38B2AC" height="22" alt="TailwindCSS"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

#### Cosa risolve

Una prenotazione non è una riga su un'agenda: occupa un tavolo per una fascia oraria, va confermata al cliente, arriva anche dai portali esterni, e quando la persona si siede la cassa deve saperlo prima della cucina. Se ogni sistema ne tiene una copia, due copie divergono e nessuno sa quale sia quella vera. **OneBooking** possiede le prenotazioni e le distribuisce: una sola griglia di disponibilità, che nessun altro sistema può contraddire.

#### Architettura

- **Web** Next.js con App Router, React e TailwindCSS su Firebase Hosting
- **Database** Cloud SQL PostgreSQL in schema dedicato, sullo stesso database del resto della suite
- **Contratto di lettura** viste versionate che i sistemi collegati interrogano senza toccare le tabelle
- **Contratto di scrittura** API firmata in HMAC, con identificativo di chiave in chiaro, nonce e marca temporale per ogni richiesta
- **Concorrenza** in isolamento Serializable, con il conflitto restituito come riprovabile e non come errore definitivo

#### Moduli

**Agenda e disponibilità**
- Griglia per servizio, con orari di apertura e chiusura per locale
- Aree e tavoli con posizione in planimetria, capienza minima e massima
- Chiusure del locale che fermano tutti i canali insieme

**Sala**
- Lista d'attesa e walk in: mettere a sedere crea una prenotazione vera, non una nota
- Stati della prenotazione fino al Seduto, con rilascio del tavolo alla chiusura del conto
- Accoppiamento dei tavoli con la cassa per identificativo e mai per etichetta, perché due tavoli possono chiamarsi allo stesso modo

**Clienti e canali**
- Sincronizzazione con TheFork
- Email di conferma e promemoria al cliente
- Registro delle modifiche per ogni prenotazione

**Multi-locale**
- Chiavi distinte per potere e per perimetro di locali
- Confronti fra locali e storico

#### Integrazioni

<p>
<img src="https://avatars.githubusercontent.com/lafourchette" height="30" alt="TheFork"/>
</p>

TheFork · K-POS (agenda in cassa, Seduto, rilascio del tavolo alla chiusura del conto) · portali di prenotazione online · email transazionali

#### Sicurezza

- Firma HMAC su ogni scrittura, con il segreto che non passa da nessuno schermo
- Chiavi separate per potere: scrivere una prenotazione e chiudere un locale non sono lo stesso permesso
- Perimetro di locali dichiarato per chiave
- Nessuna scrittura in SQL diretto: una prenotazione ha effetti collaterali che solo l'API conosce

#### Stack

<p>
<img src="https://img.shields.io/badge/Next.js-App_Router-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js"/>
<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Firebase-Hosting-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
<img src="https://img.shields.io/badge/API-HMAC_firmata-6E4C13?style=flat-square" alt="HMAC"/>
</p>

#### Ruolo

**Full-stack lead developer**. Backend prenotazioni, pannello web, contratto firmato verso i sistemi collegati e sincronizzazione con TheFork.

---

<a id="ticketos"></a>

### 8. TicketOS

> **Assistenza tecnica e manutenzione per reti di locali**

<p>
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/vite/646CFF" height="22" alt="Vite"/>&nbsp;
<img src="https://cdn.simpleicons.org/python/3776AB" height="22" alt="Python"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Slack_icon_2019.svg/120px-Slack_icon_2019.svg.png" height="22" alt="Slack"/>
</p>

#### Cosa risolve

Quando in un locale si rompe qualcosa, il guasto viaggia su WhatsApp, la foto si perde e nessuno sa da quanto tempo quel forno è fermo. **TicketOS** raccoglie le segnalazioni dei locali, le smista ai team e ai fornitori e misura quanto ci mette chi risolve. Chi apre una segnalazione dichiara cosa il locale non riesce più a fare, non quanto sia urgente: la priorità la deriva il sistema, perché in una scala dove tutto sta in cima non resta più nessun ordine.

#### Architettura

- **Web** React + Vite su Firebase Hosting, TanStack Query
- **Backend** Python con autenticazione macchina per i sistemi che si incorporano
- **Database** PostgreSQL in schema dedicato, sullo stesso database del resto della suite
- **Moduli dinamici** definiti sul server e disegnati dal client: cambiare un modulo non richiede il rilascio di un'app
- **API embed** con token a scadenza breve, tenuto in cache dal chiamante per non bruciare il limite di frequenza

#### Moduli

**Segnalazioni**
- Cinque stati, dove chiuso non vuol dire finito bene ma chiuso perché non si poteva risolvere
- Impatto dichiarato dal locale e priorità derivata dall'impatto
- Moduli dinamici per categoria, con dodici tipi di campo ammessi
- Allegati fino a dieci megabyte, venti per ticket, riletti con collegamenti firmati validi solo su quel ticket

**Smistamento**
- Team, agente assegnatario ed etichette
- Fornitori esterni e costo dell'intervento
- Manutenzione programmata

**Comunicazione**
- Messaggi pubblici sul ticket, con avviso all'assegnatario e all'autore
- Email al locale su apertura, cambio di stato e nuovo messaggio
- Annunci su Slack

**Misura**
- Cruscotto con tempi medi e ticket fuori tempo massimo
- Report per locale, categoria, team e fornitore

#### Integrazioni

K-POS (pagina Assistenza in cassa: si apre, si vede e si risponde dal banco) · Slack · email transazionali · API embed per gli altri sistemi del gruppo

#### Sicurezza

- Autenticazione macchina per i sistemi incorporati, con token a scadenza breve
- La chiave resta sul backend che si incorpora e non arriva mai su un apparecchio in sala
- Il locale è dichiarato due volte per strade indipendenti, dalla credenziale del chiamante e dal token: il giorno che non coincidessero è un difetto che si vede, non un accesso che passa
- Il locale apre, vede e modifica ma non chiude, perché la data di risoluzione alimenta la misura del lavoro di chi risolve
- Limite di frequenza per chiave, collegamenti agli allegati firmati e ristretti al singolo ticket

#### Stack

<p>
<img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Vite-bundler-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/>
<img src="https://img.shields.io/badge/Python-backend-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Firebase-Hosting%20%C2%B7%20Auth-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
<img src="https://img.shields.io/badge/TanStack-Query-FF4154?style=flat-square&logo=react-query&logoColor=white" alt="TanStack Query"/>
</p>

#### Ruolo

**Full-stack lead developer**. Gestionale web, backend, moduli dinamici, API embed per i sistemi del gruppo e integrazione con la cassa.

---

<a id="bite-radio"></a>

### 9. Bite Radio

> **La radio del gruppo Investfood, in onda 24 ore su 24**

<p>
<img src="https://cdn.simpleicons.org/html5/E34F26" height="22" alt="HTML5"/>&nbsp;
<img src="https://cdn.simpleicons.org/css/663399" height="22" alt="CSS"/>&nbsp;
<img src="https://cdn.simpleicons.org/javascript/F7DF1E" height="22" alt="JavaScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/nodedotjs/339933" height="22" alt="Node.js"/>&nbsp;
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

<p>
<img src="https://img.shields.io/badge/streaming-24%2F7-success?style=flat-square" alt="24/7"/>
<img src="https://img.shields.io/badge/palinsesto-6_fasce-blue?style=flat-square" alt="6 blocchi"/>
<img src="https://img.shields.io/badge/locali-7_sincronizzati-orange?style=flat-square" alt="7 locali"/>
<img src="https://img.shields.io/badge/curatela-umana-D97757?style=flat-square" alt="Curatela umana"/>
</p>

#### Cosa risolve

La musica in un locale non è un dettaglio di arredo: se copre le conversazioni la sala si svuota prima, se resta uguale dalla colazione alla cena il servizio perde il suo ritmo. Le playlist in loop e gli algoritmi da soli non risolvono nessuno dei due problemi. **Bite Radio** è un flusso unico e continuo, costruito sui momenti del servizio invece che sui gusti di chi lo mette.

#### Come funziona

- **Un solo flusso continuo**, 24 ore al giorno, 365 giorni all'anno: nessuna coda da gestire, nessun silenzio fra un brano e l'altro
- **Sei fasce di palinsesto** allineate ai momenti del servizio, dall'apertura alla notte
- **Curatela umana**: la selezione la fanno le persone, gli algoritmi aiutano solo a scoprire
- **Sincronizzazione fra i locali**: stesso brano nello stesso istante in tutti e sette i punti vendita

#### Architettura

- **Sito e player** pagine statiche in HTML, CSS e JavaScript scritti a mano, senza framework, con versione italiana e inglese separate e icone in sprite SVG
- **Backend** Node.js e TypeScript su Google Cloud Run, come il resto della suite
- **Database** Cloud SQL PostgreSQL per palinsesto, brani e programmazione oraria
- **Archivio audio** su Google Cloud Storage
- **Hosting** Firebase Hosting con distribuzione su CDN

#### Palinsesto

- **Bite Morning** 07:00 - 10:00
- **Poké Hour** 12:00 - 15:00
- **Wok & Roll** 15:00 - 18:00
- **Sushi Sunset** 18:00 - 21:00
- **Night Bite** 21:00 - 00:00
- **Silent Kitchen** 00:00 - 07:00

#### Mood musicali

Neo Soul · Lo-Fi House · Nu Disco · City Pop · Afro House · Indie Pop

#### Principio di selezione

Niente che copra le conversazioni, niente che spenga il servizio. Ogni brano entra in palinsesto solo se regge il livello di energia della sua fascia senza alzare la voce.

#### Stack

<p>
<img src="https://img.shields.io/badge/HTML5-static-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5"/>
<img src="https://img.shields.io/badge/CSS-hand_written-663399?style=flat-square&logo=css&logoColor=white" alt="CSS"/>
<img src="https://img.shields.io/badge/JavaScript-vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/>
<img src="https://img.shields.io/badge/Node.js-TypeScript-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Cloud_Run-managed-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Run"/>
<img src="https://img.shields.io/badge/Cloud_Storage-audio-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Storage"/>
<img src="https://img.shields.io/badge/Firebase-Hosting-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
</p>

#### Ruolo

**Full-stack lead developer**. Palinsesto, motore di trasmissione continua e sincronizzazione fra i locali.

---

<div align="center">

<a href="#indice--index"><b>Torna all'indice</b></a>

</div>

---

<a id="english"></a>

## English

<a id="investfood-tech-system-en"></a>

### InvestFood Tech System

> **The complete operating system for restaurants** · <a href="https://investfood.tech/"><b>investfood.tech</b></a>

Nine products, one single source of data. Each one works on its own, yet they all speak the same language: every receipt issued in K-POS becomes a number in AtomicBI, consumption flows down to SupplyONE, shifts close in Platform ONE. Five languages, multi-venue and multi-brand, role-based permissions, cross-venue comparisons. Built on the group's seven brands and tested in service every day.

---

> Nine complementary products designed and developed for **InvestFood SRL**. A cloud POS, an artificial intelligence platform, a multi-channel BI platform, a loyalty / ordering / kiosk platform, an all-in-one HR platform, a cloud-native ERP for food cost and inventory, reservation management, technical support and the group's radio station. Almost all in production, with native iOS, Android, Wear OS and web clients at feature parity.

---

<a id="k-pos-en"></a>

### 1. K-POS

> **Multi-company cloud POS for bars, restaurants and chains**

<p>
<img src="https://cdn.simpleicons.org/nestjs/E0234E" height="22" alt="NestJS"/>&nbsp;
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/prisma/2D3748" height="22" alt="Prisma"/>&nbsp;
<img src="https://cdn.simpleicons.org/nextdotjs/000000" height="22" alt="Next.js"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/kotlin/7F52FF" height="22" alt="Kotlin"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/redis/DC382D" height="22" alt="Redis"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

#### What it solves

A venue does not just print receipts: it sends orders to the kitchen printers, takes card payments on a terminal, issues fiscal documents and electronic invoices, and during the very same service receives orders from Glovo, Just Eat, Deliveroo, from the QR code on the table and from the digital menu. Taken one at a time, each of those flows has its own system and its own truth. **K-POS** keeps them all on the same one: a cloud backend, a web panel where you configure once for every venue, and a native iPad app that keeps working when the network drops.

#### Architecture

- **Backend** NestJS 10 on Express 5, strict TypeScript with no `any`, Prisma 6
- **Database** Cloud SQL PostgreSQL in a dedicated schema, behind PgBouncer in transaction pool, reached through the Cloud SQL connector with no public IP
- **Queues and cache** Redis with BullMQ for printing, channel sync and scheduled publishing
- **Web panel** Next.js 15 App Router, React 19, TailwindCSS, TanStack Query
- **Native iPad app** SwiftUI (iPadOS 16+) with a local GRDB database and an idempotent sync queue
- **K-Display** Android app for the customer-facing screen, **K-POS Sala** Wear OS app for the runners
- **Cloud Run** in EU region, structured logs and error tracking with Sentry

#### Modules

**Till and floor**
- Order taking for dine-in, takeaway and delivery, with a floor plan
- Split bills, table moves and merges, discounts, tips and change
- Kitchen orders on networked ESC/POS printers and a kitchen display (KDS)
- Calls to the floor wristband: dish ready, takeaway complete, table to clear
- Left-handed mode, dark theme, repositionable panels, four languages

**Fiscal**
- Commercial document on the networked fiscal printer, with refunds and voids
- Electronic invoicing over a direct SDICoop channel to the Italian Revenue Agency
- Invoice series, daily takings and an archive of every issued document
- Loyalty block printed at the foot of the pre-bill and of the fiscal receipt

**Catalogue and price lists**
- Categories, variants, build-your-own items, allergens and time-based product suspension
- Five price lists per channel and different names per menu, brand, venue and channel
- A menu saved in the panel reaches the till instantly, with nothing to republish

**Sales channels**
- In-house connectors for Glovo, Just Eat and Deliveroo, plus the Deliverect bridge
- Digital menu, Order at Table and Pay at Table from a QR code, with a bill that splits
- Menu publishing and store opening scheduled by time, weekday and timezone

**Payments**
- Satispay, SumUp, Stripe, Revolut, Nexi and VRP terminals, with per-venue credentials
- Face-value meal vouchers that by law give no change, refunds and reversals reconciled

**Platform**
- Multi-company with brands and venues, licensing and granular role permissions
- Devices activated by code and operator PIN, revocable in one tap
- Remote control plane to correct app behaviour without waiting for a release
- Audit log, offline sync and idempotent writes arbitrated by the database

#### Integrations

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/Deliverect_Logo_Primary.svg/3840px-Deliverect_Logo_Primary.svg.png" height="28" alt="Deliverect"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/165162/1753464414-glovo-on-demand-deliverect-logo.svg" height="26" alt="Glovo"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.simpleicons.org/deliveroo/00CCBC" height="24" alt="Deliveroo"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.simpleicons.org/justeat/FF8000" height="24" alt="Just Eat"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/133951/1720164277-group-1321316881.svg" height="24" alt="Satispay"/>&nbsp;&nbsp;&nbsp;
<img src="https://1000logos.net/wp-content/uploads/2021/05/Stripe-logo.png" height="28" alt="Stripe"/>&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/MultiSafepay/MultiSafepay-icons/master/methods/revolut%403x.png" height="24" alt="Revolut"/>&nbsp;&nbsp;&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Nexi_Logo.svg/250px-Nexi_Logo.svg.png" height="20" alt="Nexi"/>
</p>

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/Edenred.svg/250px-Edenred.svg.png" height="22" alt="Edenred"/>&nbsp;&nbsp;&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfarepellegrini_bianco.svg"/><img src="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfare-pellegrini_colori.svg" height="26" alt="Welfare Pellegrini"/></picture>&nbsp;&nbsp;&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Sodexo_logo.svg/250px-Sodexo_logo.svg.png" height="20" alt="Sodexo"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.day.it/Media/Images/hp/UP-Day-logo.png" height="26" alt="Up Day"/>
</p>

Glovo · Just Eat · Deliveroo · Deliverect · BiteOS (loyalty, Pay at Table, waiter suggestions) · Platform ONE (QR kiosk time tracking) · SupplyONE (stock levels at the till) · OneBooking (reservation diary) · TicketOS (support from the till) · Italian Revenue Agency (SDICoop) · Epson fiscal printers · networked ESC/POS printers · Satispay, SumUp, Stripe, Revolut, Nexi and VRP terminals · Edenred, Welfare Pellegrini, Sodexo and Up Day meal vouchers · Firebase (Auth, FCM) · Google Cloud Storage

#### Security

- Firebase JWT for people, a device credential for iPads, screens and watches
- Every route handler declares the permission it requires, and a CI script verifies that nobody forgets
- Multi-company isolation with a dedicated end to end suite for the tenancy perimeter
- Database with no public IP, secrets in Secret Manager, versioned integration keys
- Rate limiting, Helmet, CORS allowlist, persistent audit log
- Instant device revocation, idempotent writes, no till privileged over the others

#### Supported languages

Italian · English · French · German

#### Stack

<p>
<img src="https://img.shields.io/badge/NestJS-10-E0234E?style=flat-square&logo=nestjs&logoColor=white" alt="NestJS"/>
<img src="https://img.shields.io/badge/TypeScript-strict-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Prisma-6-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Redis-BullMQ-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
<img src="https://img.shields.io/badge/Next.js-15-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js"/>
<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/SwiftUI-iPadOS_16+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/GRDB-offline_first-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="GRDB"/>
<img src="https://img.shields.io/badge/Jetpack_Compose-Android%20%C2%B7%20Wear_OS-4285F4?style=flat-square&logo=android&logoColor=white" alt="Compose"/>
<img src="https://img.shields.io/badge/Cloud_Run-managed-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Run"/>
</p>

#### Role

**Full-stack lead developer**. Backend architecture, web panel, native iPad app, Android apps for the customer screen and the floor watches, delivery connectors, fiscal chain and electronic invoicing end-to-end.

---

<a id="investai-en"></a>

### 2. InvestAI

> **Artificial intelligence platform for food and beverage**

<p>
<img src="https://img.shields.io/badge/AI-demand_forecasting-8E75B2?style=flat-square" alt="Forecasting"/>
<img src="https://img.shields.io/badge/AI-conversational_assistant-D97757?style=flat-square" alt="Conversational"/>
<img src="https://img.shields.io/badge/licensing-white_label-4285F4?style=flat-square" alt="White label"/>
<img src="https://img.shields.io/badge/launch-2027-lightgrey?style=flat-square" alt="2027"/>
</p>

#### What it solves

The question a restaurant asks itself every day is always the same: how much is needed, where and when. Today the answer is intuition, and intuition errs in one direction only, towards waste. **InvestAI** turns that question into a measured forecast, and the forecast into an operational proposal: not a dashboard to interpret, but a supplier order already filled in, a shift already sized, a dish already flagged as at risk.

#### Three levels

- **Operational AI** for running the venue: forecasts, orders, shifts, waste
- **Conversational AI** facing the end customer directly
- **Licensed platform**, white-label, for chains outside the group

#### Modules

**Forecasting and procurement**
- Demand forecasting per venue, item and time slot, down to the thirty-minute delivery window
- A declared margin of error next to every forecast, because an estimate without uncertainty is not an estimate
- Supplier orders generated and aligned to the forecasts

**Margin and menu**
- Real-time food cost and margin, on actual prices
- Menu engineering crossing margin with popularity
- Waste reduction with at-risk items flagged before they expire

**People and customers**
- Staff scheduling based on expected footfall
- Conversational assistant for natural language ordering and allergen questions
- Personalisation and loyalty on each customer's own history

#### Training data

More than one hundred directly operated venues, seven Italian restaurant brands, roughly thirteen thousand customers a day. Not a model trained on purchased industry data, but on the real operations of the group that runs it.

#### Target users

Chains and franchises · delivery-first operators · suppliers and producers · travel retail and shopping centres

#### Status

In development, launch expected in 2027.

#### Role

**Full-stack lead developer**. Platform architecture, forecasting models, conversational assistant and integration with the group's operational systems.

---

<a id="atomicbi-en"></a>

### 3. AtomicBI

> **Multi-channel BI platform for multi-brand restaurant chains**

<p>
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/android/3DDC84" height="22" alt="Android"/>&nbsp;
<img src="https://cdn.simpleicons.org/python/3776AB" height="22" alt="Python"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

#### What it solves

A multi-brand food chain generates daily data that lives in silos: POS, delivery aggregators, HR systems, time tracking, warehouse ERP, multi-PSP payments, accounting. **AtomicBI** unifies everything into a single source of truth, a PostgreSQL data warehouse, exposed via API and consumed by three native clients (web, iOS, Android) with an extensive suite of functional modules.

#### Architecture

- **Web** React 19 + Vite 7 + TailwindCSS on Firebase Hosting
- **Native iOS** SwiftUI with MVVM architecture (iOS 15+)
- **Native Android** Jetpack Compose + Material 3
- **Backend** Cloud Functions Python 3.11 in EU region
- **Data warehouse** Cloud SQL PostgreSQL with PgBouncer in transaction pool
- **Real-time** Firestore listeners for RBAC, master data, alerts and push tokens

#### Modules

**Business Intelligence**
- Weekly and Monthly Business Review with historical trends, per-channel breakdown and YoY comparison
- Store Manager report with AOV, payment mix and time-bucket deep dives
- Multilingual Investor Relations (IT, EN, FR, DE) with YTD KPIs, EBITDA, headcount and data room
- Analytics for operational platforms (loyalty, HR, supply chain)

**Operations & Finance**
- Daily closure with canonical formulas, control checks and photo archive
- Automatic reconciliation of invoices, receipts and deposits
- Modules for deposits, foreign invoices and receipt anomalies
- Menu engineering with pricing suggestions

**AI & Automation**
- **AtomicAI Chat**, a conversational assistant over the data warehouse that cites the SQL queries it runs
- **AI Daily Digest** on Slack with food and QSR news
- Drag and drop Report Builder with formula editor and PDF, Excel, Word export

**User Experience**
- Push notifications with scheduling and template variables
- Per-user dynamic sidebar without redeploys

#### Integrations

POS system · delivery aggregator platforms (Deliveroo, Glovo, Uber Eats, JustEat, Deliverect) · Satispay · meal voucher providers · HR system · time-tracking system · warehouse ERP · Firebase (Auth, FCM, Storage) · LLM multi-provider · OpenMeteo · Gmail API · Slack webhooks · OpenStreetMap

#### Security

- Firebase JWT with granular RBAC (pages, store, department)
- Secret Manager and database with no public IP
- Enforced HTTPS and full audit trail
- Soft delete on sensitive data
- Auth provider and data store sync on user delete

#### Stack

<p>
<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Vite-7-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/>
<img src="https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind"/>
<img src="https://img.shields.io/badge/SwiftUI-iOS_15+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/Jetpack_Compose-Material_3-4285F4?style=flat-square&logo=android&logoColor=white" alt="Compose"/>
<img src="https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/PostgreSQL-15-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Google_Cloud-Functions%20%C2%B7%20SQL%20%C2%B7%20Firebase-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="GCP"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-D97757?style=flat-square" alt="LLM"/>
</p>

#### Role

**Full-stack lead developer**. End-to-end architecture, backend, web, iOS, Android, data pipeline and AI integration.

---

<a id="biteos-en"></a>

### 4. BiteOS

> **The operating system of multi-brand restaurants**

<p>
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/fastify/000000" height="22" alt="Fastify"/>&nbsp;
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/android/3DDC84" height="22" alt="Android"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/redis/DC382D" height="22" alt="Redis"/>&nbsp;
<img src="https://1000logos.net/wp-content/uploads/2021/05/Stripe-logo.png" height="22" alt="Stripe"/>
</p>

#### What it solves

Running multiple food brands across dozens of locations means orchestrating POS, kiosks, apps, online orders, third-party delivery, loyalty, promotions, gift cards, events and per-location multi-PSP payments. **BiteOS** makes all these systems talk to each other while keeping a single source of truth for customer, order and loyalty points.

#### Architecture

- **Backend** Fastify + TypeScript ESM on Google Cloud Run
- **PostgreSQL** Cloud SQL + PgBouncer in transaction pool
- **Redis** for caching of locations, menus and transactions
- **Private VPC** between backend and database with no public IP exposure
- **Isolated PSP webhooks** in dedicated sub-plugins with raw body parser for signature verification

#### Native apps

**iOS, Loyalty Club** (SwiftUI, iOS 16+)
- Multi-brand product catalogue
- Cart with points, gift cards and promotions
- Five ordering flows: Dine-in, Pickup, Delivery, Pay at Table via QR, Events and Masterclasses
- Store map with clustering
- Gamified experiences and referral program
- In-app multi-PSP payments, order tracking, push

**Android, Loyalty Club** (Jetpack Compose, Android 8+)
- Feature parity with iOS, Material 3, Hilt
- Coroutines + Flow
- Stripe Terminal SDK for Tap-to-Pay on merchant devices

**Proprietary Android Kiosk** (Elo Pay 22 hardware)
- In-house firmware for in-store kiosks, 24/7 kiosk mode
- Native Stripe Terminal Tap-to-Pay
- OTA self-update via Cloud Storage
- MDM and mesh VPN for fleet management
- Dynamic menu and integrated loyalty
- Crash reporter and heartbeat telemetry on a dedicated dashboard
- Waiting mini-games

#### Web dashboard

**CRM & Loyalty**
- Loyalty customer CRM
- Loyalty program: points, tiers, flash rules, per-product rules, coupons, referrals
- Student codes with university domain verification and OTP

**Marketing & Engagement**
- QR-batch promos, banners and push
- Gamified experiences
- Gift cards with automatic VAT calculation
- Events and masterclasses

**Operations**
- Location management with per-location PSP credentials
- Kiosk fleet monitoring, release management and crash history
- Delivery integration
- Customer service and multi-PSP payments

**Insight**
- Competitor social monitoring
- Sales and loyalty analytics

#### Integrations

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/Deliverect_Logo_Primary.svg/3840px-Deliverect_Logo_Primary.svg.png" height="28" alt="Deliverect"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/165162/1753464414-glovo-on-demand-deliverect-logo.svg" height="28" alt="Glovo OnDemand"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.datocms-assets.com/133951/1720164277-group-1321316881.svg" height="24" alt="Satispay"/>&nbsp;&nbsp;&nbsp;
<img src="https://1000logos.net/wp-content/uploads/2021/05/Stripe-logo.png" height="28" alt="Stripe"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.simpleicons.org/revolut/000000" height="24" alt="Revolut"/>&nbsp;&nbsp;&nbsp;
<img src="https://voucherly.it/favicon.ico" height="24" alt="Voucherly"/>
</p>

<p>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/Edenred.svg/250px-Edenred.svg.png" height="22" alt="Edenred"/>&nbsp;&nbsp;&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfarepellegrini_bianco.svg"/><img src="https://welfarepellegrini.it/wp-content/uploads/2025/08/logo-welfare-pellegrini_colori.svg" height="26" alt="Welfare Pellegrini"/></picture>&nbsp;&nbsp;&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Sodexo_logo.svg/250px-Sodexo_logo.svg.png" height="20" alt="Sodexo"/>&nbsp;&nbsp;&nbsp;
<img src="https://www.day.it/Media/Images/hp/UP-Day-logo.png" height="26" alt="Up Day"/>
</p>

Deliverect · multi-tenant POS · Stripe (multi-tenant per-location, automatic tax) · Satispay · Voucherly (meal voucher and credit card provider) · Edenred, Welfare Pellegrini, Sodexo and Up Day meal vouchers · Revolut Business · Glovo OnDemand · Wix · Firebase (Auth, FCM, Crashlytics) · Resend · social monitoring via RSS · Slack · MDM · mesh VPN

#### Security

- Firebase JWT
- Admin API keys with SHA-256 hashing in DB
- Private VPC
- Separate per-location PSP credentials
- Signature verification on every webhook
- Rate limiting, CORS allowlist, soft delete
- Auth provider and DB sync

#### Stack

<p>
<img src="https://img.shields.io/badge/Node.js-20-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/TypeScript-strict-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Fastify-ESM-000000?style=flat-square&logo=fastify&logoColor=white" alt="Fastify"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Redis-cache-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
<img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/SwiftUI-iOS_16+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/Jetpack_Compose-Android_8+-4285F4?style=flat-square&logo=android&logoColor=white" alt="Compose"/>
<img src="https://img.shields.io/badge/Stripe-Terminal_SDK-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
<img src="https://img.shields.io/badge/Cloud_Run-managed-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Run"/>
</p>

#### Role

**Full-stack lead developer**. End-to-end architecture across backend, PSP webhooks, dashboard, iOS app, Android app and Android kiosk firmware.

---

<a id="platform-one-en"></a>

### 5. Platform ONE

> **All-in-one multi-tenant HR for hospitality and retail**

<p>
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/express/000000" height="22" alt="Express"/>&nbsp;
<img src="https://cdn.simpleicons.org/prisma/2D3748" height="22" alt="Prisma"/>&nbsp;
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/kotlin/7F52FF" height="22" alt="Kotlin"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>
</p>

#### What it solves

Multi-site hospitality and retail companies manage shifts, attendance, leaves, payslips, training, evaluations and welfare on separate tools, often still on paper or WhatsApp. **Platform ONE** unifies all of it: shifts, attendance, leaves, payslips, training, performance reviews, welfare, gamification and internal communication, syncing in real time across web, iOS and Android.

#### Architecture

- **Backend** Node.js + Express + TypeScript on Google Cloud Run
- **Database** managed PostgreSQL (Cloud SQL) with Prisma ORM
- **PgBouncer** in transaction mode for high concurrent workloads
- **JWT** with refresh tokens and blacklist on logout
- **Private VPC** between Cloud Run and database

#### Modules

**Workforce Planning**
- Shift planning with weekly, daily and monthly visual editor
- Templates, automatic contractual-hours computation
- Two-level approval workflow
- Automatic CCNL constraints
- Peer-to-peer shift swaps

**Time & Attendance**
- Mobile attendance with one-tap clock-in
- QR kiosk mode on dedicated iPads
- Optional GPS validation
- Planned vs actual reconciliation

**Leave Management**
- Holidays and leave with interactive calendar
- Real-time hourly balances
- Hierarchical workflow with automatic shift cancellation
- Configurable accrual rules

**Payroll & Expenses**
- Payslips with bulk PDF upload and secure archive
- Expenses with receipt photo
- Mileage reimbursement calculator integrated with ACI tables and Google Maps Distance API

**Communication**
- Targeted company board
- Unified notifications across three channels: in-app, push, email
- Document management with expiry alerts

**Training & Performance**
- Video course catalogue with role-based paths, quizzes and automatic certificates
- Performance reviews with configurable templates and periodic campaigns
- **Multi-provider AI screening** for sentiment, strengths, areas for improvement and red flags
- Public review links for external feedback without login
- 360° feedback with partial or full anonymity

**Onboarding & Org**
- Onboarding with dynamic templates and drag-and-drop form builder
- Interactive drag-and-drop org chart

**Wellbeing & Welfare**
- Gamification via HealthKit and Health Connect: XP, badges, leaderboards
- Smart working with team calendar
- Self-service welfare and benefits per role

**Analytics**
- Labour cost by store, brand and period

#### Multi-tenancy and roles

- Native multi-tenancy with logical isolation per Company
- Six-tier role hierarchy: Platform Admin, Super Admin, Area Manager, Store Manager, HQ, Employee
- Full audit log and PIN-protected post-approval operations

#### Native mobile

- **iOS**: SwiftUI, HealthKit, Keychain, APNs and FCM
- **Android**: Kotlin, Jetpack Compose, Material 3, Hilt, Health Connect, CameraX (QR), FCM
- Feature parity with the web

#### Integrations

Firebase Auth (Google and Email, optional MFA) · Firebase Cloud Messaging · Firebase Storage · Resend · HealthKit and Health Connect · LLM multi-provider (AI review screening) · Google Maps Distance API · ACI mileage rates

#### Security and compliance

- JWT with refresh and blacklist, bcrypt cost 12
- HTTPS everywhere, private VPC, CORS allowlist
- Helmet with CSP, HSTS, X-Frame-Options
- Rate limiting on sensitive endpoints, persistent audit log
- Admin PINs, TLS in transit, encryption at rest
- **GDPR compliant** with right to be forgotten, data export, access audit
- HealthKit and Health Connect only with explicit consent

#### Stack

<p>
<img src="https://img.shields.io/badge/Node.js-Express-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/TypeScript-strict-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Prisma-ORM-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Swift-SwiftUI-orange?style=flat-square&logo=swift&logoColor=white" alt="Swift"/>
<img src="https://img.shields.io/badge/Kotlin-Compose-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin"/>
<img src="https://img.shields.io/badge/Firebase-Auth%20%C2%B7%20FCM%20%C2%B7%20Storage-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-purple?style=flat-square" alt="LLM"/>
</p>

#### Role

**Full-stack lead developer**. Multi-tenant architecture, backend, web frontend, iOS and Android apps, multi-provider AI integration, unified notification system.

---

<a id="supplyone-en"></a>

### 6. SupplyONE

> **Cloud-native ERP for food cost, inventory and HACCP**

<p>
<img src="https://cdn.simpleicons.org/python/3776AB" height="22" alt="Python"/>&nbsp;
<img src="https://cdn.simpleicons.org/fastapi/009688" height="22" alt="FastAPI"/>&nbsp;
<img src="https://cdn.simpleicons.org/sqlalchemy/D71F00" height="22" alt="SQLAlchemy"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/swift/F05138" height="22" alt="Swift"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>&nbsp;
<img src="https://cdn.simpleicons.org/appstore/0D96F6" height="22" alt="App Store"/>
</p>

#### What it solves

A restaurant, or a chain, handles dozens of daily flows that, without a unified system, live on paper, Excel and WhatsApp: supplier orders, incoming delivery notes with shifting quantities and prices, multi-warehouse inventories with weighted-average cost, recipes with allergens and food cost, HACCP controls, waste that impacts margin but nobody really tracks. **SupplyONE** brings everything under one roof, accessible from kitchen tablets (iOS) and office desktops (web), with the same source of truth in the DB.

#### Architecture

- **Backend** FastAPI (Python 3.10+) async on Google Cloud Run
- **SQLAlchemy 2.0** async, Alembic, Pydantic v2
- **Cloud SQL PostgreSQL** behind PgBouncer in transaction pooling
- **Private VPC** between backend and database
- **Web** vanilla (HTML + CSS + JavaScript) on Firebase Hosting
- **Native iOS app** SwiftUI (iOS 16+) iPhone and iPad, **published on the App Store**

#### Modules

**Master data**
- Items with linked suppliers, price history, attachments
- Suppliers with terms, delivery calendar and per-supplier SMTP
- Warehouse and site management with per-user permissions
- Users with roles and per-warehouse scoping

**Orders & Delivery Notes**
- Supplier orders with creation, email send, recurring templates
- Automatic reorder suggestions
- **Delivery notes with automatic OCR** (Google Cloud Vision with LLM multi-provider fallback): photo of the document, auto-fill of number, date, quantities and prices per matched item-code line
- Delivery-note confirmation with quantity and price reconciliation and mandatory photo

**Inventory**
- Multi-warehouse inventory with draft, count, finalisation flow
- Automatic weighted-average cost
- Movements: supplier receipt, withdrawal, transfer, adjustment
- Waste tracking with monetary valuation

**Recipes & Production**
- Recipes and menus with ingredients, allergens, food cost, margin
- Public digital menus
- BOM and semi-finished products

**Compliance & HACCP**
- Temperature and sanitisation controls
- Lot expiry with FEFO logic

**Reporting**
- Dashboard with revenue, orders and stock KPIs, expiry alerts, store map
- Detailed cost analysis per item, recipe, period

**Peripherals**
- Drivers for industrial label printers ZPL and EPL thermal
- iOS device activation by code

#### Native iOS app

The app is not a reduced version of the web: it is a tool for **kitchen tablets** and **warehouse iPhones**, optimised for quick tasks and hands-busy contexts. iPad uses `NavigationSplitView` with sidebar, iPhone uses an extended `TabView`.

- **Passwordless login** with an admin-generated numeric code. Long-lived JWT in Keychain, one device per user at a time, instant revocation
- **Rich dashboard** with gradient header, animated stat cards, Apple Maps with store pins, weather, stock and expiry alerts, recent activity, top selling
- **Period selector** with Swift Charts (vertical-bar spend per bucket, horizontal-bar top suppliers, Waste card)
- **OCR on delivery-note upload** with auto-fill on matched lines
- **Suggested reorders** with editable quantities before sending
- **Recurring order templates** creatable from the app
- **Delivery-note confirmation** at feature parity with web
- **Shared filters** (multi-select sheet and date range) reused across Orders, Delivery Notes, Inventories, Movements, Waste

#### Supported languages

Italian · English · Spanish · French · German

#### Integrations

Google Cloud Vision (delivery-note OCR) · LLM multi-provider (semantic OCR fallback) · Google Cloud Storage (per-company attachments) · Firebase Hosting and Auth · Acube (electronic invoicing SDI) · Freshdesk (ticketing) · Slack · n8n and Zapier (no-code automation) · Google Sheets API · OpenMeteo · Apple MapKit · POS · industrial label printers

#### Security and multi-tenant

- Backend-signed JWT Bearer tokens, bcrypt cost 12
- Multi-tenant scoping via dedicated header
- Three-tier roles and per-user warehouse scoping
- Device binding with instant revocation
- Rate limiting on sensitive endpoints
- Private VPC
- Server-to-server API tokens with dedicated lifetime
- Audit log and soft delete on core data

#### Stack

<p>
<img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/FastAPI-async-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
<img src="https://img.shields.io/badge/SQLAlchemy-2.0_async-D71F00?style=flat-square" alt="SQLAlchemy"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/SwiftUI-iOS_16+-orange?style=flat-square&logo=swift&logoColor=white" alt="SwiftUI"/>
<img src="https://img.shields.io/badge/Google-Vision_OCR-4285F4?style=flat-square&logo=google&logoColor=white" alt="Vision"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-8E75B2?style=flat-square" alt="LLM"/>
<img src="https://img.shields.io/badge/App_Store-published-0D96F6?style=flat-square&logo=app-store&logoColor=white" alt="App Store"/>
</p>

#### Role

**Full-stack lead developer**. Backend architecture, OCR pipeline (Vision and LLM), vanilla i18n web, native iOS app published on the App Store, e-invoicing, ticketing and automation integrations.

---

<a id="onebooking-en"></a>

### 7. OneBooking

> **Reservation and front-of-house management for restaurants**

<p>
<img src="https://cdn.simpleicons.org/nextdotjs/000000" height="22" alt="Next.js"/>&nbsp;
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/tailwindcss/38B2AC" height="22" alt="TailwindCSS"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

#### What it solves

A reservation is not a line in a diary: it holds a table for a time slot, it has to be confirmed to the guest, it also arrives from external portals, and the moment the guest sits down the till must know before the kitchen does. If every system keeps a copy, two copies drift apart and nobody knows which one is true. **OneBooking** owns the reservations and distributes them: one availability grid, which no other system is allowed to contradict.

#### Architecture

- **Web** Next.js with App Router, React and TailwindCSS on Firebase Hosting
- **Database** Cloud SQL PostgreSQL in a dedicated schema, on the same database as the rest of the suite
- **Read contract** versioned views that connected systems query without ever touching the tables
- **Write contract** HMAC-signed API, with a clear-text key id, a nonce and a timestamp on every request
- **Concurrency** under Serializable isolation, with the conflict returned as retryable rather than as a final error

#### Modules

**Diary and availability**
- Per-service grid, with opening and closing hours per venue
- Areas and tables with floor-plan positions, minimum and maximum party size
- Venue closures that stop every channel at once

**Front of house**
- Waiting list and walk-ins: seating someone creates a real reservation, not a note
- Reservation states through to Seated, with the table released when the bill is closed
- Tables paired with the till by identifier and never by label, because two tables can share a name

**Guests and channels**
- Synchronisation with TheFork
- Confirmation and reminder emails to the guest
- A change log on every reservation

**Multi-venue**
- Keys separated by power and by venue perimeter
- Cross-venue comparisons and history

#### Integrations

<p>
<img src="https://avatars.githubusercontent.com/lafourchette" height="30" alt="TheFork"/>
</p>

TheFork · K-POS (diary at the till, Seated, table released when the bill closes) · online booking portals · transactional email

#### Security

- HMAC signature on every write, with the secret never passing through any screen
- Keys separated by power: writing a reservation and closing a venue are not the same permission
- Venue perimeter declared per key
- No direct SQL writes: a reservation has side effects only the API knows about

#### Stack

<p>
<img src="https://img.shields.io/badge/Next.js-App_Router-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js"/>
<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Firebase-Hosting-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
<img src="https://img.shields.io/badge/API-HMAC_signed-6E4C13?style=flat-square" alt="HMAC"/>
</p>

#### Role

**Full-stack lead developer**. Reservation backend, web panel, signed contract towards connected systems and TheFork synchronisation.

---

<a id="ticketos-en"></a>

### 8. TicketOS

> **Technical support and maintenance for venue networks**

<p>
<img src="https://cdn.simpleicons.org/react/61DAFB" height="22" alt="React"/>&nbsp;
<img src="https://cdn.simpleicons.org/vite/646CFF" height="22" alt="Vite"/>&nbsp;
<img src="https://cdn.simpleicons.org/python/3776AB" height="22" alt="Python"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Slack_icon_2019.svg/120px-Slack_icon_2019.svg.png" height="22" alt="Slack"/>
</p>

#### What it solves

When something breaks in a venue, the fault travels over WhatsApp, the photo gets lost and nobody knows how long that oven has been down. **TicketOS** collects what venues report, routes it to teams and suppliers, and measures how long the people who fix things actually take. Whoever opens a ticket declares what the venue can no longer do, not how urgent they feel it is: the priority is derived by the system, because on a scale where everything sits at the top there is no order left.

#### Architecture

- **Web** React + Vite on Firebase Hosting, TanStack Query
- **Backend** Python with machine authentication for the systems that embed it
- **Database** PostgreSQL in a dedicated schema, on the same database as the rest of the suite
- **Dynamic forms** defined server side and drawn by the client: changing a form does not require an app release
- **Embed API** with short-lived tokens, cached by the caller so the rate limit is not burnt

#### Modules

**Tickets**
- Five states, where closed does not mean finished well but closed because it could not be solved
- Impact declared by the venue, priority derived from the impact
- Dynamic forms per category, with twelve allowed field types
- Attachments up to ten megabytes, twenty per ticket, read back through signed links valid only on that ticket

**Routing**
- Teams, assigned agent and labels
- External suppliers and cost of the intervention
- Scheduled maintenance

**Communication**
- Public messages on the ticket, notifying the assignee and the author
- Email to the venue on opening, state change and new message
- Slack announcements

**Measurement**
- Dashboard with average times and overdue tickets
- Reports per venue, category, team and supplier

#### Integrations

K-POS (Support page at the till: open, follow and reply from the counter) · Slack · transactional email · embed API for the other systems in the group

#### Security

- Machine authentication for embedding systems, with short-lived tokens
- The key stays on the embedding backend and never reaches a device on the floor
- The venue is declared twice along independent paths, by the caller's credential and by the token: the day the two disagree is a visible defect, not an access that goes through
- The venue opens, follows and edits but never closes, because the resolution date feeds the measurement of the people who fix things
- Per-key rate limiting, attachment links signed and restricted to a single ticket

#### Stack

<p>
<img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Vite-bundler-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/>
<img src="https://img.shields.io/badge/Python-backend-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Firebase-Hosting%20%C2%B7%20Auth-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
<img src="https://img.shields.io/badge/TanStack-Query-FF4154?style=flat-square&logo=react-query&logoColor=white" alt="TanStack Query"/>
</p>

#### Role

**Full-stack lead developer**. Web application, backend, dynamic forms, embed API for the group's systems and integration with the POS.

---

<a id="bite-radio-en"></a>

### 9. Bite Radio

> **The Investfood group's radio station, on air 24 hours a day**

<p>
<img src="https://cdn.simpleicons.org/html5/E34F26" height="22" alt="HTML5"/>&nbsp;
<img src="https://cdn.simpleicons.org/css/663399" height="22" alt="CSS"/>&nbsp;
<img src="https://cdn.simpleicons.org/javascript/F7DF1E" height="22" alt="JavaScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/nodedotjs/339933" height="22" alt="Node.js"/>&nbsp;
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="22" alt="TypeScript"/>&nbsp;
<img src="https://cdn.simpleicons.org/postgresql/336791" height="22" alt="PostgreSQL"/>&nbsp;
<img src="https://cdn.simpleicons.org/firebase/FFCA28" height="22" alt="Firebase"/>&nbsp;
<img src="https://cdn.simpleicons.org/googlecloud/4285F4" height="22" alt="Google Cloud"/>
</p>

<p>
<img src="https://img.shields.io/badge/streaming-24%2F7-success?style=flat-square" alt="24/7"/>
<img src="https://img.shields.io/badge/schedule-6_blocks-blue?style=flat-square" alt="6 blocks"/>
<img src="https://img.shields.io/badge/venues-7_in_sync-orange?style=flat-square" alt="7 venues"/>
<img src="https://img.shields.io/badge/curation-human-D97757?style=flat-square" alt="Human curation"/>
</p>

#### What it solves

Music in a venue is not a decorating detail: if it covers conversations the room empties earlier, and if it stays the same from breakfast to dinner the service loses its rhythm. Looping playlists and algorithms on their own solve neither problem. **Bite Radio** is a single continuous stream, built around the moments of service rather than around the taste of whoever pressed play.

#### How it works

- **One continuous stream**, 24 hours a day, 365 days a year: no queue to manage, no silence between tracks
- **Six programming blocks** aligned to the moments of service, from opening to late night
- **Human curation**: people pick the selection, algorithms only help with discovery
- **Synchronised across venues**: the same track at the same instant in all seven locations

#### Architecture

- **Site and player** static pages in hand-written HTML, CSS and JavaScript, no framework, with separate Italian and English versions and SVG sprite icons
- **Backend** Node.js and TypeScript on Google Cloud Run, like the rest of the suite
- **Database** Cloud SQL PostgreSQL for the schedule, the tracks and the hourly programming
- **Audio archive** on Google Cloud Storage
- **Hosting** Firebase Hosting with CDN distribution

#### Schedule

- **Bite Morning** 07:00 - 10:00
- **Poké Hour** 12:00 - 15:00
- **Wok & Roll** 15:00 - 18:00
- **Sushi Sunset** 18:00 - 21:00
- **Night Bite** 21:00 - 00:00
- **Silent Kitchen** 00:00 - 07:00

#### Musical moods

Neo Soul · Lo-Fi House · Nu Disco · City Pop · Afro House · Indie Pop

#### Selection principle

Nothing that covers conversations, nothing that dampens service. A track enters the schedule only if it holds the energy level of its block without raising its voice.

#### Stack

<p>
<img src="https://img.shields.io/badge/HTML5-static-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5"/>
<img src="https://img.shields.io/badge/CSS-hand_written-663399?style=flat-square&logo=css&logoColor=white" alt="CSS"/>
<img src="https://img.shields.io/badge/JavaScript-vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/>
<img src="https://img.shields.io/badge/Node.js-TypeScript-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/PostgreSQL-Cloud_SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Cloud_Run-managed-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Run"/>
<img src="https://img.shields.io/badge/Cloud_Storage-audio-4285F4?style=flat-square&logo=google-cloud&logoColor=white" alt="Cloud Storage"/>
<img src="https://img.shields.io/badge/Firebase-Hosting-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
</p>

#### Role

**Full-stack lead developer**. Programming schedule, continuous broadcast engine and synchronisation across venues.

---

<div align="center">

<a href="#indice--index"><b>Back to index</b></a>

</div>
