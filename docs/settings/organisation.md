# Organisation

## Organisation

Une **organisation** est une entité légale pouvant fonctionner de manière autonome ou en tant que filiale d'une organisation mère. Chaque organisation possède un numéro d'identification d'entreprise et un numéro d'enregistrement à la TVA uniques.

Une organisation peut comporter les éléments suivants :

- Plusieurs unités d'établissement.
- Plusieurs adresses de contact (seule l'adresse officielle du siège est requise pour les documents officiels).

Lors de la création d'une organisation, les informations suivantes doivent être fournies :

1. **Nom de l'organisation**
2. **Email et numéro de téléphone**
3. **Numéro d'entreprise et numéro de TVA**
4. **Adresse complète** : pays, ville, rue, numéro, code postal
5. **Coordonnées bancaires** : IBAN, BIC
6. **Langue de communication**

Par défaut, une organisation est initialisée avec l'identifiant 1.

Cette structure garantit une gestion efficace des informations, facilitant ainsi la communication, la facturation et le suivi administratif.


## Équipe de gestion

L'**équipe de gestion** est responsable de l'administration de plusieurs centres et centralise la facturation et la comptabilité.

Pour une gestion optimale, les informations suivantes sont nécessaires :

1. **Nom** : Nom de l'équipe ou du bureau associé.
2. **Code de groupe** : Identifiant unique au format hexadécimal.
3. **IBAN** : Numéro de compte bancaire pour la facturation des services.
4. **Type d'imprimante** : Format d'impression des documents officiels :
   - `POS-80` pour les tickets
   - `ISO-A4` pour les rapports
5. **Mode par défaut pour les documents** : Définit le format d'affichage des documents :
   - `simple`
   - `groupé`
   - `détaillé`

**Fonctionnalités**

- **Gestion des centres associés** : Chaque équipe de gestion peut être liée à plusieurs centres.
- **Journaux comptables** : Gestion détaillée des finances et suivi des opérations.
- **Signature électronique** : Ajout de signatures personnalisées pour les communications officielles.


## Centre

Le **centre** est un établissement qui offre des unités locatives pour des séjours, qu'ils soient courts ou longs.

Lors de la création d'un centre, les informations suivantes doivent être fournies :

1. **Nom du centre**
2. **Code alpha** : Identifiant unique du centre.
3. **Équipe de gestion** : Équipe responsable du centre.
4. **Type de séjour** : Type d'hébergement proposé.
5. **Organisation associée** : Organisation à laquelle le centre est affilié.


## Unité locative

L'**unité locative** permet de gérer les unités de location, leur disponibilité et les actions nécessaires à leur gestion.

Lors de la création d'une unité locative, les éléments suivants doivent être définis :

1. **Nom** : Nom de l'unité locative.
2. **Type** : Type d'unité locative en fonction de sa capacité :
   - Bâtiment
   - Chambre
   - Lit
   - Salle de réunion
   - Réfectoire
   - Salle
   - Mobilier, accessoires et équipement

3. **Catégorie** : Catégorie des produits associés à l'unité.
4. **Capacité** : Nombre de personnes pouvant être logées.
5. **Logement** : Indique si l'unité est un logement.
6. **Sous-unités** : Drapeau indiquant la présence de sous-unités.
7. **Peut être loué** : Drapeau indiquant si l'unité est disponible à la location.
8. **Location partielle ?** : Permet de spécifier si l'unité peut être louée partiellement.


