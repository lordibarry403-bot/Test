# Snake – page de connexion

Petite page web en HTML, CSS et JavaScript pur (un seul fichier, aucune dépendance) : une page de connexion avec deux modes, et un jeu Snake.

## Fonctionnalités

- **Connexion en invité** : on peut jouer à Snake (clavier, boutons à l'écran ou glisser le doigt sur mobile). Le record est gardé dans le navigateur.
- **Connexion admin** avec le code `0000` : ouvre la « Page d'admin ».
- Thème clair ou sombre selon l'appareil, adapté au téléphone.

## Lancer en local

Ouvre simplement `index.html` dans ton navigateur (double-clic). Aucune installation.

## Mettre en ligne avec GitHub Pages

1. Crée un dépôt public sur [github.com](https://github.com/new), par exemple `snake-login`.
2. Envoie les fichiers : soit avec **Add file → Upload files** sur le site, soit avec git :

   ```bash
   git init
   git add .
   git commit -m "Première version"
   git branch -M main
   git remote add origin https://github.com/TON-PSEUDO/snake-login.git
   git push -u origin main
   ```

3. Dans le dépôt, va dans **Settings → Pages**, choisis **Deploy from a branch**, puis la branche `main` et le dossier `/ (root)`, et clique sur **Save**.
4. Après une ou deux minutes, le site est en ligne sur `https://TON-PSEUDO.github.io/snake-login/`.

## Structure

```
snake-login/
├── index.html   # toute l'application (page de connexion, Snake, page admin)
├── README.md
└── LICENSE
```

## Sécurité

Le code admin est vérifié dans le navigateur : il est visible dans le code source. C'est suffisant pour un projet ou un exercice, mais pas pour protéger de vraies données. Un vrai site doit vérifier le code côté serveur.

## Licence

MIT, voir le fichier `LICENSE`.
