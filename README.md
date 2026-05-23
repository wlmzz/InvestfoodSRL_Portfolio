<div align="center">

<a href="https://investfood.it"><img src="https://static.wixstatic.com/media/cb2700_2b9dbe5db69f4506b8e416bcf20269f6~mv2.png" height="60" alt="Invest Food"/></a>

# Engineering Portfolio

**Full-stack engineering across web, mobile, backend, data and AI for a multi-brand food group**

<p>
<img src="https://img.shields.io/badge/status-in_production-success?style=flat-square" alt="status"/>
<img src="https://img.shields.io/badge/platforms-web%20%C2%B7%20iOS%20%C2%B7%20Android%20%C2%B7%20Kiosk-blue?style=flat-square" alt="platforms"/>
<img src="https://img.shields.io/badge/cloud-Google_Cloud%20%C2%B7%20Firebase-orange?style=flat-square" alt="cloud"/>
<img src="https://img.shields.io/badge/AI-LLM_multi--provider-purple?style=flat-square" alt="AI"/>
<img src="https://img.shields.io/badge/lang-IT%20%C2%B7%20EN-lightgrey?style=flat-square" alt="lang"/>
</p>

<p>
<a href="#italiano"><b>Italiano</b></a> · <a href="#english"><b>English</b></a>
</p>

</div>

---

## Indice / Index

> **Italiano**
>
> 1. [AtomicBI](#atomicbi) · piattaforma BI multi-canale per la ristorazione multi-brand
> 2. [BiteOS](#biteos) · sistema operativo della ristorazione (loyalty, ordini, pagamenti, kiosk)
> 3. [Platform ONE](#platform-one) · HR all-in-one multi-tenant per ristorazione e retail
> 4. [SupplyONE](#supplyone) · ERP cloud-native per food cost, magazzino e HACCP
>
> **English**
>
> 1. [AtomicBI](#atomicbi-en) · multi-channel BI platform for multi-brand restaurant chains
> 2. [BiteOS](#biteos-en) · the operating system of restaurants (loyalty, ordering, payments, kiosk)
> 3. [Platform ONE](#platform-one-en) · all-in-one multi-tenant HR for hospitality and retail
> 4. [SupplyONE](#supplyone-en) · cloud-native ERP for food cost, inventory and HACCP

---

<a id="italiano"></a>

## Italiano

> Quattro prodotti complementari progettati e sviluppati per **InvestFood SRL**. Una piattaforma BI multi-canale, una piattaforma di loyalty / ordini / kiosk per ristoranti, una piattaforma HR all-in-one e un ERP cloud-native per food cost e magazzino. Tutti in produzione, tutti con client nativi iOS, Android e web in parità feature.

---

<a id="atomicbi"></a>

### 1. AtomicBI

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

### 2. BiteOS

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

Deliverect · POS multi-tenant · Stripe (multi-tenant per location, calcolo IVA automatico) · Satispay · Voucherly (buoni pasto e carte di credito) · Revolut Business · Glovo OnDemand · Wix · Firebase (Auth, FCM, Crashlytics) · Resend · monitor social via RSS · Slack · MDM · VPN mesh

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

### 3. Platform ONE

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

### 4. SupplyONE

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

<div align="center">

<a href="#indice--index"><b>Torna all'indice</b></a>

</div>

---

<a id="english"></a>

## English

> Four complementary products designed and developed for **InvestFood SRL**. A multi-channel BI platform, a loyalty / ordering / kiosk platform for restaurants, an all-in-one HR platform, and a cloud-native ERP for food cost and inventory. All in production, all with native iOS, Android and web clients at feature parity.

---

<a id="atomicbi-en"></a>

### 1. AtomicBI

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

### 2. BiteOS

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

Deliverect · multi-tenant POS · Stripe (multi-tenant per-location, automatic tax) · Satispay · Voucherly (meal voucher and credit card provider) · Revolut Business · Glovo OnDemand · Wix · Firebase (Auth, FCM, Crashlytics) · Resend · social monitoring via RSS · Slack · MDM · mesh VPN

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

### 3. Platform ONE

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

### 4. SupplyONE

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

<div align="center">

<a href="#indice--index"><b>Back to index</b></a>

</div>
