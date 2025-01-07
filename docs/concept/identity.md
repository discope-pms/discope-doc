# Identité

## Identité

### Identité

L'**Identité** gère les informations relatives à une personne juridique ou naturelle dans le système. Elle définit plusieurs propriétés telles que le nom de l'identité, son type (personne physique, entreprise, organisation), ainsi que les informations bancaires, fiscales et de contact associées à cette identité.

Propriétés principales :

1. **Nom** : Nom affiché de l'identité, qui peut être le nom légal ou le nom complet d'une personne.
2. **Type** : Type de l'identité, pouvant être une personne physique, une entreprise, un auto-entrepreneur, ou une organisation.
3. **Description** : Rappel court de l'identité pour aider à l’identification dans le système.
4. **Numéro de TVA** : Numéro de TVA de l'organisation, si applicable.
5. **Adresse** : Adresse légale ou physique de l'identité, incluant la rue, la ville, le code postal et le pays.
6. **Contacts** : Liste des contacts associés à l'identité, comme les employés, les clients ou les partenaires.
7. **Organisation** : L’organisation qui est la société mère, si l'identité fait partie d'une structure hiérarchique.
8. **Coordonnées bancaires** : Détails relatifs à un compte bancaire, si disponible, pour l'identité.
9. **Statut** : Statut actuel de l'identité dans le système (actif, inactif, suspendu, etc.).


### Type d'Identité

Le Type d'Identité est utilisée pour définir et gérer les types d'identités pouvant être attribués à une entité dans le système. 

Elle permet de classer les identités en différentes catégories selon leur nature juridique ou fonctionnelle.  

| **ID** | **Code** | **Description**                              |
|-------|----------|---------------------------------------------|
| 1     | **I**    | Particulier (personne physique)             |
| 2     | **SE**   | Indépendant                                 |
| 3     | **C**    | Société                                     |
| 4     | **NP**   | Groupes, Associations et Écoles (ASBL)      |
| 5     | **PA**   | Administration publique                     |


## Utilisateur

L'Utilisateur gère les informations relatives aux utilisateurs du système. 

Elle définit plusieurs propriétés telles que le nom d'affichage de l'utilisateur, la relation avec son identité, les paramètres associés à l'utilisateur, ainsi que les centres et equipes de gestion  de l'utilisateur est rattaché. 

Propriétés principales :

1. **Nom** : Nom d'affichage de l'utilisateur.
2. **Identité** : Identifiant de l'identité de l'utilisateur.
3. **Paramètres** : Liste des paramètres associés à l'utilisateur.
4. **Centres** : Liste des centres auxquels l'utilisateur est affilié.
5. **Equipes de gestions** : Liste des bureaux des centres associés à l'utilisateur.
7. **Statut** : État actuel de l'utilisateur (créé, validé, confirmé, suspendu).

La classe prend également en charge un flux de travail pour gérer l'état de l'utilisateur, avec des états comme: 

- **Créé** (compte créé mais non validé)
- **Validé** (adresse e-mail confirmée)
- **Confirmé** (compte validé)
- **Suspendu** (compte suspendu).

Les transitions entre ces états sont basées sur des événements tels que la validation de l'adresse e-mail ou la confirmation du compte. Chaque état peut avoir des transitions spécifiques, par exemple, la suspension du compte ou la confirmation après validation.

## Contact

Le Contact représente une personne liée à une réservation avec des responsabilités spécifiques. Le partenariat reste toujours de type `contact`. 

Les types de contact possibles incluent : 

- **Réservation** pour gérer les détails de la réservation
- **Facture** pour recevoir la facture
- **Contract** pour recevoir les contrats
- **Séjour** pour identifier la personne présente durant le séjour 

## Address

L'Address est utilisée pour gérer les informations concernant les adresses physiques liées à une identité. Chaque adresse a un nom d'affichage, qui peut être dérivé des champs d'adresse (tels que la rue, la ville et le code postal). L'adresse est liée à une **identité**, et un rôle peut être attribué pour indiquer l'objectif principal de l'adresse (par exemple, légal, facture, livraison, autre).

Propriétés principales :

1. **Nom** : Nom de l'adresse.
2. **Nom d'affichage** : Nom d'affichage de l'adresse, dérivé des autres champs de l'adresse.
3. **Nom d'affichage de l'identité** : Nom de l'identité associée à l'adresse.
4. **Identité** : L'identité à laquelle l'adresse se rapporte.
5. **Rue d'adresse** : La rue et le numéro de l'adresse.
6. **Complément d'adresse** : Informations optionnelles pour l'envoi du courrier, telles qu'un appartement, un box ou un étage.
7. **Rôle** : Rôle de l'adresse
8. **Ville** : La ville de l'adresse.
8. **Code Postal** : Le code postal de l'adresse.
9. **État ou région** : L'état ou la région associé à l'adresse.
10. **Pays** : Le pays de l'adresse, utilisant le format ISO-3166-2.


Le **rôle** de l'adresse spécifie son objectif principal et peut prendre l'une des valeurs suivantes :

- **Légal**: Adresse utilisée à des fins légales.
- **Facture**: Adresse utilisée pour l'envoi des factures.
- **Livraison** : Adresse utilisée pour l'envoi des livraisons.
- **Autre** : Adresse utilisée pour d'autres objectifs non spécifiés.


## Établissement

### Center

Le Center représente un établissement d'hébergement fournissant des logements locatifs. Il permet notamment de gérer :  

- L'identifiant unique du centre.  
- Les groupes de prix et remises.  
- Les catégories et unités locatives associées.  
- Les informations de gestion comme le responsable, les modèles de communication et les compteurs de consommation.  


### Équipe de gestion

#### Équipe de gestion

Équipe de gestion permet la gestion des différents centres. Cette classe offre des fonctionnalités avancées telles que :  

- La gestion des contacts et des utilisateurs associés.  
- La configuration des signatures pour les communications.  
- La définition des modes d'impression pour les tickets de point de vente (PoS).  
- L'attribution manuelle des unités locatives.  
- La gestion des journaux comptables.  
- L'intégration avec des sections analytiques pour la comptabilité.  

L'Équipe de gestion des informations détaillées:

- Nom de l'équipe de gestion  
- Identifiant numérique de l'équipe de gestion  
- Liste des centres rattachés à l'équipe de gestion  
- Liste des contacts associés à l'équipe de gestion  
- Liste des utilisateurs liés à l'équipe de gestion  
- Mode par défaut pour la génération des documents officiels  
- Format d'impression pour les tickets de point de vente (PoS)  
- Liste des journaux comptables associés à l'équipe de gestion  
- Liste des produits favoris de l'équipe de gestion  
- Adresse e-mail pour l'envoi des copies des messages envoyés  

### Contact des équipes de gestion

La contact des équipes de gestion est utilisée pour gérer les coordonnées des contacts liés à un bureau de gestion de centre. Elle permet de définir plusieurs types de contact selon leurs responsabilités spécifiques :  

- **Réservation** : Gestion des réservations et devis.  
- **Facture** : Gestion des factures.  
- **Contract** : Questions juridiques ou contractuelles.  


La combinaison **`equipe de gestion`** et **`email`** doit être unique, garantissant l'absence de doublons dans les contacts.  

## Client

### Client

Le client est un partenaire dont l'activité principale est de réaliser une ou plusieurs réservations. 

Propriétés principales :

- Nom complet
- L'organisation à laquelle appartient le client
- L'identité du client
- La catégorie tarifaire applicable au client.
- Le type de client (en relation avec les classes tarifaires).
- La nature du client, qui permet d'attribuer une catégorie tarifaire.
- Adresse principale du client.
- Numéro de compte IBAN arbitraire associé au client.

Cette classe est essentielle pour gérer les informations des clients et leurs réservations, facilitant l'attribution des tarifs et le suivi de leur activité dans le système.


### Types de clients 

Cette classification permet de regrouper les clients selon leur statut juridique ou organisationnel, facilitant ainsi la gestion des relations commerciales et l’adaptation des services.

Exemple des valeurs par défaut :

| ID  | Code | Description                                                |
|-----|------|------------------------------------------------------------|
| 1   | I    | Particulier (personne physique)                           |
| 2   | SE   | Indépendant                                                |
| 3   | C    | Société                                                    |
| 4   | NP   | Association ou École (asbl, association de fait ou autre)  |
| 5   | PA   | Administration publique                                    |


### Nature client

La nature client gère les informations relatives aux caractéristiques et aux classifications des clients dans le système de gestion.

Elle permet de définir des attributs spécifiques pour catégoriser les clients en fonction de leur type et de leur classe tarifaire, facilitant ainsi la gestion des tarifs et des relations commerciales. Cette classe inclut plusieurs propriétés pour configurer et administrer les différentes natures de clients.

Propriétés principales :

1. **Nom** : Nom de la nature client, utilisé comme alias de la description.  
2. **Code** : Identifiant mnémotechnique de la nature client, unique et obligatoire.  
3. **Description** : Courte description de la nature client, multilingue.  
4. **Classe tarifaire** : Référence vers la classe tarifaire applicable à cette nature client.  
5. **Type de client** : Référence vers le type de client auquel cette nature est associée.  

La nature client impose des règles pour assurer la cohérence des données :  

- Le champ **Code** doit être unique et non vide.  
- Les champs **Classe tarifaire** et **Type de client** doivent pointer vers des entités existantes et actives.  
- Les descriptions doivent être localisées pour les langues prises en charge dans le système.

Les natures clients disponibles :

| ID  | Code | Description               |
|-----|------|---------------------------|
| 1   | IN   | Individuels (particuliers) |
| 2   | AC   | Administration publique    |
| 3   | AD   | Administrateur             |
| 4   | AM   | Groupe d'amis              |

### Catégorie tarifaire

La **catégorie tarifaire** est responsable de la gestion des informations liées à la classification des tarifs attribués aux clients dans le système de gestion.

Elle permet d'établir des classes tarifaires qui facilitent l'attribution de prix spécifiques aux produits réservés, en fonction de la catégorie à laquelle le client appartient. Chaque catégorie tarifaire est conçue pour répondre à des besoins particuliers et s'adapte aux diverses typologies de clients, optimisant ainsi la gestion des prix et des services.

Propriétés principales :

1. **Nom** : Identifiant unique de la catégorie tarifaire.
2. **Description** : Description succincte et multilingue de la catégorie tarifaire.

Les catégories tarifaires disponibles :

| ID  | Name | Description                            |
|-----|------|----------------------------------------|
| 1   | T1   | Institutions privilégiées (reconnues CWB) |
| 2   | T2   | Groupements                            |
| 3   | T3   | Réseau Organisation                    |
| 4   | T4   | Grand public                           |
| 5   | T5   | Ecoles primaires et secondaires        |
| 6   | T6   | TO partenaires                         |
| 7   | T7   | Ecoles maternelles                     |


### Tranche d'âge

La tranche d'âge gère les informations relatives aux plages d'âge utilisées dans les réservations. 

Elle permet d’attribuer des consommations spécifiques en fonction de la composition des hôtes associés à une réservation. Cette classe définit plusieurs propriétés pour configurer et gérer les plages d’âge, ainsi que leur utilisation dans les conditions de réduction.

Propriétés principales :

1. **Nom** : Nom de la plage d’âge, multilingue.  
2. **Description** : Courte description de la plage d’âge, multilingue.  
3. **Âge minimal** : Âge limite inférieur (inclus) pour la plage.  
4. **Âge maximal** : Âge limite supérieur (exclu) pour la plage.  
5. **Statut** : Indique si la plage d’âge est active.  

La tranche d'âge impose des restrictions pour garantir la validité des données :  

- Les champs **Âge minimal** et **Âge maximal** doivent être des entiers compris entre 0 et 99.  
- La combinaison des valeurs **Âge minimal** et **Âge maximal** doit être unique.  

Les catégories d'âge disponibles :

| **ID** | **Nom**           | **Description**                                  | **Âge De** | **Âge À** |
|--------|--------------------|---------------------------------------------------|------------|-----------|
| 1      | Adulte (26-99)     | Adultes de 26 ans et plus.                        | 26         | 99        |
| 2      | Secondaire (12-26) | Adolescents (école secondaire) et jeunes adultes. | 12         | 26        |
| 3      | Primaire (6-12)    | Enfants (école primaire).                         | 6          | 12        |
| 4      | Maternelle (3-6)   | Enfants en bas âge (école maternelle).            | 3          | 6         |
| 5      | Bébé (0-3)         | Enfants en très bas âge (bébés).                  | 0          | 3         |


### Tour Opérateur

La classe **Tour Opérateur** gère les informations relatives aux agents de voyage spécialisés dans les séjours organisés ou aux OTA (Online Travel Agencies) agissant en tant qu’intermédiaires pour finaliser des réservations.

Propriétés principales :

1. **Code** : Code de référence unique pour identifier le partenaire TO.  
2. **Commission** : Taux de commission appliqué pour le TO (peut être défini en montant ou en pourcentage). Il est facultatif et a une valeur par défaut de **0.0**.  
3. **Nature du client** : Type de client associé aux classes tarifaires.

