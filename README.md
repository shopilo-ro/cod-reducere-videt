# Cod reducere Videt — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Videt** de pe [shopilo.ro](https://shopilo.ro/magazin/videt.ro). Returneaza **cupoane Videt** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-videt](https://shopilo-ro.github.io/cod-reducere-videt/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-videt
cd cod-reducere-videt
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Videt",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la sisteme de supraveghere",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/videt.ro"
  }
]
```

## Cupoane Videt disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la sisteme de supraveghere | [shopilo.ro](https://shopilo.ro/magazin/videt.ro) |

Codurile active: **[shopilo.ro/magazin/videt.ro](https://shopilo.ro/magazin/videt.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Videt?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/videt.ro), adauga produsele in cos pe Videt, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Videt?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Videt?
Pagina [shopilo.ro/magazin/videt.ro](https://shopilo.ro/magazin/videt.ro) este actualizata zilnic cu cele mai noi cod reducere Videt, voucher Videt si cupon promotional Videt.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Videt

Videt este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/videt.ro) cele mai bune cod reducere Videt, cupoane Videt verificate si voucher Videt active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-videt
```

```javascript
const { fetchCoupons } = require('cod-reducere-videt');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
