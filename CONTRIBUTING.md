# Contribuer

## Conventions proposées pour ce dépôt

- Documentation et échanges fonctionnels en français ; fichiers UTF-8, fins de ligne LF.
- Chemins techniques en minuscules sans espaces ; conserver les libellés de l'interface lorsqu'ils sont cités.
- Branches courtes : `docs/sujet`, `feat/sujet`, `fix/sujet`, `chore/sujet`.
- Commits ciblés : `docs: préciser le contrat d'import`, `feat: ...`, `fix: ...`, `chore: ...`.
- Après l'amorçage, proposer les changements par pull request vers `main`. Cette convention n'active aucune protection GitHub.
- Relier les travaux aux lots du backlog ; expliquer le problème, le comportement obtenu et la validation.

## Avant de coder

Retrouver l'existant. Ne pas choisir une nouvelle stack, créer une base ou dupliquer une fonction sans décision documentée. Distinguer demande confirmée, proposition et question ouverte. Ne jamais transformer une hypothèse en règle métier.

## Revue et validation

Vérifier les critères d'acceptation et les liens documentaires. Pour du code d'import : tests utiles sur droits, erreurs, doublons, liens, persistance et régression. Fournir la commande et le résultat des contrôles ; signaler ce qui n'a pas été testé.

## Dépôt public

Publier uniquement du code et des exemples synthétiques autorisés. Ne pas committer de données CNPS, fichiers sources métier, données personnelles, justificatifs, exports, mots de passe ou clés. Les exclusions Git sont une aide, pas une garantie de confidentialité. Aucune licence n'est choisie dans ce socle.
