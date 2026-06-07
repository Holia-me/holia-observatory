# Glossaire

Définitions des termes employés dans l'Observatoire Holia et dans les jeux de données associés.

## Approche

Modalité, filière ou cadre d'intervention associé à un **sujet** (besoin ou thématique) dans la taxonomie éditoriale Holia. Exemples : sophrologie, hypnose thérapeutique, naturopathie.

Dans les études OBS-002, une « approche » correspond le plus souvent au **métier principal déclaré** d'un praticien lié à un sujet donné. Ce n'est pas une classification médicale officielle.

## Métier

Profession ou filière telle que **déclarée sur la fiche praticien** Holia et harmonisée dans le référentiel des métiers (ex. sophrologue, ostéopathe, coach bien-être).

Le métier principal (`profession_id`) sert de base aux classements par filière. Il ne reflète pas nécessairement l'ensemble des qualifications ou activités du professionnel.

## Sujet

Thématique ou problématique d'accompagnement structurée dans la taxonomie Holia (ex. stress et anxiété, troubles du sommeil, burn-out). Les sujets permettent le maillage éditorial entre contenus, hubs thématiques et profils référencés.

Un sujet n'est **pas un diagnostic médical** dans le cadre de l'Observatoire.

## Praticien

Professionnel du bien-être ou de l'accompagnement référencé sur Holia, dont la fiche est **active et visible** dans la recherche publique au moment de l'arrêté de l'étude.

Sont exclus des agrégats : comptes internes, fiches de démonstration, profils masqués.

## Filière

Synonyme opérationnel de **métier déclaré** dans les tableaux de répartition (OBS-001). Désigne la catégorie professionnelle retenue pour le classement, par opposition aux combinaisons multi-métiers ou libellés agrégés très larges.

## Référentiel

Ensemble structuré et versionné des entités que Holia utilise pour publier son écosystème :

- métiers ;
- sujets et approches ;
- communes et territoires reconnus ;
- règles de visibilité publique.

L'Observatoire mesure le **référentiel tel qu'il existe à une date donnée**, pas la réalité économique ou sanitaire hors plateforme.

## Graphe Holia

Représentation des **liens éditoriaux** entre entités du référentiel : praticien ↔ métier, praticien ↔ sujet, sujet ↔ approche, praticien ↔ commune, etc.

Les études de co-occurrence (OBS-004, OBS-006, OBS-007) et de diversité (OBS-010) exploitent ce graphe pour produire des agrégats descriptifs. Le graphe complet n'est pas publié dans ce dépôt ; seuls les **résultats agrégés** le sont.

## Observatoire Holia

Pôle de publication de Holia dédié à la **transparence des données agrégées** issues du référentiel public. Il produit :

- des **études** numérotées (OBS-001 à OBS-010 et suivantes) ;
- des **jeux de données CSV** réutilisables ;
- une **méthodologie** accessible et versionnée.

Site : [https://holia.me/observatoire](https://holia.me/observatoire)

## Édition

Période de publication d'un snapshot (ex. `2026-05`, `2026-06`). Une édition regroupe un ou plusieurs rapports et leurs jeux de données, arrêtés à une date précise.

## Snapshot

Extraction figée du référentiel Holia à une **date d'arrêté** documentée. Tous les chiffres d'une édition proviennent du même snapshot ou de snapshots compatibles explicitement indiqués.

## Co-occurrence

Présence conjointe de deux suets ou thèmes dans les **déclarations observées** sur une même fiche ou dans des agrégats de proximité taxonomique. Une co-occurrence **n'implique pas** une relation causale ou clinique.

## Part relative

Rapport entre le volume d'une catégorie (métier, sujet, filière) et un total local ou global **dans le référentiel Holia**. Distincte du volume absolu : une commune peut compter peu de praticiens d'un métier tout en affichant une part relative élevée si l'offre locale est peu diversifiée.

## Voir aussi

- [limitations.md](./limitations.md)
- [data-collection.md](./data-collection.md)
