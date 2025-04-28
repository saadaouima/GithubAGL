Projet Floulou – Spécification


1.	Informations Générales 

• Nom du projet : Floulou 
• Auteurs : Nour El Houda Boussaidi, Meryem Saadaoui, Roua Labidi. 
• Date : 02/04/2025 

2.	Introduction au projet 

Floulou est une boutique en ligne spécialisée dans la vente de bouquets de fleurs. Le projet vise à offrir une expérience utilisateur fluide pour l'achat de bouquets prêts à livrer. 

Objectifs du projet
 
• Permettre aux clients de parcourir et d'acheter des bouquets de fleurs en ligne. 
• Gérer les commandes de manière efficace. 

Motivation 

Ce projet a été choisi pour répondre à la demande croissante des consommateurs pour des achats en ligne rapides et efficaces, tout en mettant en avant un marché éco-responsable et émotionnellement engageant.
 
3.	Spécifications du projet 

Notions de base et contraintes :
 	• Système de paiement sécurisé. 
• Interface utilisateur intuitive et responsive. 
       • Système de gestion des stocks et des livraisons. 
	
Acteurs et Fonctionnalités :

Acteurs : 
• Client : Achète des bouquets, suit ses commandes. 
• Administrateur : Gère les stocks et les commandes. 

Fonctionnalités principales : 

• Inscription et connexion des utilisateurs (Clients, Administrateurs). 
• Consultation du catalogue de bouquets. 
• Ajout de bouquets au panier 
• Passation de commande et paiement en ligne.
• Gestion des stocks et des produits (Admin).


## Diagrammes UML
Voici le diagramme de cas d'utilisation représentant les interactions des utilisateurs avec le système.

![Diagramme de cas d'utilisation](Diagrammes/diagramme%20de%20cas%20d'utilisation.png)

### Explication du Diagramme
Le diagramme présente les acteurs du système :

- **Utilisateur** : Peut rechercher des produits, passer des commandes, gérer son compte, etc.
- **Administrateur** : Gère les produits du système.
- **Système de paiement** : Valide les paiements par différentes méthodes (carte, MoneyGram, etc.).

Les lignes pointillées entre les cas d'utilisation et l'authentification indiquent que l'utilisateur doit être authentifié pour effectuer ces actions.

## ✅ Tests de Validation
## Table de Décision – Connexion de l'Utilisateur

| Pré-condition                  | 1  | 2  |
|--------------------------------|---|---|
| L’utilisateur a un compte      | F | T |
| **Post-condition**             |   |   |
| L’utilisateur est redirigé vers son tableau de bord | F | T |
| **Nombre de jeux de tests :**  | 2 


## Table de décision - consulter catalogue et ajouter au panier

| Pré-conditions                  | 1  | 2  | 3  | 4  |
|----------------------------------|---|---|---|---|
| L’utilisateur est connecté       | F | T | F | T |
| Des produits disponibles dans le catalogue | F | F | T | T |
| **Post-conditions**              |   |   |   |   |
| Produit ajouté au panier         | F | F |   | T |
| L’utilisateur consulte les détails du panier | F | F |   | T |
| **Nombre de jeux de tests**      | 4    
