# APPLICATION RESTAURANT

Il s'agit d'une application de gestion de restaurant simple, construite avec Express.js et MySQL.

## Table des matières

- [Aperçu](#aperçu)
- [Démarrage rapide](#démarrage-rapide)
- [Fonctionnalités](#fonctionnalités)
- [Exemples](#exemples)
- [Contribuer](#contribuer)
- [Licence](#licence)

## Aperçu

L'**APPLICATION RESTAURANT** est conçue pour gérer le menu et les catégories d'un restaurant. Elle vous permet d'effectuer des opérations telles que la visualisation des articles disponibles, l'ajout de nouvelles catégories et la suppression d'articles du menu.

## Démarrage rapide

Avant de commencer, assurez-vous d'avoir installé les prérequis suivants :

- Node.js et npm

Pour commencer avec l'**APPLICATION RESTAURANT**, suivez ces étapes simples :

1. Clonez le dépôt :

   ```bash
   git clone https://github.com/votre-nom-utilisateur/application-restaurant.git
   cd application-restaurant

# Fonctionnalités
- Visualiser tous les articles du menu disponibles
- Visualiser les articles du menu par catégories
- Ajouter de nouveaux articles au menu
- Supprimer des articles du menu
- Visualiser toutes les catégories disponibles
- Ajouter de nouvelles catégories
- ...

# Exemples 

#Exemple 1 : Visualisation de tous les articles du menu
Pour visualiser tous les articles du menu disponibles, utilisez l'endpoint suivant :


```
GET /items
````

#Exemple 2 : Ajout d'une nouvelle catégorie
Pour ajouter une nouvelle catégorie, utilisez l'endpoint suivant :

````
POST /category
````
Incluez le nom de la catégorie dans le corps de la requête.

#Exemple 3 : Suppression d'un article du menu
Pour supprimer un article du menu, utilisez l'endpoint suivant :

```
DELETE /delitems/:item_id
```
Remplacez :item_id par l'ID de l'article que vous souhaitez supprimer.

