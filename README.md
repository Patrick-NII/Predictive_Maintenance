# À propos du Dataset

## Ensemble de données de classification de la maintenance prédictive des machines

Étant donné que les ensembles de données de maintenance prédictive réels sont généralement difficiles à obtenir et particulièrement difficiles à publier, nous présentons et fournissons un ensemble de données synthétiques qui reflète la maintenance prédictive réelle rencontrée dans l'industrie au mieux de nos connaissances.

L'ensemble de données se compose de 10 000 points de données stockés sous forme de lignes avec 14 entités dans les colonnes :

- **UID** : Identifiant unique compris entre 1 et 10,000.
- **productID** : Composé d'une lettre L, M ou H pour faible (50 % de tous les produits), moyenne (30 %) et élevée (20 %) comme variantes de qualité du produit et d'un numéro de série spécifique à la variante.
- **température de l'air [K]** : Générée à l'aide d'un processus de marche aléatoire, normalisée ultérieurement à un écart type de 2 K autour de 300 K.
- **température du processus [K]** : Générée à l'aide d'un processus de marche aléatoire normalisé à un écart type de 1 K, ajouté à la température de l'air plus 10 K.
- **vitesse de rotation [tr/min]** : Calculée à partir d'une puissance de 2860 W, superposée à un bruit normalement distribué.
- **couple [Nm]** : Les valeurs de couple sont normalement distribuées autour de 40 Nm avec un σ = 10 Nm et aucune valeur négative.
- **usure de l'outil [min]** : Les variantes de qualité H/M/L ajoutent 5/3/2 minutes d'usure de l'outil utilisé dans le processus.
- **étiquette « panne de machine »** : Indique si la machine est tombée en panne dans ce point de données particulier pour l'un des modes de défaillance suivants.

Important : il y a deux cibles - Ne faites pas l'erreur d'utiliser l'une d'entre elles comme fonctionnalité, car cela entraînerait une fuite.
- **Objectif** : Échec ou pas.
- **Type de défaillance** : Type de défaillance.

### Colonnes du dataset

- **UDI** : Identifiant unique du produit.
- **Product ID** : Identifiant du produit.
- **Type** : Type de produit.
- **Air temperature [K]** : Température de l'air en Kelvin.
- **Process temperature [K]** : Température du processus en Kelvin.
- **Rotational speed [rpm]** : Vitesse de rotation en tours par minute.
- **Torque [Nm]** : Couple en Newton-mètres.
- **Tool wear [min]** : Usure de l'outil en minutes.
- **Target** : Cible (éventuellement le résultat ou la classe à prédire).
- **Failure Type** : Type de défaillance.
