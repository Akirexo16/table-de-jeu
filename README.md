# Table de Jeu

Un petit site statique pour jouer au **blackjack** (et bientôt au **poker**) avec des jetons virtuels — aucun argent réel n'est jamais en jeu.

## Structure

```
├── index.html        page d'accueil avec le menu des jeux
├── blackjack.html     table de blackjack jouable
├── poker.html          page "bientôt disponible"
├── css/style.css       feuille de style commune
└── js/blackjack.js     logique du jeu de blackjack
```

## Lancer en local

Aucune dépendance ni build : ouvrez simplement `index.html` dans un navigateur,
ou lancez un petit serveur local, par exemple :

```bash
python3 -m http.server 8000
```

puis rendez-vous sur `http://localhost:8000`.

## Héberger sur GitHub Pages

1. Poussez ce dossier dans un dépôt GitHub.
2. Dans les réglages du dépôt, ouvrez **Settings → Pages**.
3. Choisissez la branche `main` (ou `master`) et le dossier `/ (root)`.
4. Le site sera publié à une adresse du type
   `https://votre-utilisateur.github.io/nom-du-depot/`.

## Fonctionnement du blackjack

- Le joueur commence avec 1000 jetons (solde sauvegardé dans le navigateur via `localStorage`).
- Règles classiques : blackjack naturel payé 3 pour 2, le croupier tire jusqu'à 17.
- Boutons : Distribuer, Tirer, Rester, Doubler.

## À venir

Une table de poker (Texas Hold'em contre des bots) sur `poker.html`.
