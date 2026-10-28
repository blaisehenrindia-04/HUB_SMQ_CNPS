# Validation à mettre en place

Les scénarios suivants guideront les tests du futur code :
- fichier valide, vide, mal formé, colonnes absentes et valeurs invalides ;
- prévisualisation et annulation sans écriture ;
- doublon dans le fichier, doublon existant et réimportation selon la politique validée ;
- référence inconnue et lien hors périmètre ;
- utilisateur autorisé ou refusé, isolation des organisations/projets selon l'existant ;
- échec de persistance, résultat transactionnel conforme à la décision et compte rendu exact ;
- données retrouvables après rechargement ;
- ajout manuel et import depuis les trois sections ; absence de régression.

Utiliser uniquement des données synthétiques explicitement marquées. Les résultats attendus dépendant des règles métier seront fixés avec le contrat validé. Aucun test applicatif ni résultat de recette n'est revendiqué par ce socle.
