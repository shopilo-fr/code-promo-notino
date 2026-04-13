# Code promo Notino, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Notino** depuis [shopilo.fr](https://shopilo.fr/reductions/notino.fr). Renvoie les **coupons Notino** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-notino](https://shopilo-fr.github.io/code-promo-notino/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-notino
cd code-promo-notino
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Notino",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les parfums et cosmetiques",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/notino.fr"
  }
]
```

## Coupons Notino disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les parfums et cosmetiques | [shopilo.fr](https://shopilo.fr/reductions/notino.fr) |

Codes actifs : **[shopilo.fr/reductions/notino.fr](https://shopilo.fr/reductions/notino.fr)**

## Questions frequentes

### Comment utiliser un code promo Notino ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/notino.fr), ajoutez les produits a votre panier sur Notino et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Notino ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Notino les plus recents ?
La page [shopilo.fr/reductions/notino.fr](https://shopilo.fr/reductions/notino.fr) est mise a jour quotidiennement avec les codes promo Notino, bons de reduction Notino et coupons promotionnels Notino les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Notino

Notino est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/notino.fr), retrouvez les meilleurs codes promo Notino, coupons Notino verifies et bons de reduction Notino actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-notino
```

```javascript
const { fetchCoupons } = require('code-promo-notino');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
