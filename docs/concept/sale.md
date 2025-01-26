# Configuration de Ventes

Cette option permet de définir les paramètres pour les réservations, les réductions et les produits automatiques.

## Réservation
### Types de réservation

Cette configuration permet de définir différents types de réservations en fonction de la clientèle ou de l’organisation concernée, ainsi que les délais d’expiration des options qui y sont associés. Chaque type est identifié par un code unique et possède un nombre de jours d’expiration spécifique pour l’option de réservation. Ces paramètres peuvent être modifiés afin de s’adapter aux besoins spécifiques de l’organisation.

| ID  | Nom                         | Code  | Délai d'expiration (jours) |
|-----|-----------------------------|-------|----------------------------|
| 1   | Individuel (tout public)    | TP    | 10                         |
| 3   | Stage                       | STA   | 20                         |
| 4   | Séjour scolaire             | SEJ   | 30                         |
| 6   | Groupe (tout public)        | TPG   | 10                         |
| 13  | Tour Operateur              | TO    | 10                         |
| 14  | Online Travel Agencies      | OTA   | 1                          |
| 15  | Autre                       |       |                            |


## Catalogue 

### Produits

#### Produits
La configuration des produits permet d’associer chaque produit à un modèle spécifique, garantissant ainsi un SKU unique pour une identification précise. Chaque produit doit comporter un libellé descriptif, un SKU, un modèle de produit correspondant, ainsi que des informations clés telles que son statut de vente, sa possibilité d’être inclus dans un pack et la famille à laquelle il appartient. De plus, un produit peut regrouper plusieurs autres produits, formant ainsi un pack. Enfin, il peut avoir plusieurs prix selon différentes listes de prix.
#### Modelé de produit
La configuration de Modèle de Produits permet de définir et organiser les types de produits dans l'organisation, en spécifiant leur libellé, type, famille et possibilité de vente. Elle inclut aussi des détails sur la comptabilisation, les statistiques de vente, et si le produit est un repas, collation ou logement. Un modèle peut avoir plusieurs variantes et être disponible pour plusieurs groupes.
#### Catégories
La configuration de catégorie permet de regrouper les modèles de produits et les types de réservation. Elle inclut des familles telles que Séjours scolaires (CDV), Produits de caisse (POS) et SPORT (SPT). Chaque catégorie a une description spécifique pour faciliter la gestion
#### Familles
La famille est le regroupement de produits présents dans tous les centres. Par défaut, une famille doit être créée dans laquelle seront regroupés tous les produits de l'organisation
#### Groupes
Il est nécessaire de remplir les champs suivants : Nom du groupe de produits et Centre. La configuration de groupe permet d'organiser les modèles de produits et les produits.


### Prix

#### Prix
La classe Price gère les prix des produits, y compris le prix hors taxes, le prix TTC, le taux de TVA, et les règles comptables associées. Elle permet de définir des prix en fonction de la méthode de calcul, d’assurer leur validité et de les lier à des produits spécifiques et des listes de prix.

#### Liste de prix
La configuration de la liste de prix permet de gérer les tarifs applicables sur des périodes spécifiques et selon des catégories de services. La liste  doit être défini une fois par an.  Chaque entrée inclut un identifiant, un statut, des dates de validité et la durée, garantissant l'application des tarifs corrects pour  chaque catégorie de liste de prix. 

### Remises

#### Remise
La réduction permet d’offrir des avantages tarifaires aux clients selon des critères spécifiques. Chaque réduction se compose d’un libellé, d’une valeur, d’un type (pourcentage ou gratuité) et de conditions à remplir pour en bénéficier.
 
#### Liste de remises
Cette liste définit des remises pour différentes catégories tarifaires sur une période donnée. Chaque entrée inclut un libellé, une catégorie, des dates de validité, une classe tarifaire et des taux de remise minimum et maximum. De plus, la liste de réductions regroupe les différentes remises disponibles.

### Produits automatiques
La liste des produits est organisée par catégorie et par période précise, à partir d'une date de début et d'une date de fin. Elle inclut tous les produits devant être appliqués automatiquement à la réservation, si celle-ci correspond à la période spécifiée et aux conditions de chaque produit.


### Saisons

#### Saison

La classe saison gère les saisons, leur année d'application, leur catégorie et les périodes associées. Elle permet de définir si une saison est liée à une classe tarifaire spécifique et de lier des catégories de centres cibles pour la saison

#### Periodes de Saison 
La classe periode de saison définit une période dans une saison, avec des dates de début et de fin, ainsi que des informations sur le type de saison et la catégorie. Elle calcule également le mois, l'année et la catégorie de la saison..

#### Types de Saison

La classe Type de saison définit les différents types de saison. Chaque type a un nom court et une description détaillée qui explique quand et comment utiliser ce type de saison. La description peut être multilingue

| ID  | Nom  | Description        |
| --- | ---- | ------------------ |
| 1   | BS   | Basse saison       |
| 2   | MS   | Moyenne saison     |
| 3   | HS   | Haute saison       |
| 4   | THS  | Très haute saison  |

### Séjours and Planning

####  Tranches horaires

La classe Time Slot permet de diviser une journée en créneaux horaires pour la planification. Elle comprend un nom, une description, l'heure de début et de fin, ainsi qu'un ordre pour trier les créneaux. Utilisée pour organiser des plages horaires dans des systèmes de réservation ou de gestion.

### Plan de paiement
Le plan de paiement définit les modalités de règlement pour les réservations. Pour chaque plan de paiement, il est nécessaire de préciser le type de réservation, la catégorie tarifaire et les échéances correspondantes.


