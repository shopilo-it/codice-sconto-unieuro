# Codice sconto Unieuro, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Unieuro** da [shopilo.it](https://shopilo.it/negozi/unieuro.it). Restituisce **coupon Unieuro** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-unieuro](https://shopilo-it.github.io/codice-sconto-unieuro/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-unieuro
cd codice-sconto-unieuro
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Unieuro",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su prodotti selezionati",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/unieuro.it"
  }
]
```

## Coupon Unieuro disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su prodotti selezionati | [shopilo.it](https://shopilo.it/negozi/unieuro.it) |

Codici attivi: **[shopilo.it/negozi/unieuro.it](https://shopilo.it/negozi/unieuro.it)**

## Domande frequenti

### Come utilizzo un codice sconto Unieuro?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/unieuro.it), aggiungi i prodotti al carrello su Unieuro e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Unieuro?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Unieuro piu recenti?
La pagina [shopilo.it/negozi/unieuro.it](https://shopilo.it/negozi/unieuro.it) viene aggiornata quotidianamente con i codici sconto Unieuro, voucher Unieuro e coupon promozionali Unieuro piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Unieuro

Unieuro e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/unieuro.it) trovi i migliori codici sconto Unieuro, coupon Unieuro verificati e voucher Unieuro attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-unieuro
```

```javascript
const { fetchCoupons } = require('codice-sconto-unieuro');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
