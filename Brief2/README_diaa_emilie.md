source : carburants_france_releve.xlsx <br>
lien google sheet https://docs.google.com/spreadsheets/d/1mj10AiRd26li8wP2L3ZeW7-_ld9Th37k/edit?gid=1936346784#gid=1936346784

### Axe d’analyse

<ul>
  <li> Comparaison nationale des prix des carburants <strong>  -  Comparaison_nationale </strong> </li>
<li>  Analyse de la dispersion des prix dans les Hauts-de-France <strong> - Dispersion_HDF </strong> </li>
<li> Influence du type de station : route ou autoroute <strong> - Type_de_station </strong>  </li>
<li> Détection et analyse des valeurs atypiques <strong>  - Valeurs_atypiques </strong>  </li>
</ul>

## Les carburants sont-ils réellement plus chers dans les Hauts-de-France que dans les autres régions,et quels facteurs expliquent les écarts de prix entre stations?

<em>Les automobilistes des Hauts-de-France paient-ils réellement leur carburant plus cher qu’ailleurs en France ?
L’analyse des prix médians montre que la région ne figure pas systématiquement parmi les plus chères et que la situation varie selon le carburant.
Les écarts apparaissent également au sein même des Hauts-de-France, selon les départements et les stations.
Le SP98 se distingue notamment par une dispersion des prix plus importante.
L’analyse révèle enfin que certains prix atypiques sont plausibles et correspondent à de véritables différences de prix plutôt qu’à de simples erreurs de saisie.</em>

## Réponse à la question du lecteur

L’analyse ne permet pas d’affirmer que les carburants sont systématiquement plus chers dans les Hauts-de-France que dans les autres régions. La comparaison des prix médians par carburant et par région montre une situation différente selon le carburant. Par exemple, dans les Hauts-de-France, le prix médian observé est de 0,851 € pour l’E85, 2,379 € pour le Gazole, 1,010 € pour le GPLc, 2,180 € pour le SP95 et 2,272 € pour le SP98.
L’analyse de la dispersion montre également que les différences ne s’expliquent pas uniquement par la région. Dans les Hauts-de-France, le SP98 est le carburant dont les prix sont les plus dispersés, avec un écart-type d’environ 0,12 €, tandis que l’E85 et le GPLc présentent une dispersion plus faible. Des différences sont également observées selon les départements et le type de station.

## Ce que nous avons trouvé de plus intéressant

L’analyse des valeurs atypiques constitue un résultat supplémentaire intéressant. La méthode de l’IQR identifie plusieurs prix dépassant le seuil atypique haut pour le SP98, le SP95, le GPLc et l’E85. Cependant, leur vérification montre que plusieurs de ces valeurs sont cohérentes avec d’autres observations ou associées à des stations autoroutières. Elles ont donc été conservées : une valeur statistiquement atypique n’est pas nécessairement une erreur dans les données.

## Les trois limites du jeu de données

<ol>
<li> Les données correspondent à un relevé effectué à une période donnée : les prix des carburants évoluent dans le temps et les résultats ne décrivent donc pas nécessairement la situation à une autre date.</li>

<li>Le nombre d’observations n’est pas identique pour tous les carburants. Certains, comme le GPLc, sont moins représentés, ce qui limite les comparaisons directes entre carburants.</li>

<li>Le jeu de données permet d’observer les différences de prix entre régions, départements et types de stations, mais il ne permet pas à lui seul d’identifier toutes les causes de ces écarts.</li>
</ol>

Auteurs : Diakemba Diaby et Émilie Farah
