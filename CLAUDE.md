# Site de Lucile Sallenave, sophrologue — contexte du projet

Projet réalisé par l'Agence Lemonnier (Julien Vattier). Julien n'aime pas les interfaces techniques : c'est Claude qui fait les modifications, les enregistre (commit) et les met en ligne (push sur `main`). Réponses courtes et en français.

## Le site
- Site vitrine statique (HTML/CSS, sans outil de build), hébergé sur GitHub Pages depuis `main` : https://lucilesallenave.github.io/site-sophrologue/
- `index.html` (accueil), `mentions-legales.html`, `assets/style.css` (couleurs en variables en haut), `assets/favicon.svg`.
- Ambiance « Aube » : fond pêche #F7EEE8, encre #2E1F26, accent prune #6B3E57 ; titres Instrument Serif, texte Work Sans.
- Lucile est itinérante : séances en visio partout en France + à domicile (elle se déplace).

## Tarifs affichés
- Visio : première séance (1 h 15) 60 €, séance 50 €, forfait 5 séances 225 €, forfait 10 séances 430 €.
- Domicile : première séance (1 h 15) 60 €, séance 55 €, forfait 5 séances 250 €, forfait 10 séances 480 €.
- Sous chaque grille : « En moyenne, entre 15 € et 60 € remboursés par séance par votre mutuelle, selon votre contrat. »
- La Sécurité sociale ne rembourse pas la sophrologie (Lucile n'est pas médecin) : ne jamais l'écrire.

## Lieu d'activité modifiable par Lucile
- Google Sheet « Site Lucile – Où suis-je en ce moment » (Drive de Julien, partagé en modification avec Lucile, lecture publique par lien) : id `1NQDHjcdmUVDTtw9oaEPwlKMmxpvx9TxvbeEdoQunwtU`, onglet `Lieu`.
  - B1 = lieu actuel (texte libre), B2 = séances à domicile OUI/NON.
- `index.html` lit B1:B2 via l'URL gviz CSV ; éléments `[data-lieu]` (texte du lieu) et `[data-domicile]` (masqués si NON). Texte par défaut : « Seine-et-Marne (77) ».
- Fonctionnement à vérifier une fois le site en ligne (non testable depuis le cloud).

## Reste à faire (éléments entre crochets dans le site)
- Zone de déplacement et frais de déplacement.
- Parcours / formation de Lucile (+ certification et syndicat, utile pour les mutuelles).
- Photos (accueil, portrait, séance) → `assets/photos/`.
- Conditions d'annulation, nombre de séances conseillé (FAQ).
- Outil de réservation (Calendly ou autre) : brancher les boutons « Réserver ».
- Thèmes de la section « Pour quoi venir me voir ? » à valider.
- Plus tard : nom de domaine (puis « Enforce HTTPS »), 2FA sur les comptes GitHub et Google.
