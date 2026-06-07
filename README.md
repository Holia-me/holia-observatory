# Observatoire Holia

**Données ouvertes, études et méthodologie** autour du référentiel public [Holia](https://holia.me), plateforme de mise en relation avec des professionnels du bien-être et de l'accompagnement.

Ce dépôt est la **vitrine publique** de l'Observatoire Holia. Il documente les études publiées, les jeux de données réutilisables et le cadre méthodologique. Il ne contient ni code applicatif de holia.me, ni données brutes propriétaires, ni algorithmes internes.

---

## Mission

L'Observatoire Holia a pour objectif de :

1. **Publier** des agrégats statistiques descriptifs issus du référentiel public Holia ;
2. **Documenter** la méthode, le périmètre et les limites de chaque publication ;
3. **Faciliter la réutilisation** des données par les chercheurs, journalistes, institutions et citoyens ;
4. **Renforcer la transparence** sur ce que la plateforme observe, sans prétendre représenter l'ensemble du marché français.

---

## Liens utiles

| Ressource | URL |
|-----------|-----|
| Observatoire en ligne | [holia.me/observatoire](https://holia.me/observatoire) |
| Études | [holia.me/observatoire/etudes](https://holia.me/observatoire/etudes) |
| Jeux de données CSV | [holia.me/observatoire/datasets](https://holia.me/observatoire/datasets) |
| Méthodologie | [holia.me/observatoire/methodologie](https://holia.me/observatoire/methodologie) |
| Portail Open Data France | [data.gouv.fr](https://www.data.gouv.fr/) |

---

## Méthodologie générale

Les publications OBS reposent sur des **snapshots datés** du référentiel Holia :

- profils praticiens **actifs et visibles** en recherche publique ;
- agrégation **anonymisée** (comptages, parts, classements, co-occurrences) ;
- taxonomie éditoriale Holia (métiers, sujets, approches, territoires) ;
- version de méthode documentée (v1.0 pour les éditions 2026-05 et 2026-06).

Documentation détaillée dans [`methodology/`](./methodology/README.md).

---

## Limites essentielles

Les chiffres de l'Observatoire :

- décrivent **le référentiel Holia**, pas la France entière ;
- **ne constituent pas** une statistique officielle (INSEE, DREES, etc.) ;
- **n'ont pas de valeur médicale** ni de valeur de recommandation thérapeutique ;
- reflètent des **déclarations observées** ou une **taxonomie éditoriale**, selon l'étude.

Lire [`methodology/limitations.md`](./methodology/limitations.md) avant toute réutilisation.

---

## Études publiées (OBS-001 à OBS-010)

| ID | Titre | Édition |
|----|-------|---------|
| [OBS-001](./studies/obs-001.md) | L'offre de bien-être sur Holia | 2026-05 |
| [OBS-002](./studies/obs-002.md) | Répartition nationale des approches par besoin | 2026-06 |
| [OBS-003](./studies/obs-003.md) | Spécialisations revendiquées par métier | 2026-06 |
| [OBS-004](./studies/obs-004.md) | Problématiques associées au burn-out | 2026-06 |
| [OBS-005](./studies/obs-005.md) | Sophrologie par territoire | 2026-06 |
| [OBS-006](./studies/obs-006.md) | Problématiques associées à l'anxiété | 2026-06 |
| [OBS-007](./studies/obs-007.md) | Problématiques associées au sommeil | 2026-06 |
| [OBS-008](./studies/obs-008.md) | Villes par métier du bien-être | 2026-06 |
| [OBS-009](./studies/obs-009.md) | Concentration des spécialisations par métier | 2026-06 |
| [OBS-010](./studies/obs-010.md) | Diversité de l'offre par ville | 2026-06 |

Index complet : [`studies/README.md`](./studies/README.md)

---

## Jeux de données publics

**28 fichiers CSV** répartis sur 10 études (identifiants D01 à D28).

| Étude | Fichiers | Dossier |
|-------|----------|---------|
| OBS-001 | 4 | [`datasets/obs-001/`](./datasets/obs-001/README.md) |
| OBS-002 | 2 | [`datasets/obs-002/`](./datasets/obs-002/README.md) |
| OBS-003 | 2 | [`datasets/obs-003/`](./datasets/obs-003/README.md) |
| OBS-004 | 2 | [`datasets/obs-004/`](./datasets/obs-004/README.md) |
| OBS-005 | 2 | [`datasets/obs-005/`](./datasets/obs-005/README.md) |
| OBS-006 | 2 | [`datasets/obs-006/`](./datasets/obs-006/README.md) |
| OBS-007 | 2 | [`datasets/obs-007/`](./datasets/obs-007/README.md) |
| OBS-008 | 2 | [`datasets/obs-008/`](./datasets/obs-008/README.md) |
| OBS-009 | 2 | [`datasets/obs-009/`](./datasets/obs-009/README.md) |
| OBS-010 | 2 | [`datasets/obs-010/`](./datasets/obs-010/README.md) |

Catalogue : [`datasets/README.md`](./datasets/README.md)

**Téléchargement direct** : chaque fiche indique l'URL `https://holia.me/observatoire/datasets/{slug}.csv`

---

## À propos des données

### Ce que contiennent les CSV

- tableaux **agrégés** (effectifs, parts, rangs, indices, co-occurrences) ;
- métadonnées d'édition (slug, labels, territoires, métiers) ;
- **aucune donnée personnelle** identifiable.

### Ce que les CSV ne contiennent pas

- fiches praticiens individuelles ;
- coordonnées, avis, prix, agendas ;
- code source ou paramètres de calcul internes.

### Licence

Tous les jeux de données et la documentation de ce dépôt sont publiés sous **[Creative Commons Attribution 4.0 (CC BY 4.0)](./LICENSE)**.

Citation type :

> Observatoire Holia. *Titre de l'étude* (OBS-00X, édition YYYY-MM, arrêté AAAA-MM-JJ). Licence CC BY 4.0. https://holia.me/observatoire

### data.gouv.fr

Les fiches correspondantes sont **en cours de déploiement** sur [data.gouv.fr](https://www.data.gouv.fr/). En attendant, holia.me reste la source de référence pour le téléchargement et les métadonnées à jour.

---

## Structure du dépôt

```
holia-observatory/
├── README.md                 # Ce fichier
├── LICENSE                   # CC BY 4.0
├── studies/                  # Rapports OBS-001 à OBS-010
├── datasets/                 # Documentation par jeu de données
├── methodology/              # Collecte, limites, glossaire
└── .github/FUNDING.yml       # Soutien au projet
```

---

## Contribuer et contact

Ce dépôt est maintenu par l'équipe Holia. Pour signaler une erreur documentaire ou proposer une réutilisation :

- ouvrir une **issue** sur ce dépôt GitHub ;
- consulter l'Observatoire en ligne : [holia.me/observatoire](https://holia.me/observatoire).

Les propositions de nouvelles études ou d'éditions sont pilotées par le calendrier éditorial de l'Observatoire Holia.

---

## Glossaire rapide

| Terme | Définition courte |
|-------|-------------------|
| **Référentiel Holia** | Ensemble structuré des profils, métiers, sujets et territoires publiés sur la plateforme |
| **Snapshot** | Photographie du référentiel à une date d'arrêté |
| **Édition** | Période de publication (ex. 2026-05, 2026-06) |
| **Co-occurrence** | Présence conjointe de thèmes dans les déclarations observées (sans causalité) |

Définitions complètes : [`methodology/glossary.md`](./methodology/glossary.md)
