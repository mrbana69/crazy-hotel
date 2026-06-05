# 🏨 Crazy Hotel

Sito web di presentazione e prenotazione per il **Crazy Hotel** — un B&B immaginario con un tocco di follia.

🔗 **[mrbana69.github.io/crazy-hotel](https://mrbana69.github.io/crazy-hotel)**

---

## Di cosa si tratta

Crazy Hotel è un sito statico a due pagine che simula il sito ufficiale di un hotel. La homepage presenta la struttura con un video in background, mostra le camere disponibili e le recensioni degli ospiti. Da lì, un pulsante porta alla pagina di prenotazione, dove l'utente compila un modulo, sceglie la camera e il metodo di pagamento, e il sito calcola automaticamente il prezzo totale in base ai giorni di soggiorno.

Il progetto è un esercizio scolastico di sviluppo web front-end: niente backend, niente database — tutto gira nel browser.

---

## Le pagine

**`index.html` — Homepage**

La landing page del Crazy Hotel. Un video in autoplay fa da sfondo all'intestazione di benvenuto. Scorrendo si trovano le due tipologie di camere (ognuna con il suo video), poi le recensioni di quattro ospiti con foto e commento. In fondo il footer con i contatti dell'hotel. Il pulsante "Prenota Ora" rimanda alla pagina di prenotazione.

**`prenotazione.html` — Modulo di prenotazione**

Il cuore funzionale del progetto. L'utente inserisce:

- Nominativo e email
- Tipo di camera: Base (70€/notte) o Comfort (120€/notte)
- Date di check-in e check-out
- Metodo di pagamento: Carta di credito, PayPal o Altro

Il JavaScript calcola automaticamente il numero di notti e il totale, valida i campi e reindirizza alla pagina di pagamento corrispondente al metodo scelto (tre pagine separate in `assets/html/`). I dati vengono passati tra le pagine tramite `localStorage`.

---

## Struttura del progetto

```
crazy-hotel/
├── index.html              # Homepage
├── prenotazione.html       # Modulo di prenotazione
├── leggimi_fra.txt         # Istruzioni (da leggere)
└── assets/
    ├── css/
    │   ├── style_home.css  # Stile homepage
    │   └── style.css       # Stile pagina prenotazione
    ├── foto/               # Logo e foto recensioni (maria, luca, anna, marco)
    ├── video/              # Video homepage e camere
    └── html/
        ├── pagamento_carta.html
        ├── pagamento_paypal.html
        └── pagamento_altro.html
```

---

## Tecnologie usate

HTML, CSS e JavaScript vanilla. Font Roboto via Google Fonts. Nessuna libreria esterna, nessun framework.

---

## Come aprirlo

Il modo migliore è usare il **Live Server** di VS Code aperto su `index.html` — i video non si caricano aprendo il file direttamente nel browser per via delle restrizioni CORS sui file locali.

In alternativa, la versione live è già disponibile su GitHub Pages:

👉 [https://mrbana69.github.io/crazy-hotel](https://mrbana69.github.io/crazy-hotel)

> *"sta volta non ho messo un nome inappropriato ehh!"*
> — `leggimi_fra.txt`
