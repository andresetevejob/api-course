# API


## 1. Definition

Application programming interface, en Français interface de programmation d'application.
Elles permettent à des applications de communiquer entre elles, en faisant abstraction des langages, elles sont écrites  au moyen d'un ou plusieurs protocols.
Ce cours sera porté sur les API web.

## 2. Fonctionnement
* Elle fonctionne comme un contrat établit entre le fournisseur et le demandeur d'informations.
Le demandeur doit envoyer la donnée dans une structure particulière attendu par le protocol, le fournisseur devra répondre selon une condition particulière.

* Le consommateur n'a aucune visibilité sur comment les données sont constituées avant de lui être envoyées

* C'est le fournisseur qui decide de ce qu'il veut pouvoir communiquer comme informations

* Le fournisseur et le consommateur peuvent être soient présent sur le même réseau, ou être distants.

* Elle peut avoir une durée de vie.Le fournisseur peut décider de fermer l'API pour plusieurs raisons (budgétaire, etc...)

Les apis, permettent à votre infrastructure d'être connecté à d'autres systèmes.Les apis apportent de la valeur métier à votre système d'information.

### 2.1 Les éléments qui interviennent dans son fonctionnnement
- Le client : Le demandeur de la ressource
- Les ressources : 
 sont les informations que les différentes applications fournissent à leurs clients. Les ressources peuvent être des images, des vidéos, du texte, des chiffres ou tout type de données. La machine qui fournit la ressource au client est également appelée le serveur. Les organisations utilisent les API pour partager des ressources et fournir des services Web tout en maintenant la sécurité, le contrôle et l'authentification. En outre, les API les aident à déterminer quels clients ont accès à des ressources internes spécifiques.

- Le serveur : Le fournisseur de la ressource.IL expose les informations qu'il souhaite mettre à disposition sans sacrifier la sécurité de ces dernères.

- Le protocol : moyen par lequel client et serveur communique

### 2.2  Le contrat d'une API WEB
IL contient les informations suivantes :

 - Le protocol de communication
 - Le chemin d'accès à la ressource
 - Les opérations disponibles
 - La politique de sécurité et de gestion des erreurs

Exemple : https://newsapi.org/docs/get-started#search

## 3. Les différents types d'API

 - Les API publiques
 - Les API privées
 - Les API partenaires

### 3.1 API publiques



### 3.2 API privées



### 3.3 API partenaires



## 4. Protocols

Une api peut être implémenter au moyens de différents protocols et différentes Architectures web

 ### 4.1 Les protocols

* HTTP
* FTP
* KAFKA
* RPC

 ### 4.2 Les architectures

 * SOAP
 * REST
 * GRAPHQL
 * GRPC

Dans notre apprentissage, nous allons nous focaliser sur le protocol HTTP, ainsi que l'architecture REST qui est la plus répandue à l'heure ou j'écris ces lignes sur le web.


### Ressources
- https://aws.amazon.com/fr/what-is/api/
- https://www.redhat.com/fr/topics/api/what-are-application-programming-interfaces#types-dapi
- https://aws.amazon.com/fr/what-is/restful-api/