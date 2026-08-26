# Site Alron — mise en ligne gratuite sur GitHub Pages (version mobile)

Tous les fichiers de ce dossier sont **à plat, sans sous-dossier** — pensé pour
un upload en une seule fois depuis un téléphone, où il n'est pas possible de
glisser-déposer une arborescence de dossiers dans GitHub.

## 1. Il ne reste qu'une seule chose à compléter

Tout est déjà rempli (email, Facebook, Ko-fi, notice) sauf l'archive de
l'application elle-même :

| Élément | Repère dans le fichier | À faire |
|---|---|---|
| Archive de l'application | fichier `alron.zip` | à déposer une fois le build finalisé (voir `LISEZ-MOI-telechargement.txt`) |

Aucune autre modification n'est nécessaire dans `index.html`.

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

## 3. Ajouter le zip de l'application une fois prêt

Quand votre build sera peaufiné, revenez sur le dépôt et utilisez
**Add file > Upload files** pour déposer `alron.zip` à la racine, au même
niveau que les autres fichiers — le bouton "Télécharger l'archive" de la
page fonctionnera alors immédiatement, sans aucune autre modification.

## 4. Brancher un vrai nom de domaine plus tard (optionnel)

Si vous achetez un jour `alron.fr` (~5 à 15 €/an) :
1. Chez votre registrar, ajoutez un enregistrement DNS de type CNAME pointant
   `alron.fr` vers `VOTRE-PSEUDO.github.io`.
2. Dans **Settings > Pages** du dépôt GitHub, renseignez `alron.fr` dans le
   champ **Custom domain**.
3. Cochez **Enforce HTTPS** une fois le certificat généré (automatique).
