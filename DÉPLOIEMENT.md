# Guide de Déploiement sur GitHub Pages

Ce guide vous explique comment mettre votre journal **Info connectée** en ligne gratuitement grâce à GitHub Pages.

## 1. Créer un dépôt sur GitHub
1. Connectez-vous à votre compte [GitHub](https://github.com/).
2. Créez un nouveau dépôt (Repository) nommé `info-connectee`.
3. Gardez-le en **Public**.
4. Ne cochez **aucune** case (pas de README, pas de .gitignore).

## 2. Relier votre projet local à GitHub
Ouvrez un terminal dans le dossier du projet et lancez ces commandes :

```bash
git init
git add .
git commit -m "Premier commit : Journal Info connectée"
git branch -M main
git remote add origin https://github.com/VOTRE_NOM_UTILISATEUR/info-connectee.git
git push -u origin main
```
*(Remplacez `VOTRE_NOM_UTILISATEUR` par votre vrai pseudo GitHub)*.

## 3. Configurer GitHub Pages
1. Sur la page de votre dépôt GitHub, allez dans l'onglet **Settings** (Paramètres).
2. Dans le menu de gauche, cliquez sur **Pages**.
3. Sous la section **Build and deployment** > **Source**, choisissez **GitHub Actions**.

## 4. C'est en ligne !
Grâce au fichier que j'ai créé dans `.github/workflows/hugo.yml`, GitHub va automatiquement construire et publier votre site à chaque fois que vous ferez un `git push`.

Votre site sera visible à l'adresse suivante :
`https://VOTRE_NOM_UTILISATEUR.github.io/info-connectee/`

## 💡 Notes importantes
- **baseURL** : J'ai configuré le déploiement pour qu'il détecte automatiquement votre URL. Vous n'avez rien à modifier dans `hugo.toml`.
- **Mises à jour** : Pour publier de nouveaux articles, il suffira de faire :
  ```bash
  git add .
  git commit -m "Ajout d'un nouvel article"
  git push
  ```
