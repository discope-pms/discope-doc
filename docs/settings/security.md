# Sécurité

## Utilisateurs

Pour configurer un nouvel utilisateur, il est nécessaire de renseigner les informations suivantes :

- Sélectionner une **identité existante**.
- Fournir une **adresse email** et un **mot de passe**.
- Attribuer un **nom d’utilisateur**.
- Choisir la **langue de préférence**.

**Note** : Une fois l’utilisateur créé, sa validation devra être effectuée par un administrateur.

## Groupes

La configuration des groupes permet de gérer l'accès des utilisateurs aux différentes applications et fonctionnalités du système. Chaque groupe d'utilisateurs est défini par des **rôles spécifiques**, assurant ainsi une gestion fine des **permissions**.

Les groupes sont organisés pour couvrir une large gamme de domaines fonctionnels, chacun ayant des niveaux d'accès bien définis. Par défaut, certains groupes sont créés lors de l'initialisation de l'application, mais de nouveaux groupes peuvent être ajoutés en précisant un nom et une description, afin de répondre aux besoins spécifiques de l'organisation.

Les groupes couvrent les domaines suivants :

- **Administration système** : Accès complet au système pour les administrateurs.
- **Vente** : Rôles d'administrateur et d'utilisateur pour la gestion des ventes.
- **Réservation** : Rôles d'administrateur et d'utilisateur pour la gestion des réservations.
- **Comptabilité** : Gestion des opérations financières avec des rôles d'administrateur et d'utilisateur.
- **Statistiques** : Accès aux données statistiques avec des droits différenciés.
- **Documents** : Administration et gestion des documents partagés.
- **Configuration** : Rôles pour les utilisateurs et administrateurs chargés de la configuration du système.
- **Inventaire** : Gestion de l'inventaire, avec des utilisateurs et administrateurs dédiés.
- **Caisse** : Gestion du point de vente (POS) avec des droits spécifiques.
- **Support** : Équipe de support pour l'assistance aux utilisateurs et le suivi des demandes.

## Permissions

Le système de **permissions** permet de gérer les accès des utilisateurs aux différentes fonctionnalités de l'application. Chaque permission définit les droits d'un groupe ou d'un utilisateur sur une entité spécifique. Cela inclut :  

- **class_name** : Nom de l'entité ou de la fonctionnalité concernée.  
- **group_id** : Identifiant du groupe qui possède les permissions.  
- **rights** : Actions autorisées (**Créer**, **Lire**, **Modifier**, **Supprimer**).  

### Exemples de permissions

- **Administrateur** : Accès complet aux réservations, contrats et factures (**Créer**, **Lire**, **Modifier**, **Supprimer**).  
- **Responsable financier** : Gestion complète de la comptabilité (**Créer**, **Modifier**).  
- **Équipe commerciale** : Gestion des produits, saisons et paiements (**Créer**, **Modifier**, **Supprimer**).  
- **Utilisateur standard** : Accès en lecture seule aux documents.  

### Étapes pour créer de nouvelles permissions
1. Identifier le groupe ou l'utilisateur concerné.  
2. Sélectionner l'entité cible (ex. : `sale\booking`, `finance\accounting`).  
3. Définir les droits nécessaires : **Créer**, **Lire**, **Modifier**, **Supprimer**.  
4. Appliquer les changements dans la configuration des permissions.  
