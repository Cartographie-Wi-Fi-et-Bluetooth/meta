# Présentation du projet cartographie wifi et bluetooth

## Sommaire
1. Introduction
  1. Description
  2. Équipe
  2. Développement

2. Analyse des besoins
  1. Description du sujet et du contexte
  2. Cahier des charges
  3. Liste des fonctionnalités de l'application

3. Plan de charge
  1. Plan de charge
  2. Suivi d'activités

4.Planning prévisionnel

5. Conception préliminaire
  1. Première version du plan du rapport final

6. Conclusion
  1. Récapitulatif des résultats obtenus dans le livrable
  2. Perspectives pour la suite du projet



## Introduction

### Description
Dans le cadre d'un projet scolaire en informatique à l'école Télécom SudParis, nous réaliserons une application mobile permettant la localisation d'appareil Wi-Fi et Bluetooth.

### Équipe
* Augustin Bresset  
* Pierre Chambet
* Guillaume De Terline
* Zacharie March

#### Encadrant

Rémy Grünblatt

## Développement

Trois pôles ont étaient retenues pour le développement de l'application :

#### Frontend
Création de la carte
* Leaflet
* React
* geodjango

#### Application mobile
Développement de l'application pour smartphone sous android.
* Kotlin
* Android Studio

#### Backend
Traitement des données, communication avec les serveurs.
* Django (Python)

#### Supplémentaires
Déploiement des APIs à l'aide de REST.
Développement de l'algorithme de géolocalisation.

## Analyse des besoins

### Description du sujet et du contexte

### Cahier des charges

#### Backend

Établir un serveur qui recueille les données transmises par l’application mobile.


* Etablissement du modèle de la base de données avec django : Les modèles de base de données avec Django sont des classes python. Ces classes définissent les champs de chaque table.

* Préciser les informations à recueillir :
    1. le signal bluetooth
    2. le signal WI-FI
    
    Cette étape prend forme lors de la déclaration des champs. Les signaux recueillis ont plusieurs attributs, il faut donc choisir ceux d'intérêts. Par exemple, les informations utiles peuvent être la puissance du signal reçu et l’heure à laquelle ce signal est reçu.

* Mettre en relation les classes avec les clés étrangères : Afin de pouvoir comparer et utiliser les deux sources d’informations (bluetooth/WIFI).

* Traitement des données : Pour pouvoir employer les données, il faut tout d'abord les traiter dans un format adapté. Il nous faut également des méthodes de classe afin d’exploiter ces données. On peut alors effectuer des opérations, des calculs sur ces données.

* Modifier la base de données : Une fois les résultats obtenus, il faut effectuer une migration django afin de mettre à jour les modèles

* Envoyer les résultats : Une fois le traitement des données effectué, il faut les envoyer



#### Développement mobile : Kotlin sur Android Studio


Présenter une application mobile développée sur Android affichant une carte repérant les positions des différents appareils WIFI/Bluetooth émettant un signal perceptible par le smartphone.


* Conception de l’interface utilisateur de l’application via l’éditeur d’interface d’Android Studio et en utilisant la carte après réalisation de la partie Frontend.

* Ajout du code Kotlin permettant d’établir l’échange de données avec le serveur (Backend), et d’indiquer les points WIFI et Bluetooth à proximité. Les données en question concernent les puissances des signaux WIFI et Bluetooth reçus par le smartphone support de l’application.

* Test et débogage de l’application.


#### Frontend


Réalisation d’une carte où sont pointés les localisations des appareils WIFI/Bluetooth. On peut voir cette carte sur l’application mobile développée.


* Utilisation de la bibliothèque Leaflet pour créer une carte interactive à mettre sur l’application mobile.

* Pointer les localisations des différents appareils WIFI/Bluetooth sur la carte.

* (Utilisation de la bibliothèque React pour créer une interface utilisateur interactive.)

* Éventuellement s’il nous reste du temps pointer la position de l’utilisateur en fonction de sa proximité aux différents points WIFI par triangulation.

### Liste des fonctionnalités de l'application
#### Affichage des points d'accès sur une carte interactive
Les points d'accès seront représentés par des marqueurs sur la carte et les utilisateurs pourront interagir avec eux en cliquant dessus.
#### Filtrage des résultats
Les utilisateurs pourront filtrer les résultats en fonction de leur position, de la puissance du signal reçu et d'autres critères pertinents.
####Ajout de nouveaux points d'accès
Les utilisateurs pourront ajouter de nouveaux points d'accès à la carte en fournissant les informations pertinentes, telles que l'emplacement et la puissance du signal reçu.
####Bouton pour rafraîchir la page

## Plan de charge


|                                                  	| Plan de charges prévisionnel |             	|                         	|                           	|            	|            	|
|------------------------------------------------------|------------------------------|-----------------|-----------------------------|-------------------------------|----------------|----------------|
|                                                  	|                          	|             	| Charge en heure/participant |                           	|            	|            	|
| Description de l'activité                        	| Charge en %              	| Charge en heure | Augustin BRESSET        	| Guillaume MACQUART DE TERLINE | Pierre CHAMBET | Zacharie MARCH |
| Total                                            	| 100                      	| 200         	| 50                      	| 50                        	| 50         	| 50         	|
| Gestion de projet                                	| 24                       	| 48          	| 12                      	| 12                        	| 12         	| 12         	|
| Réunion de lancement                             	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Planning prévisionnel et Suivi des activités     	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Réunions de suivi                                	| 12                       	| 24          	| 6                       	| 6                         	| 6          	| 6          	|
| Rédaction                                        	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
| Outil collaboratifs (Google drive, Github)       	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
| Spécification                                    	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
| Définition des fonctionnalités                   	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
| Conception préliminaire                          	| 14                       	| 28          	| 7                       	| 7                         	| 7          	| 7          	|
| Définition des données                           	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Définition des formats des données               	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Définition des modèles des données               	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Définir les vues sur django                      	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Créer des templates pour la présentation des données | 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Mise en place des protocoles de triangulation    	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
| Conception détaillé                              	| 18                       	| 36          	| 9                       	| 9                         	| 9          	| 9          	|
| Auto-formation                                   	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
| Définition des classes (Kotlin, JavaScript)      	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
| Définition des clés étrangères (Django)          	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Défintion des méthodes (Kotlin, JavaScript)      	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
| Migration Django                                 	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Configurer les URL                               	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
| Codage                                           	| 24                       	| 48          	| 12                      	| 12                        	| 12         	| 12         	|
| Codage des classes                               	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Codage des clés étrangères                       	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Codage des méthodes                              	| 8                        	| 16          	| 4                       	| 4                         	| 4          	| 4          	|
| Implémenter la triangulation                     	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
| Codage de la carte avec la bibliothèque Leaflet  	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Codage des tests unitaires                       	| 6                        	| 12          	| 3                       	| 3                         	| 3          	| 3          	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
| Intégration                                      	| 8                        	| 16          	| 4                       	| 4                         	| 4          	| 4          	|
| Intégration des modules                          	| 4                        	| 8           	| 2                       	| 2                         	| 2          	| 2          	|
| Test d'intégration                               	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
| Test de l'application                            	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
|                                                  	|                          	|             	|                         	|                           	|            	|            	|
| Soutenance                                       	| 8                        	| 16          	| 4                       	| 4                         	| 4          	| 4          	|
| Préparation de la soutenance                     	| 6                        	| 12          	| 3                       	| 3                         	| 3          	| 3          	|
| Soutenance                                       	| 2                        	| 4           	| 1                       	| 1                         	| 1          	| 1          	|



### Suivi des activités

|                                          	| Suivi d'activité |             	|                         	|                           	|            	|            	|
|----------------------------------------------|------------------|-----------------|-----------------------------|-------------------------------|----------------|----------------|
|                                          	|              	|             	| Charge en heure/participant |                           	|            	|            	|
| Description de l'activité                	| Charge en %  	| Charge en heure | Augustin BRESSET        	| Guillaume MACQUART DE TERLINE | Pierre CHAMBET | Zacharie MARCH |
| Total                                    	|              	|             	|                         	|                           	|            	|            	|
| Gestion de projet                        	| 10           	| 20          	| 6                       	| 6                         	| 6          	| 1          	|
| Réunion de lancement                     	| 1,5          	| 3           	| 1                       	| 1                         	| 1          	| 0          	|
| Planning prévisionnel et Suivi des activités | 2            	| 4           	| 1                       	| 1                         	| 2          	| 0          	|
| Réunions de suivi                        	| 0            	| 0           	| 0                       	| 0                         	| 0          	| 0          	|
| Rédaction                                	| 4,5          	| 8           	| 2                       	| 3                         	| 2          	| 0          	|
| Outil collaboratifs (Google drive, Github)   | 2            	| 5           	| 2                       	| 1                         	| 1          	| 1          	|



##Planning prévisionnel


* 24/02 - 31/03 : Réalisation des conceptions préliminaires et détaillées. Auto-formations en Kotlin, Django et JavaScript

* 31/03 - 17/05 : Réalisation du codage et des phases d’intégration. Validation du bon fonctionnement de l’application.

* 17/05 - 30/05 : Préparation de la soutenance

* 30/05 - 31/05 : Soutenance



## Conception préliminaire

### Première version du plan du rapport final

1. Introduction
2. Cahier des charges
3. Développement
  1. Analyse du problème et spécification fonctionnelle
  2. Conception préliminaire
  3. Conception détaillée
  4. Codage
  5. Tests unitaires
  6. Tests d'intégration
  7. Tests de validation

4. Etude des résultats
  1. Réalisation des tests
  2. Pertinence des résultats
  3. Critique 
  4. Suggestion d'Amélioration

5. Conclusion

## Conclusion

### Récapitulatifs des résultats obtenus dans le livrable

Nous faisons ici le constat de la charge de travail et sa répartition. Une idée plus concrète des étapes du projet s'est formée. 

La répartition du travail est présentée de manière uniforme mais nous savons que ce ne sera pas le cas pour les étapes de développement qui seront réparties par pôles.

Le temps d'apprentissage compris dans *auto-formation* est biaisé car répartie sur l'ensemble du projet.


### Perspective pour la suite du projet

Les prochaines étapes consistent en la mise en place de l'architecture de notre logiciel, la définition des objets employés et des structures de bases de données, une approche mathématique de triangulation pour estimer la localisation.






