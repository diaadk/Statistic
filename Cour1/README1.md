# PARTIE A — Position

google sheet : https://docs.google.com/spreadsheets/d/1XtCHi-tSLJQ9kiQiFY3a4_SeehYDVZ0m6vgPvd8fgsk/edit?usp=sharing

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

<em>L'ecart entre la mediane et la moyenne est du au fait que les prix élevés font augmenter la moyenne, les prix sont étaler sur la droite. Alors que pour les notes clients c'est symétriques</em>

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

<em>Je choisirais la moyenne pondérée, car elle prend en compte le montant des commandes. Les commandes avec un montant plus élevé ont davantage de poids dans le résultat. Après avoir exclu les 53 notes vides, le résultat est de 4,07/5. La moyenne simple de 4,10/5 est aussi correcte si l'on souhaite donner le même poids à chaque client, car elle mesure directement la note moyenne attribuée par les clients.</em>

## A7 · La phrase de restitution (15 min)

Écris, dans une cellule de l'onglet `Position`, **une seule phrase** décrivant le montant typique
d'une commande Cyclo'Nord. Elle doit contenir un indicateur de position, son périmètre, et ne pas
induire Nadia en erreur.

<em> En 2025 sur l'ensemble des commandes de Cyclo'Nord, le montant médian d'une commande est de 177 € TTC.</em>

# PARTIE B — Dispersion

## Question B1. Les deux écarts-types diffèrent de 12 € sur 15 500. Explique en deux lignes laquelle des deux fonctions convient ici, et pourquoi la différence est si faible.

<em> Les deux écart-type différe de 12€ car l'un prend en compte tout le tableau alors que l'autre prend tout le tableau n- 1, c'est pourquoi la différence est si faible. Les deux fonctions conviennent mais l'écart type standard corrige la sous-estimation de la dispersion réelle </em>

## B2 · Le résumé à cinq nombres ET Complète la phrase :

|          | Formule                    | Valeur    |
| -------- | -------------------------- | --------- |
| Effectif | `=NB(...)`                 | 613       |
| Minimum  | `=MIN(...)`                | 15,20€    |
| Q1       | `=QUARTILE.INCLURE(...;1)` | 50,15€    |
| Médiane  | `=MEDIANE(...)`            | 177€      |
| Q3       | `=QUARTILE.INCLURE(...;3)` | 1790€     |
| Maximum  | `=MAX(...)`                | 379 050€  |
| IQR      | `=Q3-Q1`                   | 1 739,85€ |

« La moitié des commandes Cyclo'Nord se situe entre 50,15€ € et
1 790 €. »

## B3 · Repérer les valeurs atypiques Le seuil bas est négatif. Est-ce un bug ? Que faut-il en conclure sur la forme de la distribution ?

<em>Les seuil bas est négatif car il y a une grosse différence entre le Q1 50,15€ et l'IQR 1 739€. La forme de la distribution est vers la droite à cause des commandes élevés </em>

## Question B4. Pour chacune des trois commandes de quantité 100, dis si tu la gardes, si tu l'écartes ou si tu l'analyses à part — et justifie. Aucune des trois réponses n'est automatiquement fausse ; c'est la justification qui compte.

<em>
Je deciderais de garder les deux commandes "en cours" et "livrée" dans mon analyse, car même si comparer aux autres commandes elles sont plus conséquente quantité, elles correspondent à des commandes réelles. Je metterais de coté la commande de 379 000€ car elle est annulé et c'est un haut montant qui influence les statistiques. Je l'analyserais à part, car il est possible qu'il s'agisse d'une véritable commande de flotte pour une entreprise. </em>

## B4 · Mesurer l'effet d'une seule ligne

| Mesure     | Avec        | Sans      | Variation en % |
| ---------- | ----------- | --------- | -------------- |
| Moyenne    | 1 679,77 €  | 1 063,15€ | -36,71%        |
| Médiane    | 177,00 €    | 177€      | 0%             |
| Écart-type | 15 504,58 € | 2707,51€  | -82,54%        |
| IQR        | 1 739,85 €  | 1673,10€  | -3,84%         |

## Question B5. Classe ces quatre indicateurs du plus robuste au plus sensible.

<em> 
Médiane </br>
IQR </br>
Moyenne </br>
Écart-type </br>
</em>

## B6 · Le cas Arras

## Question B7. Arras est premier sur une colonne et dernier sur une autre. Rédige les deux phrases que tu mettrais dans un rapport : celle qui décrit le fait, et celle qui l'explique.

<em>Arras est le premier magasin en CA pour l'ensembles de ses commandes avec 442 616,80 €, mais dernier en CA livré avec 29 214,80 €.
Cet écart s'explique par une commande de 379 050 €, enregistrée à Arras mais annulée, qui gonfle le CA. </em>
