# Domaine Joblot — suivi du domaine

Application web statique, hébergée par GitHub Pages. Le workflow publie le contenu de `index.html.html` sous le nom `index.html` ; le fichier source existant est ainsi conservé.

## Publier

1. Dans GitHub, ouvrez **Settings > Pages** et sélectionnez **GitHub Actions** comme source de publication.
2. Enregistrez puis poussez les changements sur la branche `main` (ou lancez manuellement **Publish on GitHub Pages** dans l’onglet **Actions**).
3. Attendez la réussite du workflow. L’application sera disponible à l’adresse `https://cotejeanne98-cmyk.github.io/app-domaine-Joblot/`.

## Données et sauvegardes

Les saisies sont enregistrées automatiquement dans le stockage local du navigateur. Elles restent sur cet appareil et dans ce navigateur ; GitHub Pages ne synchronise pas les appareils.

- À la première ouverture après la mise à jour du parcellaire, les unités de plantation sont ajoutées automatiquement dans **Vigne > Parcelles**, regroupées par secteur. Une migration distincte sépare Chanevarie et Clos Charlé des parcelles auxquelles elles étaient regroupées, en conservant les unités et leurs caractéristiques existantes, les identifiants des parcelles et les suivis historiques. Ces suivis ne sont pas réattribués. L’initialisation et la migration sont enregistrées avec les données et ne sont pas répétées aux ouvertures suivantes. Le bouton **✏️ Modifier** permet de modifier les caractéristiques d’une parcelle et de ses unités ; les changements sont sauvegardés avec les autres données.
- **Vigne > Réparations** permet de signaler, filtrer, modifier, terminer et supprimer des réparations. Les réparations sont sauvegardées avec les autres données et reliées aux parcelles par leur identifiant. Les formulaires tracteur proposent TXH, Geyer et Renault ; les anciennes valeurs de tracteur restent inchangées.
- Dans **Tracteur > Sessions**, chaque intervention peut associer plusieurs outils viticoles ou « Aucun outil ». L’historique affiche le tracteur et les outils ; les filtres par tracteur et par outil facilitent la recherche. Les interventions existantes sans outil restent valides et les outils sont inclus dans la sauvegarde JSON.
- Avant de quitter l’ancienne version, téléchargez une copie complète de vos données depuis **Plus > Exports**.
- Pour transférer les données, ouvrez **Plus > Exports** sur l’appareil source et téléchargez une sauvegarde JSON, puis restaurez ce fichier sur l’autre appareil. La restauration remplace les données de cet appareil après confirmation.
- Gardez une copie du fichier JSON en lieu sûr. Effacer les données du navigateur ou changer d’appareil peut autrement rendre les saisies locales inaccessibles.

## Faire évoluer l’application

Modifiez `index.html.html`, puis poussez les changements sur `main`. Le workflow GitHub Pages republiera automatiquement l’application.
