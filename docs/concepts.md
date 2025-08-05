# Récapitulatif des concepts manipulés

## Organisation

Discope permet la gestion des activités d'une (ou plusieurs)
organisation(s), dont l'objet est la location d'unités locatives de
différents types : bâtiments, salles, chambres et lits (et, dans
certains cas, du mobilier).

## Centre

Les unités locatives sont réparties au sein d'un ou plusieurs
**Centres**.

Un centre est une unité d'établissement (entité administrative) qui
regroupe un ou plusieurs bâtiments, dont dépendent celui-ci.

La capacité d'un centre (en termes de lits) est la somme des capacités
des bâtiments et autres unités locatives qui en font partie.

## Equipe de gestion

Pour chaque organisation, une ou plusieurs **équipes de gestion**
assurent la gestion administrative des locations relatives à un ou
plusieurs Centres.

La gestion d'un Centre est toujours assurée par une et une seule équipe
de gestion.

## Unités locatives

Une **unité locative** est tout espace ou équipement lié à un centre qui
peut faire l'objet d'une réservation. Chaque centre dispose
d'équipements intérieurs et extérieurs qui incluent toutes les unités
locatives, qu'elles soient destinées ou non au logement.

Les unités locatives incluent les ressources non destinées au logement
(dans lesquelles il n'est pas possible de dormir), dont, notamment :
les salles de réunion, les espaces sportifs, du mobilier ou des
appareils électroménagers. Les unités locatives « ressources » peuvent
éventuellement être exclusives à une unité locative « logement »
spécifique.

La communication concernant les disponibilités de location se fait
toujours par unité locative.

Certaines unités locatives sont associées à une capacité, dont la nature
varie en fonction de l'équipement : pour un réfectoire, ce sera le
nombre de places assises, tandis que pour une chambre, ce sera le nombre
de lits.

En comptabilisant la capacité des unités locatives de type "logement",
on obtient le nombre total de lits dont dispose un centre. Si un centre
dispose de plusieurs unités du même type, chacune est renseignée avec sa
capacité individuelle.

## Contacts

Les fiches contact sont utilisées pour identifier toute personne devant
pouvoir être contactée et décrivent donc exclusivement des personnes
physiques.

-   Prénom, nom
-   Titre : Mr, Mme,
-   Type : personnel, secrétariat, direction,
-   Langue
-   Téléphone, fax, email

## Client

Les clients sont les personnes au nom desquelles sont créées les
réservations.

Les règles de base sont :

-   Une réservation ne peut être prise qu'au nom d'un client ;
-   Un client peut être une personne physique ou une personne morale.

Il peut y avoir un lien hiérarchique entre les clients de type
« organisation » (uniquement pour les personnes morales):

-   Une organisation peut être une filiale d'une (et une seule)
    organisation mère (dans ce cas, il faut pouvoir indiquer
    l'organisation parente)
-   Une organisation dispose d'un (et un seul) numéro d'identification
    d'entreprise et un (et un seul) numéro d'enregistrement à la TVA ;
-   Une organisation peut avoir plusieurs unités d'établissement ;
-   Une organisation peut avoir plusieurs adresses de contact (il y a
    des obligations légales concernant le siège d'une organisation \[et
    la publication des adresses de ses unités d'établissements\], mais
    aucune contrainte concernant les communications). Dans les faits,
    sur les documents officiels, il faut faire figurer l'adresse
    officielle (siège), mais pouvoir envoyer ces documents par la poste
    à n'importe quelle adresse fournie par l'organisation. (Adresse
    "de facturation" <> adresse figurant sur la facture)
-   Dans certaines situations, les factures d'une organisation sont
    payables par une autre organisation (avec laquelle elle n'a pas
    forcément de lien légal). Dans ce cas, les règles ci-dessus
    s'appliquent à l'organisation "payeuse".

Une organisation peut avoir plusieurs 'partenaires'. Un partenaire est
soit une personne physique, soit une autre organisation.

Dans les informations relatives à une organisation, on a besoin de
connaitre :

-   Ses détails administratifs (contrat)
-   Les personnes de contact
-   Les organisations qui paient ses factures
-   L'adresse à laquelle envoyer les factures (liées aux organisations 'payeuses')

Les informations qui doivent être retrouvées pour chaque client
sont similaires aux contacts:

-   Titre
-   Nom
-   Adresse, localité, zip, country
-   Langue
-   Téléphone, fax, email
-   IBAN, BIC

Avec des information supplémentaires spécifiques aux organisations:

-   Nom organisation (+ service ou département)
-   TVA

## Nature client

A des fins de statistiques ou de catégorisation tarifaire, les clients
peuvent être assignés à une « nature » spécifique.

La nature du client permet d'associer une catégorie tarifaire en
fonction de la manière dont un client se présente (école, stage, asbl,
...).

A chaque nature de client, est associé une (et une seule) catégorie
tarifaire, qui dépend de la configuration.

## Catégories tarifaires

Les catégories tarifaires permettent l'application de réductions
systématiques, et influencent la définition des saisons, qui sont
également prises en compte pour les réductions systématiques (il peut
éventuellement y avoir des saisons différentes en fonction des
catégories tarifaires).

Pour permettre la souplesse requise dans la gestion des ristournes, il
est nécessaire de définir des types de réduction (discount) : les
calculs de taux de réduction peuvent alors y être appliqués selon un
algorithme générique.

-   Les ristournes sont cumulatives avec un plafond (pour tous les
    produits) défini par catégorie tarifaire
-   Les ristournes sont définies selon au taux (cumulatif) et une
    condition
-   Les tests des conditions sont complexes et doivent être faits
    manuellement ; et pour chaque type de réduction, il y a des
    paramètres différents

Le taux de réduction final est calculé pour chaque ligne, mais peut
aussi être défini manuellement.

## Produits

Un ou plusieurs produits peuvent être associées à une réservation.

Typiquement les produits sont des nuitées, des pensions, ou d'autres
consommations liées à un séjour.

Chaque produit a la possibilité d'être rattaché à une ressource.

Chaque liste de produits (par centre) peut être considérée comme une
liste de prix.

Un assistant permet la duplication automatique de produits pour ceux qui
sont communs à tous les centres.

Les produits nécessitent la possibilité d'être regroupés par critères
d'application : âge, période, type (pension, dîner, ...)

La meilleure approche consiste à associer des catégories aux produits
(possibilité de gérer les catégories indépendamment). Ceci offre
l'avantage que les catégories peuvent être associés aux produits de tous
les centres (pas de catégorisation par centre).

Comme les produits sont à considérer par année, un assistant donne la
possibilité de dupliquer tous les produits à l'identique pour une
nouvelle année civile.

Les produits répondent aux besoins suivant pour la gestion de la
location :

-   Attribution des réductions à un produit (catégorie client)
-   Déterminer l'impact d'une réservation sur la disponibilité
-   Tenue de la comptabilité

A chaque produit sont associés un nom, un mnémonique (SKU), un type
(service \[simple ou planifiable\] ou consommable \[simple ou
stockable\]), une famille, et des règles comptables.

## Services (pensions)

Les options de pension possibles sont :

-   Pas de repas
-   Petit déjeuner (B&B)
-   Demi-pension
-   Pension complète

## Réservations

Une réservation est constituée par l'ensemble des informations qui
permettent d'identifier le client qui occupe un lieu à un moment donné,
les personnes concernées, ainsi que les options et services associés.

Une réservation est toujours limitée à un centre mais peut porter sur
plusieurs unités locatives.

Pour le moment, les réservations peuvent avoir une structure
hiérarchique à deux niveaux : une réservation pour faire l'objet d'une
ou plusieurs réservations "enfants", c'est à dire qui se rapportent à la
même période et au même groupe.

La structure préconisée est d'associer, pour chaque réservation, une ou
plusieurs lignes de réservation qui font le lien entre une réservation
et la liste des produits réservés (relatifs au centre visé par la
réservation). Cette approche permet également d'avoir une gestion au
niveau des produits (paramètres éventuellement différents par produit
d'une même réservation) pour les réductions et pour le client final (qui
paie quel produit).

## Types de réservation

Pour permettre le suivi historique et la ventilation des réservations,
un type peut être assigné à une réservation. Les types existants sont
les suivants :

-   Individuel (tout public)
-   Stage
-   Séjour scolaire
-   Groupe (tout public)
-   Tour Opérateur
-   Online Travel Agencies
-   Autre

Ce dispositif sert à la fois à des fins de statistiques et d'assistance
à la navigation des utilisateurs (une réservation CDV peut avoir des
options distinctes d'une réservation B&B).

## Produits inclus dans la réservation

Pour pouvoir faire un lien entre ce qui est réservé et la "disponibilité
restante" et pour permettre de générer plusieurs factures pour une même
réservation, c'est à dire pouvoir répartir le paiement de différents
produits d'une même réservation entre plusieurs clients, les
réservations sont décrites en utilisant des lignes de réservation. Ainsi
chaque ligne de réservation peut être assignée à un client différent
(par défaut, il s'agit du client de la réservation).

Une ligne associe une ressource (via un produit) à un moment dans le
temps.

Chaque réservation est donc composée d'une ou plusieurs lignes de
réservation qui permettent l'association entre une réservation et un
produit.

Chaque ligne reprend donc les informations suivantes :

-   Produit (avec indication du centre visé)
-   Client (par défaut celui de la réservation, mais peut être modifié
    manuellement)
-   Date de début du séjour
-   Heure de début du séjour
-   Date de fin du séjour
-   Heure de fin du séjour
-   Prix (calculé sur base du produit visé)
-   Taux de réduction à appliquer (en fonction de la catégorie tarifaire
    déduite sur base du client)

Pour le moment :

-   Utilisation de réservation parent et réservation enfant
-   Pour chaque pack, on a une ligne de réservation

## Compositions

Une composition est une liste (exhaustive) des personnes qui occuperont
la ou les ressources liées à une **réservation**. La raison d'être des
compositions est liée à des obligations administratives et légales (taxe
de séjour locale et déclaration de séjour auprès de la police locale).
Les compositions sont ventilées par réservation, groupe, et unité
locative (bâtiment, chambre).

Une composition peut être récurrente (toujours la même pour un groupe
donné), mais peut toujours être adaptée en rapport avec une réservation
particulière.

## Packs

Il est possible de créer des "packs" qui représentent la description de
certains patterns récurrents de réservation. Les packs peuvent également
décrire des offres spécifiques, de type "séjours".

Un "pack" regroupe un ou plusieurs produits ou services et, lorsqu'il
est sélectionné, permet l'ajout automatique de ces éléments dans la
liste des services associé au séjour correspondant.

Dans le cas d'un pack, les quantités (et prix) des lignes de réservation
correspondant aux éléments sont ajustées automatiquement sur base dates
du séjour correspondant.
