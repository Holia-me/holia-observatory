# Collecte et production des données

Ce document décrit la chaîne de production des données publiées par l'Observatoire Holia, sans exposer les composants techniques propriétaires de la plateforme holia.me.

## 1. Sources observées

L'Observatoire s'appuie exclusivement sur des **informations déjà publiques ou rendues publiques** dans le cadre du référentiel Holia :

- fiches praticiens visibles dans la recherche publique ;
- métadonnées déclarées (métier principal, localisation, mots-clés de prise en charge) ;
- liens éditoriaux entre sujets, métiers et approches, maintenus dans la taxonomie Holia ;
- dates d'enregistrement technique des profils.

Aucune donnée issue de dossiers médicaux, de résultats cliniques ou de parcours de soins n'entre dans le périmètre.

## 2. Structuration éditoriale

Avant toute agrégation, les informations brutes sont normalisées dans un **référentiel éditorial** :

| Couche | Rôle |
|--------|------|
| **Métiers** | Libellés professionnels déclarés et harmonisés (ex. sophrologue, naturopathe) |
| **Sujets** | Problématiques ou thèmes d'accompagnement (ex. sommeil, anxiété, burn-out) |
| **Approches** | Modalités ou filières associées aux suets dans la taxonomie Holia |
| **Territoires** | Communes et départements reconnus dans le référentiel géographique Holia |

Cette structuration permet des comparaisons cohérentes d'une édition à l'autre, sous réserve des évolutions documentées de la taxonomie.

## 3. Agrégation

Les études OBS-001 à OBS-010 sont produites par **agrégation statistique descriptive** :

- comptages et parts relatives ;
- classements (top N) avec seuils de lisibilité lorsque nécessaire ;
- mesures de concentration ou de diversité ;
- co-occurrences entre suets dans les déclarations observées.

Chaque agrégat est calculé sur un **snapshot daté** : les chiffres correspondent à un instant T, pas à une mesure en temps réel permanente.

## 4. Anonymisation et protection

Les règles appliquées aux publications ouvertes :

- **aucun identifiant personnel** (nom, email, téléphone, adresse exacte) dans les CSV ;
- **seuils de regroupement** sur les petites communes lorsque la lisibilité l'exige ;
- **exclusion** des comptes internes, de démonstration et des fiches masquées ;
- **pas de croisement** permettant de réidentifier un praticien isolé.

Les fichiers publiés sont des **tableaux agrégés**, jamais des exports bruts de fiches individuelles.

## 5. Contrôle qualité

Avant publication, chaque édition passe par :

1. Vérification du périmètre population (profils éligibles vs exclus).
2. Contrôle de cohérence des totaux entre jeux de données d'une même étude.
3. Rédaction des limites d'interprétation et du README associé.
4. Publication synchronisée sur holia.me et archivage dans ce dépôt.

## 6. Fréquence de mise à jour

| Type | Rythme indicatif |
|------|------------------|
| Éditions majeures | Trimestriel ou semestriel (selon calendrier éditorial) |
| Jeux de données CSV | À chaque nouvelle édition d'étude |
| Documentation méthode | Lors de changement de version (v1.1, v2.0, etc.) |

Les dates d'arrêté et numéros d'édition (`2026-05`, `2026-06`) figurent dans chaque fichier et README.

## 7. Ce que ce document ne décrit pas

Par conception, ce dépôt public **ne contient pas** :

- scripts d'ingestion ou d'enrichissement automatique ;
- algorithmes de matching ou de classement internes ;
- règles SEO ou logiques produit de holia.me ;
- accès à la base de données de production.

Ces éléments relèvent de l'infrastructure privée Holia et ne sont pas nécessaires pour comprendre ou réutiliser les agrégats publiés.

## Voir aussi

- [limitations.md](./limitations.md)
- [glossary.md](./glossary.md)
- [Études](../studies/README.md)
