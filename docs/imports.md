# Importation des exigences et des actions

**Spécification de travail proposée ; contrat de fichier non validé.**

## Parcours proposé

1. Choisir le type d'objet depuis la section concernée.
2. Sélectionner le fichier ; annoncer les formats réellement pris en charge.
3. Lire la structure et proposer un mapping uniquement sur les colonnes reconnues.
4. Prévisualiser les valeurs et les erreurs, sans écriture.
5. Valider les champs, les références, le périmètre et les doublons.
6. Afficher le bilan puis demander une confirmation explicite dans l'application.
7. Enregistrer selon la politique transactionnelle retenue.
8. Afficher le compte rendu et permettre de retrouver les objets enregistrés.

Le même service applicatif devra être appelé depuis les trois sections et depuis l'ajout manuel, afin de partager les validations et les contrôles d'accès. L'ajout manuel suit le même enregistrement mais n'a pas d'étape de lecture de fichier.

## Contrat à compléter

| Sujet | État |
| --- | --- |
| Formats CSV/XLSX ou autres, encodage, séparateur, taille maximale | À décider ; aucune compatibilité annoncée |
| Onglets et colonnes, champs requis et facultatifs | À relever sur un modèle autorisé |
| Dates, valeurs vides, textes, références externes | À définir sans substitution silencieuse |
| Identifiant d'exigence et lien action/exigence | À confirmer |
| Génération des identifiants d'actions | Indication TemyCertif à vérifier ; aucune règle HUBSMQ fixée |
| Doublons internes, objets déjà présents, réimport et mise à jour | Clé et politique à confirmer |
| Erreurs bloquantes et avertissements | À distinguer dans le contrat validé |
| Atomicité et reprise après échec | À décider avant écriture |

Les responsabilités, structures, statuts, échéances et liens ne doivent jamais être déduits ou complétés arbitrairement.

## Contrôles techniques proposés

- Vérifier les droits et le périmètre côté serveur avant lecture de données existantes et avant écriture.
- Ne pas faire confiance aux identifiants ni au périmètre fournis dans le fichier.
- Conserver la référence de ligne et de colonne pour expliquer une erreur.
- Bloquer l'enregistrement si le contrat ou la politique de doublons nécessaire n'est pas défini.
- Éviter toute écriture lors d'une prévisualisation ou d'une annulation.
- Garantir la cohérence des liens et tester l'absence de doublons lors d'un nouvel envoi.
- Ne pas journaliser les contenus complets ni les informations sensibles ; définir les métadonnées et la rétention.
- Traiter le contenu importé comme des données, jamais comme du code ou une formule à exécuter.

## Compte rendu proposé

Résultat explicite : succès, refus ou échec ; nombres de lignes lues, acceptées, rejetées et ignorées selon la politique retenue ; erreurs localisées et raison compréhensible ; référence du traitement si journalisation retenue. Les nombres doivent correspondre aux données effectivement persistées.

Les règles détaillées seront versionnées avant de livrer un premier adaptateur de fichier.
