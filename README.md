# Meme Generator - Application Web de création de mèmes personnalisés

## Présentation du projet

Ce projet est une application web complète permettant de créer des mèmes de manière totalement personnalisée. L'utilisateur peut importer plusieurs images, ajouter du texte librement, ajuster les couleurs, la taille, la position et générer un rendu final téléchargeable.

Le projet est structuré en deux parties : un frontend en React et un backend en Express.

## Technologies utilisées

* **React** : pour la création de l'interface utilisateur, avec gestion des états, composants dynamiques, et manipulation d’images via canvas.
* **Express.js** : serveur backend pour gérer les routes API, le traitement des fichiers et l’interfaçage avec la base de données.
* **MongoDB** : utilisée pour stocker les memes.
* **Cloudinary** : utilisé pour le stockage, l’optimisation et la livraison rapide des fichiers image.
* **Tailwind CSS** : utilisée pour le design.
* **HTML5 Canvas** : utilisé pour dessiner dynamiquement les mèmes, superposer des textes, ajuster l’affichage et exporter l’image finale.

## Fonctionnalités principales

* Importation d'une ou plusieurs images (jusqu’à 4 dans l’interface de base, sans limite en mode personnalisé).
* Modes d’affichage : horizontal, vertical, grille 2x2.
* Ajout de texte personnalisable (haut, bas, ou position libre par clic).
* Modification dynamique du texte : couleur, opacité, fond.
* Manipulation libre de chaque élément (drag, resize, delete).
* Aperçu en temps réel et génération d’un fichier image téléchargeable.
* Consultation des images suavegarder via gallery ou peut télecharger, partager et supprimer un memes.
* Possibilité de partager vos création directement depuis l'interface.
* Interface responsive et accessible sur tous types d’écrans.

## Fonctionnalité avancée : création totalement personnalisée

L’utilisateur peut passer en mode de création avancée lui permettant :

* d’ajouter autant de textes qu’il le souhaite, positionnés librement sur l’image,
* d’ajouter plusieurs images et les réorganiser comme il le souhaite,
* d’éditer chaque élément indépendamment (taille, couleur, rotation, suppression),
* d’avoir un contrôle total sur le rendu final, y compris les overlays, les fonds et l'ordre des calques.

## Lancement du projet en local

### Prérequis

* Node.js (v16 ou supérieur)

### Installation

1. Cloner le dépôt :

```bash
git clone https://github.com/KCaziz/meme-generator.git
cd meme-generator
```

2. Installer les dépendances :

```bash
cd client
npm install
cd ../server
npm install
```

3. Configurer les variables d’environnement :
   Pas besoin de configurer vos variables d'environnement utiliser les miennes
4. Lancer le backend :

```bash
cd server
node server.js
```

5. Lancer le frontend :

```bash
cd client
npm start
```

L’application sera disponible sur `http://localhost:3000` et le backend sur `http://localhost:5000`.

### Mode production (local)

Depuis le dossier `client` :

```bash
npm run prod
```

Cela build l’application React et la sert en production locale via `serve`.

## Déploiement

Le projet a été déployé sur Render (avec une autre config pour un fonctionnement stable)

https://memes-front.onrender.com/

## Structure du projet

```
/
├── client/         # Frontend React
│   ├── public/
│   ├── src/
│   └── ...
│
├── server/         # Backend Express
│   ├── controllers/
│   ├── routes/
│   └── server.js
│
└── README.md
```

## Auteurs et crédits

Ce projet a été développé dans une logique d'apprentissage, et dans le cadre d'un projet pour l'école SUPINFO.
Merci aux bibliothèques open-source et services cloud gratuits utilisés.
