CAHIER DE REGISTRE — version GitHub Pages (l'application, gratuite)

⚠️ IMPORTANT : ce dossier contient seulement l'APPLICATION (ce que les gens installent).
La vérification des licences se fait sur un serveur à part (le paquet "cahier-registre-deno").
Il faut donc avoir déjà mis ce serveur en ligne sur Deno Deploy AVANT de faire les étapes ci-dessous.
(Si ce n'est pas encore fait, reprends le README du dossier cahier-registre-deno en premier.)

ÉTAPE 1 — Indiquer l'adresse de ton serveur
  Ouvre le fichier config.js et remplace :
      window.API_BASE = "https://TON-PROJET.deno.dev";
  par ta vraie adresse Deno Deploy (celle donnée après le déploiement), SANS "/" à la fin.

ÉTAPE 2 — Mettre en ligne sur GitHub Pages
  1. Va sur https://github.com et connecte-toi (même compte que pour Deno Deploy si tu veux).
  2. Crée un nouveau dépôt (New repository), par exemple "cahier-registre".
  3. Mets TOUS les fichiers de ce dossier à la racine de ce dépôt (index.html, config.js,
     manifest.json, sw.js, icon-180.png, icon-192.png, icon-512.png).
  4. Dans le dépôt : Settings > Pages.
  5. Sous "Build and deployment" > "Source", choisis "Deploy from a branch".
  6. Choisis la branche "main" et le dossier "/ (root)", puis Save.
  7. Attends 1 à 2 minutes. Le lien apparaît en haut de cette même page :
        https://ton-compte.github.io/cahier-registre/

C'EST CE LIEN QUE TU PARTAGES avec tes clients (WhatsApp, SMS...), pour qu'ils l'installent
sur leur écran d'accueil (Android : Chrome > ⋮ > Ajouter à l'écran d'accueil ;
iPhone : Safari > Partager > Sur l'écran d'accueil).

À SAVOIR
- GitHub Pages est gratuit et sans limite pratique pour ce genre d'app.
- Chaque mise à jour : remplace les fichiers dans le dépôt GitHub, Pages se met à jour
  automatiquement en 1-2 minutes.
- Le fichier config.js est le SEUL à modifier si l'adresse de ton serveur Deno change un jour.
