# Cadrage et provenance

## Établi

| Élément | Provenance et portée |
| --- | --- |
| Pilotage des exigences, actions correctives et préparation aux audits | Objectif exprimé le 7 avril 2026 dans le contexte HUBSMQ/Temy |
| Ajout manuel et import dans les trois sections décrites au README | Demande du 26 octobre 2026 dans le contexte HUBSMQ/TemyCertif |
| Réutilisation de l'existant, absence de doublons, ergonomie préservée, enregistrement accessible | Contraintes de la même demande |
| Création du socle de HUB_SMQ_CNPS, priorité aux exigences/actions, aucune invention métier | Instruction du 28 octobre 2026 |

Ces éléments ont été retrouvés dans l'historique des échanges. Ils ne prouvent pas l'existence d'un code partagé ou d'un déploiement commun.

## Contexte TemyCertif à vérifier sur les sources

Le contexte documentaire retrouvé mentionne :
- un cahier des charges consolidé favorisant la réutilisation du code, de la base et des flux existants, avec organisations/projets et habilitations séparées ;
- un modèle d'import où « Exigences » et « Structures » sont obligatoires, « Points de contrôle » et « Processus » recommandés, et « Plan d’action », « Jalons », « Risques », « Opportunités » facultatifs ;
- une génération automatique des identifiants d'actions et de points de contrôle.

Ces indications proviennent d'un résumé de contexte documentaire, sans examen direct des fichiers dans ce dépôt. Elles ne constituent pas encore un contrat d'import HUBSMQ. Le modèle réel et ses en-têtes doivent être examinés avant implémentation. Les fichiers métier ne sont pas reproduits dans ce dépôt public.

## À préciser avant développement

| Question | Conséquence |
| --- | --- |
| Où est le code de l'application existante et quelle version fait référence ? | Inventaire des fonctions réutilisables et choix de stack |
| HUBSMQ et TemyCertif partagent-ils du code, des données ou seulement des besoins ? | Frontières d'intégration |
| Quels formats, onglets, en-têtes, types et champs obligatoires sont autorisés ? | Contrat de données versionné |
| Quelles clés définissent un doublon et comment traiter une réimportation ? | Idempotence, création ou mise à jour |
| Une action peut-elle exister sans exigence ? Plusieurs liens sont-ils permis ? | Validation des relations |
| Quels statuts, responsabilités, échéances et référentiels sont confirmés ? | Validation métier ; aucune liste inventée |
| Quels droits, périmètres d'organisation/projet et règles de conservation appliquer ? | Contrôles d'accès et journalisation |
| Import atomique ou acceptation partielle ? Quels volumes et limites ? | Transactions, performances et compte rendu |
| Quels échantillons peuvent être utilisés et publiés ? Quelle licence retenir ? | Jeux de test et réutilisation du dépôt |

## Propositions techniques

Le parcours de prévisualisation, la séparation des responsabilités et le découpage des lots sont des propositions de ce socle. Leur présence dans le dépôt ne vaut pas validation métier. Toute décision validée sera datée dans le registre.
