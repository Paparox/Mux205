# Site Pro Therma (plomberie · chauffage)

Site vitrine d'une seule page, sans serveur ni base de données : un fichier `index.html` + un dossier `photos/`.

## 1. Mettre les vraies infos

Ouvrir `index.html`, chercher `const CONFIG` (vers le bas du fichier) et remplacer :

| Champ | Exemple |
|---|---|
| `telephone` | `06 12 34 56 78` |
| `telephoneIntl` | `+33612345678` |
| `whatsapp` | `33612345678` (sans + ni espaces) |
| `email`, `ville`, `zone`, `zoneCourte`, `horaires` | |
| `facebook` | lien de la page Facebook |
| `messenger` | `https://m.me/nom-de-la-page` |
| `siret` | numéro SIRET |
| `demo` | `false` pour retirer le bandeau « Maquette » |

## 2. Ajouter les photos de chantier

1. Récupérer les photos depuis la page Facebook (ou directement sur le téléphone de l'artisan, meilleure qualité).
2. Les réduire à environ 1600 px de large (format JPG, ~300 Ko) et les déposer dans `photos/`.
3. Dans `index.html`, compléter la liste `const PHOTOS` :

```js
{ src: "photos/sdb-dupont.jpg", titre: "Salle de bain complète", lieu: "Douche à l'italienne", cat: "sdb" },
```

Catégories possibles : `sdb`, `chauffage`, `eau-chaude`, `depannage`.

## 3. Mettre en ligne (gratuit)

- **Netlify Drop** (le plus simple) : aller sur https://app.netlify.com/drop et glisser le dossier `pro-therma`. Le site est en ligne en 30 secondes avec une adresse en `.netlify.app`.
- **GitHub Pages** : possible aussi, idéalement depuis un dépôt dédié au site.
- **Nom de domaine** (`pro-therma.fr` par ex., environ 10 €/an chez OVH, Gandi, etc.) à relier ensuite à Netlify.

## À valider avec l'artisan

- Les textes des services (ne garder que ce qu'il fait vraiment).
- Mentions légales obligatoires pour un professionnel (raison sociale, SIRET, adresse, assurance décennale si travaux concernés).
- Vérifier sur https://data.inpi.fr que le nom « Pro Therma » ne pose pas de souci : « Protherm » est une marque de chaudières du groupe Vaillant.
