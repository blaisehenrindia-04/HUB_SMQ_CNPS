# Premier découpage fonctionnel

Les lots ci-dessous sont des travaux proposés, sans calendrier ni responsable attribué. Ils ne sont pas des fonctionnalités déjà livrées.

| Lot | Livrable | Dépendance | Critères d'acceptation |
| --- | --- | --- | --- |
| F01 — Inventaire de l'existant | Localisation du code, ajout/import, stockage, droits et points d'entrée | Accès au code de référence | Fonctions réutilisables identifiées ; écarts documentés ; stack consignée |
| F02 — Contrat d'import | Modèles autorisés, mapping, types, règles de liens et doublons | F01 et arbitrages métier | Champs confirmés sourcés ; inconnues explicites ; exemples synthétiques et cas invalides |
| F03 — Lecture et prévisualisation | Adaptateur du premier format confirmé, rapport d'erreurs | F02 | Lecture sans écriture ; erreurs par ligne/colonne ; fichier invalide refusé ; annulation sans effet |
| F04 — Exigences | Service partagé d'ajout manuel et d'import avec persistance | F01–F03, droits et atomicité définis | Enregistrement accessible après rechargement ; droits vérifiés ; réimport conforme à la politique de doublons ; échec cohérent |
| F05 — Actions | Service partagé d'ajout manuel et d'import avec relations validées | F02–F04 selon règles de liens | Liens contrôlés ; identifiants selon règle confirmée ; doublons traités ; données retrouvables |
| F06 — Intégration des sections | Commandes en haut des trois sections | F04–F05 | Exigences dans Norme & auto-évaluation, actions dans Plan d'action, les deux dans Mon espace ; mêmes services ; cohérence graphique |
| F07 — Recette et traçabilité | Scénarios de bout en bout et compte rendu | F06 | Permissions, persistance, réimport, erreurs et absence de régression vérifiés ; aucune donnée réelle dans les tests publics |

## Définition de terminé

Le lot dispose de critères vérifiables, de décisions sourcées, d'une revue et d'une validation adaptée. Une fonctionnalité d'import n'est terminée que si les données sont réellement enregistrées, accessibles dans le bon périmètre et si les échecs et réimportations ont été testés.
