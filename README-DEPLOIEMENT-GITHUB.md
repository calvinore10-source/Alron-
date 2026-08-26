# Site Alron — mise en ligne gratuite sur GitHub Pages (version mobile)

Tous les fichiers de ce dossier sont **à plat, sans sous-dossier** — pensé pour
un upload en une seule fois depuis un téléphone, où il n'est pas possible de
glisser-déposer une arborescence de dossiers dans GitHub.

## 1. À compléter avant publication

Le site est fonctionnel mais contient encore des **placeholders** à remplacer
dans `index.html` :

| Élément | Repère dans le fichier | À remplacer par |
|---|---|---|
| Email de contact | `votre-email@exemple.fr` (2 occurrences) | votre adresse réelle |
| Lien Facebook | `VotrePageAlron` (2 occurrences) | l'URL de votre page |
| Lien Ko-fi | `VotrePseudoKofi` (2 occurrences) | votre lien Ko-fi |
| Archive de l'application | fichier `alron.zip` | à déposer vous-même (voir `LISEZ-MOI-telechargement.txt`) |
| Notice utilisateur | fichier `notice-alron.pdf` | à déposer vous-même (voir `LISEZ-MOI-notice.txt`) |

Ces modifications peuvent se faire directement dans l'éditeur de fichier
intégré à GitHub (ouvrez `index.html` dans le dépôt, appuyez sur le crayon
"Edit", cherchez le texte à remplacer, puis "Commit changes").

## 2. Publier sur GitHub Pages (gratuit, depuis un téléphone)

1. Créez un compte gratuit sur https://github.com si vous n'en avez pas.
2. **New repository**, nommez-le par exemple `alron`, cochez **Public**,
   ne cochez aucune option d'initialisation (pas de README, pas de licence).
3. Sur la page du dépôt fraîchement créé, cherchez le lien
   **"téléchargez un fichier existant"** (ou **Add file > Upload files**).
4. Sélectionnez **tous les fichiers de ce dossier en une seule fois**
   (tous à la racine, aucun dossier à gérer). Sur Android, la plupart des
   gestionnaires de fichiers permettent une sélection multiple.
5. Descendez en bas de page et validez avec **"Commit changes"**.
6. Allez dans **Settings > Pages** (menu du dépôt).
7. Sous **Build and deployment > Source**, choisissez **Deploy from a
   branch**, branche `main`, dossier `/ (root)`, puis **Save**.
8. Patientez 1 à 2 minutes : l'URL du site s'affiche en haut de cette page,
   du type `https://VOTRE-PSEUDO.github.io/alron/`.

Chaque nouvelle modification (via l'éditeur GitHub ou un nouvel upload)
republie le site automatiquement en quelques dizaines de secondes.

## 3. Ajouter les fichiers manquants plus tard

Pour déposer votre notice PDF ou le zip de l'exe compilé plus tard, revenez
sur le dépôt et utilisez à nouveau **Add file > Upload files** — les
nouveaux fichiers `notice-alron.pdf` et `alron.zip` viendront simplement
s'ajouter à la racine, au même niveau que les autres.

## 4. Brancher un vrai nom de domaine plus tard (optionnel)

Si vous achetez un jour `alron.fr` (~5 à 15 €/an) :
1. Chez votre registrar, ajoutez un enregistrement DNS de type CNAME pointant
   `alron.fr` vers `VOTRE-PSEUDO.github.io`.
2. Dans **Settings > Pages** du dépôt GitHub, renseignez `alron.fr` dans le
   champ **Custom domain**.
3. Cochez **Enforce HTTPS** une fois le certificat généré (automatique).
