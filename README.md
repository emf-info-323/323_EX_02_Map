<h1><code>Module 323</code> - Programmer de manière fonctionnelle</h1>

# 😅 Exercice 02 - Comprendre map()

## Objectifs

- Découvrir et bien comprendre cette incontournable méthode de programmation `map()`.

## Données

Les trois fichiers de données ci-dessous sont déjà chargés par le fichier HTML. Ces fichiers fournissent beaucoup d'informations sur :

- [ex02-data-motos.js](/src/ex02-data-motos.js) ➜ des marques de motos et des modèles de moto
- [ex02-data-villes.js](/src/ex02-data-villes.js) ➜ des villes, leur canton et nombre d'habitants
- [ex02-data-evaluations.js](/src/ex02-data-evaluations.js) ➜ des résultats d'évaluation de branches matu pour les apprentis de l'EMF

Ces informations sont directement utilisables via ces 3 constantes (`dataMotos`, `dataVilles` et `dataEvaluations`).

## Rapports à produire

Les rapports à produire :

- [M1 - La liste des marques de moto (pas de tri pour le moment)](#m1---la-liste-des-marques-de-moto-pas-de-tri-pour-le-moment)
- [M2 - Toutes les villes et leur canton (sans les habitants)](#m2---toutes-les-villes-et-leur-canton-sans-les-habitants)
- [M3 - La liste des "Prénom NOM" des apprentis évalués (pour le moment avec doublons et pas triés)](#m3---la-liste-des-prénom-nom-des-apprentis-évalués-pour-le-moment-avec-doublons-et-pas-triés)
- [M4 - La liste des cantons](#m4---la-liste-des-cantons)
- [M5 - La liste des branches évaluées](#m5---la-liste-des-branches-évaluées)
- [M6 - La liste des marques de moto et leurs modèles (pas de tri pour le moment)](#m6---la-liste-des-marques-de-moto-et-leurs-modèles)

## M1 - La liste des marques de moto (pas de tri pour le moment)

À partir des données disponibles (`dataMotos`), vous devez obtenir ceci en utilisant la fonction `map()`:

```json
[
   "Honda",
   "Yamaha",
   "Ducati",
   "BMW",
   "Harley-Davidson"
]
```

## M2 - Toutes les villes et leur canton (sans les habitants)

Toujours pas de tri pour le moment. À partir des données disponibles (`dataVilles`), vous devez obtenir ceci :

```json
[
   {
      "ville": "Fribourg",
      "canton": "FR"
   },
   {
      "ville": "Bulle",
      "canton": "FR"
   },
   {
      "ville": "Villars-sur-Glâne",
      "canton": "FR"
   },
   {
      "ville": "Riaz",
      "canton": "FR"
   },
   {
      "ville": "Lessoc",
      "canton": "FR"
   },
   {
      "ville": "Lausanne",
      "canton": "VD"
   },
   {
      "ville": "Yverdon-les-Bains",
      "canton": "VD"
   },
   {
      "ville": "Montreux",
      "canton": "VD"
   },
   {
      "ville": "Olten",
      "canton": "SO"
   },
   {
      "ville": "Solothurn",
      "canton": "SO"
   },
   {
      "ville": "Grenchen",
      "canton": "SO"
   },
   {
      "ville": "Sion",
      "canton": "VS"
   },
   {
      "ville": "Martigny",
      "canton": "VS"
   },
   {
      "ville": "Brig-Glis",
      "canton": "VS"
   },
   {
      "ville": "Zermatt",
      "canton": "VS"
   },
   {
      "ville": "Bern",
      "canton": "BE"
   },
   {
      "ville": "Biel/Bienne",
      "canton": "BE"
   },
   {
      "ville": "Thun",
      "canton": "BE"
   },
   {
      "ville": "Lully",
      "canton": "FR"
   },
   {
      "ville": "Lully",
      "canton": "VD"
   },
   {
      "ville": "Lully",
      "canton": "GE"
   },
   {
      "ville": "Villars",
      "canton": "VD"
   },
   {
      "ville": "Villars",
      "canton": "FR"
   }
]
```

## M3 - La liste des "Prénom NOM" des apprentis évalués (pour le moment avec doublons et pas triés)

Pour le moment avec doublons et toujours pas triés.

À partir des données disponibles (`dataEvaluations`), vous devez obtenir ceci :

```json
[
   "Claire VOYANTE",
   "Alain TERNET",
   "Guy TARISTE",
   "Claire VOYANTE",
   "John D'ŒUF",
   "Alain TERRIEUR",
   "Alain TERRIEUR",
   "Eddy FICE",
   "Remy NISSENS",
   "Alex TERRIEUR",
   "Alain TERNET",
  ...
  ...
  ...
   "Remy NISSENS",
   "Eddy FICE",
   "Alain TERNET",
   "Claire VOYANTE",
   "Mac HARONI",
   "Alex TERRIEUR",
   "Théo RIQUE",
   "John D'ŒUF",
   "Alex TERRIEUR",
   "Claire VOYANTE",
   "Alain TERRIEUR"
]
```

## M4 - La liste des cantons

Pour le moment avec doublons et toujours pas triés.

À partir des données  disponibles (`dataVilles`), vous devez obtenir ceci :

```json
[
   "FR",
   "FR",
   "FR",
   "FR",
   "FR",
   "VD",
   "VD",
   "VD",
   "SO",
   "SO",
   "SO",
   "VS",
   "VS",
   "VS",
   "VS",
   "BE",
   "BE",
   "BE",
   "FR",
   "VD",
   "GE",
   "VD",
   "FR"
]
```

## M5 - La liste des branches évaluées

Pour le moment avec doublons et toujours pas triés.

À partir des données disponibles (`dataEvaluations`), vous devez obtenir ceci :

```json
[
   "Physique",
   "Français",
   "Allemand",
   "Maths",
   "Anglais",
   "Physique",
   "Physique",
   "Maths",
   "Histoire",
   "Maths",
   "Allemand",
   "Physique",
   "Histoire",
   "Histoire",
   "Physique",
   "Français",
   "Français",

   ...
   ...
   ...

   "Géographie",
   "Physique",
   "Français",
   "Allemand",
   "Français",
   "Allemand",
   "Maths",
   "Géographie",
   "Physique",
   "Physique",
   "Maths",
   "Géographie",
   "Histoire"
]
```

## M6 - La liste des marques de moto et leurs modèles

Pour le moment toujours pas de tri.

À partir des données disponibles (`dataMotos`), vous devez obtenir ceci en utilisant la fonction `map()`:

```json
[   {
      "marque": "Honda",
      "modeles": [
         "CB750 Four",
         "Africa Twin CRF1100L",
         "CBR1000RR Fireblade",
         "Gold Wing"
      ]
   },
   {
      "marque": "Yamaha",
      "modeles": [
         "YZF-R1",
         "MT-09",
         "XT500",
         "Ténéré 700"
      ]
   },
   {
      "marque": "Ducati",
      "modeles": [
         "Panigale V4",
         "Monster 1200",
         "Scrambler Icon",
         "916"
      ]
   },
   {
      "marque": "BMW",
      "modeles": [
         "R1250GS",
         "S1000RR",
         "K1600GTL",
         "R nineT"
      ]
   },
   {
      "marque": "Harley-Davidson",
      "modeles": [
         "Sportster 883",
         "Fat Boy 114",
         "Electra Glide",
         "Street Glide Special"
      ]
   }
]
```

---

<img src="res/EMF_logo_RVB_Info_long.png" width="25%" style="margin-left:-20px;">
