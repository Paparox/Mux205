# Site Protherma – Joël Laugier, chauffagiste

Site vitrine d'une seule page aux couleurs de la carte de visite et du flyer Protherma.
Il n'y a ni serveur ni base de données : `index.html`, le logo dans `assets/` et les photos dans `photos/`.

## Ajouter les photos (sans toucher au code)

Déposer les fichiers dans le dossier `photos/` **avec exactement ces noms** :

| Fichier | Emplacement sur le site |
|---|---|
| `joel.jpg` | Photo de Joël devant son camion (encadré orange « Votre artisan ») |
| `chantier-01.jpg` | Remplacement chaudière fioul par PAC haute température R290 |
| `chantier-02.jpg` | Chaufferie : ballon d'eau chaude et module hydraulique |
| `chantier-03.jpg` | Climatisation murale dans un séjour |
| `chantier-04.jpg` | Console de climatisation sous fenêtre de toit |
| `chantier-05.jpg` | Unité extérieure de climatisation |
| `chantier-06.jpg` | Remplacement de chaudière |

Sur GitHub : ouvrir le dossier `photos`, puis **Add file → Upload files** et glisser les photos.
Tant qu'un fichier manque, la case affiche « Photo à venir ».

Pour ajouter d'autres chantiers ou changer les titres, modifier la liste `const PHOTOS` dans `index.html`.
Les catégories possibles sont `chaudiere`, `pac`, `clim` et `entretien`.
Format conseillé : JPG d'environ 1600 px de large et de moins de 500 Ko.

## Modifier les infos

Dans `index.html`, le bloc `const CONFIG` contient le téléphone, l'e-mail, l'adresse, les liens Facebook et Messenger et le SIRET.
Une fois le site validé, passer `demo` à `false` pour retirer le bandeau « Maquette ».

## Mettre en ligne avec GitHub Pages

Dans le dépôt, aller dans **Settings → Pages → Build and deployment**. Choisir la source « Deploy from a branch », la branche du site et le dossier `/ (root)`, puis cliquer sur **Save**.
Le site apparaît en 1 à 2 minutes.

## À valider avec Joël

- Le SIRET et les mentions légales, obligatoires pour un professionnel.
- La zone d'intervention précise.
- Le lien Messenger (`https://m.me/100085293757633`) : à tester depuis un téléphone.
- Le nom : « Protherma » est très proche de « Protherm », une marque de chaudières du groupe Vaillant. Il vaut mieux vérifier sur https://data.inpi.fr.
