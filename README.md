# BES Fiches atelier

Application de production de BOIS ECO-STYLE : saisie des meubles (placards, cuisines, meubles TV, meubles sur mesure), plan coté en temps réel, liste de débit, plans de découpe et fiche atelier imprimable en arabe et en français.

- Application : `index.html` (fichier unique, sans installation)
- Enregistrement des projets : navigateur (local) et Supabase (table `fiches_projets`)

## Relevé de chantier

- Page : `releve/` (bouton « Relevé de chantier » à l'accueil), croquis coté sur tablette
- Enregistrement : sur l'appareil (fonctionne sans internet) puis envoi automatique dans Supabase (table `releves`) dès que la connexion revient
- Chaque produit posé sur le croquis a un type (placard, cuisine, meuble TV, meuble). Le bouton « Fiche → » crée la fiche atelier avec le chantier et les mesures (cm convertis en mm), ou ouvre la fiche si elle existe déjà
- À l'accueil des fiches, la carte « Depuis un relevé de chantier » liste les relevés et leurs produits ; la fiche affiche un bandeau « Voir le croquis »
