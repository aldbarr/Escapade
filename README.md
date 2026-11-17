# Escapade – idées de sorties en Suisse romande, Berne et Lucerne

Site statique (aucun build) : `index.html` + `activities.json`.

## Déployer sur Netlify depuis GitHub
1. Crée un dépôt GitHub et pousse ces fichiers à la racine.
2. Netlify → *Add new site* → *Import an existing project* → GitHub → choisis le dépôt.
3. Build command : (vide) · Publish directory : `.` → *Deploy*.

## Barre du bas et badge de l'hébergeur
Quand la page est affichée seule (Netlify, GitHub Pages…), la barre du bas est remontée de 56 px
pour ne pas être cachée par le badge de l'hébergeur. Pour ajuster : constante `NAV_LIFT` en haut du `<script>` dans `index.html`.

## Mettre à jour les activités
Toutes les données sont dans `activities.json` (`items[]`, `sources[]`, `updated`).
Un commit sur ce fichier redéploie automatiquement le site sur Netlify.
