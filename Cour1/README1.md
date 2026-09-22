# PARTIE A — Position

## A1 · Typer les colonnes (20 min)

| Colonne             | Type (quantitative continue / discrète / qualitative nominale / ordinale / date / identifiant) | Moyenne possible ? (oui/non) |
| ------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------- |
| `ID_commande`       | identifiant                                                                                    | non                          |
| `Date_commande`     | date                                                                                           | non                          |
| `Magasin`           | quanlitative nominale                                                                          | non                          |
| `Departement`       | qualitative nominale                                                                           | non                          |
| `Categorie`         | qualitative nominale                                                                           | non                          |
| `Produit`           | qualitative nominale                                                                           | non                          |
| `Canal`             | qualitative nominale                                                                           | non                          |
| `Quantite`          | quantitative discrete                                                                          | non                          |
| `Prix_unitaire_TTC` | quantitative continue                                                                          | oui                          |
| `Remise`            | quantitative continue                                                                          | oui                          |
| `Montant_TTC`       | quantitative continue                                                                          | oui                          |
| `Statut`            | qualitative nominale                                                                           | non                          |
| `Note_client`       | qualitative ordinale                                                                           | non                          |

<em>La moyenne de Note_client est discutable car les notes peuvent être classées de la moins bonne à la meilleure, mais les écarts entre les niveaux de satisfaction ne sont pas nécessairement équivalents.</em>

## Question A2. L'écart entre moyenne et médiane est énorme sur Montant_TTC et Prix_unitaire_TTC, presque nul sur Note_client. Qu'est-ce que cela t'apprend sur la forme de chacune de ces trois distributions ? (3 lignes)

<em>L'ecart entre la mediane et la moyenne est du au fait que les prix élevés font augmenter la moyenne les prix sont étaler sur la droite. Alors que pour les notes clients c'est symétriques</em>

## Question A3. Nadia veut écrire dans sa présentation : \_« Nos 613 commandes obtiennent une note moyenne de 4,1/5. »\_ Cette phrase est-elle exacte ? Réécris-la correctement.

<em> « Nos 560 commandes obtiennent une note moyenne de 4,1/5» </em>

## Question A4. Que dirais-tu à Nadia si elle voulait annoncer « 1 029 700 € de chiffre d'affaires 2025 » ?

✅ Part attendue : **33,4 %**

<em> 1 029 700€ n'est pas le chiffre d'affaire de l'année car il comptabilise toute les commande livrée, annulée et retourner. Les commande livrées représente seulement 33,4% du montant TTC total donc 343 877€ </em>

| Catégorie   | Nb commandes | CA total      | Montant moyen |
| ----------- | ------------ | ------------- | ------------- |
| Accessoires | 189          | 15 730,75€    | 82,23€        |
| Atelier     | 134          | 7 874,70€     | 58,77€        |
| VAE         | 97           | 672 822,50€   | 6 936,31€     |
| VTT         | 88           | 157 276,05€   | 1 787,23€     |
| Vélo urbain | 105          | 175 996,50€   | 1 676,16€     |
| **Total**   | 613          | 1 029 700,50€ | 10 541,70€    |

## Question A5.

**Le VAE représente quel pourcentage des commandes** ?
<em> 15,82 %</em>

**Quel pourcentage du montant** ?
<em>65,34%</em>

**Commente l'écart en une phrase.**

<em>Le VAE représente seulement 15,8 % des commandes mais 65,3 % du montant total, car les commandes de VAE ont un montant moyen beaucoup plus élevé</em>

## Question A6. Les deux résultats diffèrent. Lequel utiliserais-tu, et pour dire quoi ? et comment le corrigerais-tu ?

<em>Je choisirais la moyenne pondérée car il prend en compte </em>

## A7 · La phrase de restitution (15 min)

Écris, dans une cellule de l'onglet `Position`, **une seule phrase** décrivant le montant typique
d'une commande Cyclo'Nord. Elle doit contenir un indicateur de position, son périmètre, et ne pas
induire Nadia en erreur.

<em>. </em>

# PARTIE B — Dispersion
