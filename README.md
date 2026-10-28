# Batterie, mode d’emploi

Site d’une page : micro-cours de 15 minutes pour prolonger la durée de vie de la batterie d’un téléphone (iPhone et Android).

## Contenu

```
index.html               la page complète (HTML, CSS et JS intégrés)
assets/presentation.mp4  vidéo de présentation (H.264, 720p, 52 s)
assets/poster.jpg        image affichée avant la lecture de la vidéo
.nojekyll                indique à GitHub Pages de publier les fichiers tels quels
```

Aucune étape de compilation. Les polices viennent de Google Fonts.

## Publier sur GitHub Pages

1. Créez un dépôt sur GitHub, par exemple `batterie-mode-emploi`.
2. Ajoutez-y tous les fichiers de ce dossier à la racine, y compris `.nojekyll` et le dossier `assets`.
   - Depuis le site GitHub : **Add file → Upload files**, glissez les fichiers, puis **Commit changes**.
   - Ou en ligne de commande :
     ```
     git init
     git add .
     git commit -m "Premier envoi du site"
     git branch -M main
     git remote add origin https://github.com/VOTRE-COMPTE/batterie-mode-emploi.git
     git push -u origin main
     ```
3. Dans le dépôt, ouvrez **Settings → Pages**.
4. Sous **Build and deployment**, choisissez **Deploy from a branch**, puis la branche `main` et le dossier `/ (root)`. Cliquez sur **Save**.
5. Après une à deux minutes, le site est disponible à l’adresse
   `https://VOTRE-COMPTE.github.io/batterie-mode-emploi/`.

## Tester en local

Ouvrez `index.html` dans un navigateur, ou lancez un petit serveur depuis ce dossier :

```
python3 -m http.server 8000
```

puis ouvrez http://localhost:8000.

## Modifier

- Textes et quiz : tout est dans `index.html` (les questions des quiz sont dans l’objet `Q` du script en bas de page).
- Couleurs et polices : jetons CSS en haut de la balise `<style>` (`--mint`, `--amber`, `--night`…).
- Vidéo : remplacez `assets/presentation.mp4` par un fichier MP4 (H.264) du même nom.
