# Administration du site FO IRP AUTO Gestion

## Installation
1. Conserver une copie de sauvegarde de votre dépôt actuel.
2. Dans GitHub, envoyer le contenu de ce dossier à la **racine** de la branche publiée par GitHub Pages. Les fichiers `.pages.yml`, `index.html`, le dossier `contenu` et le dossier `assets` doivent être au même niveau. Le fichier `.pages.yml` est masqué dans certains explorateurs : vérifier sa présence.
3. Vérifier que le site fonctionne après publication.
4. Aller sur https://app.pagescms.org/ et choisir la connexion GitHub.
5. Autoriser l'application Pages CMS **uniquement sur le dépôt FO**, puis choisir le dépôt et la **branche réellement publiée** par GitHub Pages.
6. Modifier une rubrique et enregistrer. Le CMS crée un commit GitHub ; GitHub Pages republie ensuite le site.

## Rubriques disponibles
- Accueil : titre, introduction et illustration.
- Bilan du mandat : titre, présentation et lien de la profession de foi.
- Cartes du bilan : intitulés, textes et pictogrammes.
- Nos engagements : titre et introduction.
- Cartes des engagements : listes de points.
- Vidéo : texte et chemin du fichier MP4 ou lien direct vers un fichier vidéo compatible navigateur.
- Présentation équipe : titre et introduction.
- Photos et candidats : nom, site, collège, mandat, photo.
- Appel au vote : titre et texte.

## Points importants
- Le logo d'origine est conservé dans `assets/LOGO_FO IRPAUTOGESTION.png`. Il n'est pas proposé à l'édition dans le CMS.
- **Ne jamais publier de jeton GitHub ni de mot de passe dans les fichiers du site.** La connexion se fait sur Pages CMS via GitHub.
- Pages CMS est un service externe : seuls les utilisateurs GitHub autorisés sur le dépôt et sur l'application doivent y accéder.
- Les photos et contenus de la version source sont conservés. Vérifier les droits à l'image et les informations nominatives avant diffusion publique.
- Les fichiers `contenu/*.json` doivent rester accessibles publiquement : ils ne doivent contenir aucune donnée confidentielle.
- Un aperçu local par ouverture directe de `index.html` en `file://` ne chargera pas les JSON. Tester sur GitHub Pages ou avec un serveur HTTP local (`python -m http.server 8000`).
- Les mises à jour du CMS ne s'affichent pas instantanément : attendre la fin du déploiement GitHub Pages.
- Le lien PDF présent dans le site source pointe vers `profession-de-foi.pdf` : ajouter ce fichier à la racine, ou renseigner un lien public dans le CMS.
- La vidéo MP4 n'était pas présente dans l'archive fournie. Ajouter la vidéo ou modifier son lien dans le CMS.
