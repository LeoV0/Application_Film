# Application Film

Application web de découverte de films construite avec React et Vite, déployée sur Vercel.
Elle permet de parcourir un catalogue de films, d’afficher les détails d’un film et de rechercher rapidement un titre spécifique.

 **Démo en ligne** : https://application-film.vercel.app/

---

## Fonctionnalités

- Affichage d’une liste de films avec leur affiche, titre et note. 
- Détails pour chaque film (Langage, date de sortie, etc.). 
- Barre de recherche pour trouver un film par titre.
- Interface responsive adaptée aux écrans desktop et mobile.

---

## Stack technique

- **Framework** : React.  
- **Outil de build** : Vite.  
- **Langages** : JavaScript, HTML, CSS. 
- **Déploiement** : Vercel.

---

## Prérequis

- Node.js (version LTS récente, par exemple 18+).  
- npm, pnpm ou yarn installé sur la machine.

---

## Installation et lancement

1. Cloner le dépôt :
```
git clone https://github.com/LeoV0/Application_Film.git
cd ApplicationFilm
```

2. Installer les dépendances :
```
npm install
```

3. Lancer le serveur de développement :
```
npm run dev
```


4. Ouvrir le navigateur sur l’URL indiquée par Vite (généralement `http://localhost:5173`).

---

## Scripts disponibles

Les scripts principaux disponibles dans `package.json` sont :

- `npm run dev` : lance le serveur de développement Vite. 
- `npm run build` : génère la version de production. 
- `npm run preview` : prévisualise la build de production en local.  
- `npm run lint` : exécute ESLint sur le projet, si configuré.

---

## Structure du projet

- `public/` : Fichiers statiques publics. 
- `src/` : Code source de l’application React. 
- `index.html` : Point d’entrée HTML de l’application.

À l’intérieur de `src/`, la structure typique peut être :

- `src/components/` : Composants réutilisables (Cartes de film, Search, etc.). 
- `src/App` : Page principale (liste des films). 

Adapte cette section en fonction de l’organisation réelle de tes fichiers.

---

## API & données

L’application consomme une API de films (par exemple The Movie Database – TMDB) pour récupérer : 

- La liste des films affichés sur la page principale.  
- Les détails d’un film sélectionné.

Si tu utilises une clé API, configure une variable d’environnement Vite :

VITE_API_KEY=ta_cle_api_ici


Puis utilise-la dans ton code côté client via `import.meta.env.VITE_API_KEY`.

---

## Qualité du code

- ESLint est configuré pour appliquer des règles de qualité sur le code. 
- La configuration peut être étendue pour intégrer TypeScript et des règles supplémentaires si nécessaire.

---

## Déploiement

- Le projet est déployé sur **Vercel**, directement connecté au dépôt GitHub.
- Chaque push sur la branche principale déclenche une nouvelle build et mise en production.

---

## Pistes d’amélioration

- Filtrer les films par genre, popularité ou année de sortie.  
- Ajouter une pagination ou un infinite scroll.
- Mettre en place un système de favoris / watchlist pour les utilisateurs.

---

## Auteur

- **Léo** – Développeur front-end