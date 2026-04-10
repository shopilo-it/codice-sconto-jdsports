# Codice sconto JD Sports, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto JD Sports** da [shopilo.it](https://shopilo.it/negozi/jdsports.it). Restituisce **coupon JD Sports** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-jdsports](https://shopilo-it.github.io/codice-sconto-jdsports/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-jdsports
cd codice-sconto-jdsports
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "JD Sports",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su scarpe sportive",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/jdsports.it"
  }
]
```

## Coupon JD Sports disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su scarpe sportive | [shopilo.it](https://shopilo.it/negozi/jdsports.it) |

Codici attivi: **[shopilo.it/negozi/jdsports.it](https://shopilo.it/negozi/jdsports.it)**

## Domande frequenti

### Come utilizzo un codice sconto JD Sports?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/jdsports.it), aggiungi i prodotti al carrello su JD Sports e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon JD Sports?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher JD Sports piu recenti?
La pagina [shopilo.it/negozi/jdsports.it](https://shopilo.it/negozi/jdsports.it) viene aggiornata quotidianamente con i codici sconto JD Sports, voucher JD Sports e coupon promozionali JD Sports piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su JD Sports

JD Sports e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/jdsports.it) trovi i migliori codici sconto JD Sports, coupon JD Sports verificati e voucher JD Sports attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-jdsports
```

```javascript
const { fetchCoupons } = require('codice-sconto-jdsports');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
