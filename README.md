# 🎰 Roulette Picture Bets — Entraîneur

Application web pour s'entraîner aux **picture bets** de la roulette : ces dispositions visuelles de jetons que les croupiers reconnaissent instantanément pour annoncer un paiement sans calcul mental.

Pose des jetons sur le tapis, choisis le numéro gagnant, et l'app te détaille la composition du paiement (sixaine, transversale, carré, cheval, plein) avec le total.

## 🚀 Lancer l'application

### Option 1 — En local
Télécharge `index.html` et ouvre-le dans n'importe quel navigateur. C'est tout. Aucune dépendance, aucun build.

### Option 2 — GitHub Pages
Active **GitHub Pages** dans les *Settings* du dépôt (branche `main`, dossier `/root`). L'app sera servie à `https://<ton-pseudo>.github.io/roulette-picture-bets/`.

## 🎯 Comment ça marche

| Action | Résultat |
|---|---|
| Clic gauche sur le tapis | Pose un jeton à la position la plus proche (plein, cheval, carré, transversale ou sixaine selon la zone) |
| Clic droit sur un jeton | Retire un jeton |
| Bouton **Annuler** | Retire le dernier jeton posé |
| Bouton **Tout effacer** | Remet le tapis à zéro |
| Grille 0–36 à droite | Sélectionne le numéro gagnant |
| Bouton **Afficher les positions** | Révèle des marqueurs subtils pour repérer les positions de chaque type de mise |

Quand tu choisis un numéro gagnant, seuls les jetons qui le couvrent contribuent au total. La composition s'affiche groupée par type de mise (ex. *2 carrés × 8 = 16*, *1 cheval × 17 = 17*) avec le total en grand.

## 📐 Multiplicateurs (mises à l'intérieur)

| Mise | Numéros couverts | Multiplicateur |
|---|---|---|
| Plein | 1 | ×35 |
| Cheval | 2 | ×17 |
| Carré | 4 | ×8 |
| Transversale | 3 | ×11 |
| Sixaine | 6 | ×5 |

## 📋 Picture bets classiques

Quelques compositions de référence intégrées dans l'app :

| Montant | Composition |
|---|---|
| 21 | 2 sixaines + 1 transversale |
| 25 | 1 carré + 1 cheval |
| 33 | 2 carrés + 1 cheval |
| 42 | 1 carré + 2 chevaux |
| 51 | 2 carrés + 1 plein |
| 52 | 1 cheval + 1 plein |
| 60 | 1 carré + 1 cheval + 1 plein |
| 67 | 4 carrés + 1 plein |
| 68 | 2 carrés + 1 cheval + 1 plein |
| 69 | 2 chevaux + 1 plein |
| 77 | 1 carré + 2 chevaux + 1 plein |
| 86 | 3 chevaux + 1 plein |
| 100 | 4 carrés + 4 chevaux |
| 101 | 4 carrés + 2 chevaux + 1 plein |
| 102 | 2 carrés + 3 chevaux + 1 plein |
| 103 | 4 chevaux + 1 plein |
| 116 | 2 transversales + 1 carré + 3 chevaux + 1 plein |

## 🧱 Stack

Une seule page HTML. Vanilla JS + SVG. Aucun framework, aucune dépendance npm. Police Google Fonts (Playfair Display, Manrope, JetBrains Mono).

## 📂 Structure

```
roulette-picture-bets/
├── index.html      # L'application complète (HTML + CSS + JS + SVG)
├── README.md
├── LICENSE
└── .gitignore
```

## 🪪 Licence

MIT — voir [LICENSE](./LICENSE).
