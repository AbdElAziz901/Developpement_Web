# Developpement_Web
Application Web d’analyse et de prédiction AIS

---------------------------------Pour la connexion -------------------------------------------------------------------------------

lien : http://etu0311.projets.isen-ouest.info/pageaccueil.html
identifiant: etu0311
mot de passe : lnnkbaql

----------------------------------Présentation-------------------------------------------------------------------------------------

Notre **Projet Web** est une plateforme web interactive développée dans le cadre du projet ISEN 2025.  
Elle permet de :
- Visualiser des bateaux sur une carte interactive,
- Prédire leur type, leur trajectoire future, et leur cluster.

-----------------------Langages de programmation et outils utilisées----------------------------------------------------------------

- **Frontend** : HTML, CSS, JavaScript
- **Carte interactive** : Plotly
- **Backend** : PHP
- **Intelligence artificielle** : Scripts Python (classification, clustering, trajectoire)
- **Communication client-serveur** : AJAX + JSON

----------------------------------Fonctionnement du site----------------------------------------------------------------------------

 1. Accueil (`pageaccueil.html`)
Présentation du projet et de son objectif pédagogique.

2. Formulaire (`formulaire.html`)
Interface pour ajouter des données sur les bateaux.

3. Carte interactive (`visualisation.html`)
Affiche tous les bateaux sur une carte via Plotly :
- Les informations de chaque point de **bateau** sont disponible en passant la souris sur le point concerné.

--------------------------------------Prédiction avancée----------------------------------------------------------------------------

Depuis la carte ou un tableau :
1. **Sélectionnez un bateau** via un bouton radio.
2. Cliquez sur :
   - `Prédire le type` → Exécute un script Python type.py
   - `Prédire la trajectoire` → Exécute un script Python trajectoire.py
   - `Prédire les clusters` → Exécute un script Python cluster.py
3. Le site ouvre une **nouvelle page de résultats**.
4. Un **script Python est appelé côté serveur** (via PHP).
5. Le **résultat est renvoyé au navigateur** et affiché à l'utilisateur.

---------------------------------Organisation des fichiers à la base du serveur SSH ------------------------------------------------
/
├── css/

│   └── style_projet.css

│

├── img/

│   ├── logo.jpg

│   └── vue-aerienne-du-cargo-porte-conteneurs-en-mer.jpg
│
├── js/
│   ├── cluster.js
│   ├── etat.js
│   ├── predict_type.js
│   ├── trajectoire.js
│   └── visualisation.js
│
├── php/
│   ├── basededonnees.php
│   ├── cluster.php
│   ├── constantes.php
│   ├── etat.php
│   ├── formulaire.php
│   ├── predict_type.php
│   ├── trajectoire.php
│   └── visualisation.php
│
├── python/
│   ├── cluster.py
│   ├── predict_type.py
│   ├── trajectoire.py
│   └── type.py
│
├── cluster.html
├── formulaire.html
├── pageaccueil.html
├── predict_type.html
├── trajectoire.html
└── visualisation.html


---------------------------------------------------------------------------------------------------------------------------------------
