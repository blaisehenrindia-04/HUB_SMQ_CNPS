# HUB_SMQ_CNPS

Socle initial de HUBSMQ, consacré en priorité à l'ajout manuel et à l'importation des exigences et des actions.

**État : cadrage et organisation du dépôt. Aucune application exécutable, base de données ou import opérationnel n'est encore livré.**

## Objectifs établis

Piloter et suivre les exigences, les actions correctives et la préparation aux audits de certification. Les demandes antérieures HUBSMQ/TemyCertif précisent les points d'entrée suivants :

| Section | Ajout manuel et import |
| --- | --- |
| Norme & auto-évaluation | Exigences |
| Plan d'action | Actions |
| Mon espace | Exigences et actions |

Les commandes doivent être clairement placées en haut de chaque section. Les données enregistrées doivent rester accessibles. Réutiliser les fonctions existantes, éviter les doublons et préserver l'ergonomie, la cohérence graphique et les autres fonctionnalités.

## Limites du socle

Le code de l'application existante n'est pas présent dans ce dépôt. L'architecture, le lien technique avec TemyCertif, les formats exacts et les règles métier restent à préciser. Aucun choix de framework, de fournisseur, de licence ou de modèle de base n'est imposé. Aucune donnée métier réelle ni contenu normatif n'est publié.

## Organisation

- `docs/cadrage.md` : éléments établis, sources et questions ouvertes.
- `docs/imports.md` : parcours et contrat de travail proposé pour les imports.
- `docs/backlog.md` : premier découpage fonctionnel et critères d'acceptation.
- `docs/decisions/README.md` : registre des décisions.
- `src/README.md` : responsabilités envisagées pour le futur code.
- `tests/README.md` : scénarios de validation attendus.
- `examples/imports/README.md` : règles pour les futurs exemples synthétiques.
- `CONTRIBUTING.md` : conventions de travail.

## Démarrer

1. Lire le cadrage et les questions ouvertes.
2. Retrouver le code et les fonctions d'ajout/import existants avant toute implémentation.
3. Valider le contrat de données sur un exemple autorisé et anonymisé.
4. Suivre les lots de `docs/backlog.md` ; consigner chaque décision.

Il n'existe à ce stade aucune commande d'installation ou de lancement. Le dépôt privé TemyCertif n'est pas modifié par ce socle.
