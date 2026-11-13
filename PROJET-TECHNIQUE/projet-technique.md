# Projet technique (Prototype CRUD)

Avant de commencer le développement du projet principal, j'ai réalisé un projet technique servant de prototype : une application web de **Restaurant / Food Delivery App** permettant aux propriétaires de restaurants de gérer plusieurs restaurants, leurs plats et leurs catégories alimentaires.

La plateforme permet à un propriétaire de gérer plusieurs restaurants indépendamment, en organisant les menus et les catégories de chaque restaurant.

## Fonctionnalités Clés

- **Restaurant Management :** Gestion de plusieurs restaurants par un seul propriétaire (CRUD complet).
- **Menu Items Management :** Ajouter, afficher, modifier et supprimer les plats de chaque restaurant.
- **Food Categories Management :** Ajouter, afficher, modifier et supprimer les catégories alimentaires.
- **Menu Organization :** Associer plusieurs catégories à un même plat et organiser les plats selon leurs catégories.

## Classes principales du modèle

- **RestaurantOwner :** Représente le propriétaire qui gère plusieurs restaurants.
- **Restaurant :** Représente un restaurant appartenant au propriétaire.
- **MenuItem (Plat) :** Représente les plats proposés dans un restaurant.
- **FoodCategory (Catégorie) :** Représente les différentes catégories utilisées pour organiser les plats.

## Relations principales

- **RestaurantOwner ↔ Restaurant :** Relation One-to-Many (un propriétaire peut gérer plusieurs restaurants).
- **Restaurant ↔ MenuItem :** Relation One-to-Many (un restaurant peut proposer plusieurs plats).
- **Restaurant ↔ FoodCategory :** Relation One-to-Many (un restaurant peut posséder plusieurs catégories).
- **MenuItem ↔ FoodCategory :** Relation Many-to-Many (un plat peut appartenir à plusieurs catégories et une catégorie peut contenir plusieurs plats).