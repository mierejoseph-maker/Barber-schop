# Barber-schop
 
Site vitrine statique (HTML/CSS) pour un salon de coiffure fictif (Barber schop) basé à Brazzaville, Congo.
 
## 1. Aperçu du projet
 
| | |
|---|---|
| Pages | 3 (Accueil, Services, Contact) |
| Techniques | HTML5 sémantique, CSS3 (Flexbox + Grid), SVG inline |
| Responsive | 2 points de rupture : 641px et 1024px |
 
## 2. Structure des fichiers
 
```
  Barber schop/
├── index.html       # Page d'accueil (hero, présentation, chiffres clés)
├── services.html     # Page services (4 prestations + déroulement de visite)
├── contact.html     # Page contact (coordonnées + formulaire)
├── style.css         # Feuille de style unique, partagée par les 3 pages
└── README.md         # Ce fichier
```

 
## 3. Installation et lancement en local
 
Aucune installation n'est nécessaire, ce site est 100% statique.
 
**Ouverture directe**
Double-cliquer sur `index.html`, il s'ouvre dans le navigateur par défaut.
 
## 4. Personnalisation — ce qu'il faut remplacer avant mise en ligne
 
Toutes les informations ci-dessous sont **fictives** et doivent être remplacées par les vraies données de l'entreprise :
 
- **Nom du salon** : « Barber schop » apparaît dans `<title>`, dans le logo (`.brand`) et dans le pied de page des 3 fichiers HTML.
- **Adresse** : « Rond point otina, Nkombo, Brazzaville » — présente dans le pied de page (3 fichiers) et dans `contact.html`.
- **Téléphone** : « +242 05 589 66 63 » — pied de page + `contact.html`.
- **E-mail** : « barberschop@gmail.com » — pied de page, `contact.html`, et attribut `action="mailto:..."` du formulaire.
- **Horaires** : dans `contact.html`, section coordonnées.
- **Tarifs des services** : Dans `services.html` (`<p class="price">`).
Astuce : faire une recherche du texte `barberschop@gmail.com` et `+242 05 589 66 63` dans les 3 fichiers HTML pour être sûr de ne rien oublier.
 
 
## 5. Système de couleurs et typographies
 
Toutes les valeurs sont centralisées en haut de `style.css`, dans le bloc `:root`, pour faciliter les changements de charte graphique :
 
```css
--ink: #21121f;          /* Texte principal */
--aubergine: #3c1f42;    /* Couleur de marque principale */
--gold: #c99a3b;         /* Accent doré */
--emerald: #1f6f54;      /* Accent vert */
--cream: #f6f1e3;        /* Fond de page */
```
 
## 6. Responsive design
 
Le site est conçu mobile-first, avec 2 points de rupture définis dans `style.css` :
 
| Breakpoint | Largeur | Changements principaux |
|---|---|---|
| Mobile (par défaut) | < 641px | Une seule colonne, navigation compacte |
| Tablette | ≥ 641px | Cartes services sur 2 colonnes, formulaire sur 2 colonnes |
| Desktop | ≥ 1024px | Cartes services sur 4 colonnes, hero en 2 colonnes, page contact en 2 colonnes |
