# Pistes pour le traitement du dataset


Le but est de créer un système de recommandation basé sur le Dataset MovieLens.

## Piste 1 : Recommandation de films similaires à un certain film en se basant sur genome-scores


### Description du probleme

En se basant sur le fichier genome-scores.csv, chaque film identifié par son movieId a un pourcentage de "relevance" pour chacun des 1128 tags decrits dans le fichier genome-tags. Pour illustrer cela, on pourrait considérer que chaque film peut etre placé tel un point sur un graph a 1128 dimensions, le but étant de déterminer quels sont les points les plus proches (films a recommander). On en déduit ainsi qu'on a à faire à un probleme supervisé de classification.

### Composition du dataset utilisable

- Colonne movieId de genome-scores.csv
- Colonne title de movies.csv pour assisgner un titre de film a chaque movieId
- Colonne tagId de genome-scores.csv
- Colonne tag de genome-tags.csv pour assigner un nom de tag a chaque tagId
- Colonne relevance de genome-scores.csv

### Algorithme à utiliser

A déterminer
