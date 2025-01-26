# Communication

## Emails (SMTP)
Cette configuration permet d'établir les paramètres nécessaires pour l'envoi d'e-mails via un serveur SMTP. Elle inclut des éléments essentiels tels que l'hôte SMTP, le port, le nom d'affichage du compte, le nom d'utilisateur, le mot de passe et l'adresse e-mail associée. De plus, il est important de fournir une adresse e-mail pour signaler les abus. Tous ces paramètres doivent être définis dans le fichier `config.json`.

### Paramètres de configuration SMTP

- **`EMAIL_SMTP_HOST`** : Nom d'hôte du serveur SMTP pour l'envoi d'e-mails.
- **`EMAIL_SMTP_PORT`** : Port à utiliser pour les connexions SMTP.
- **`EMAIL_SMTP_ENCRYPT`** : Couches de chiffrement à utiliser pour les connexions SMTP ('tls' ou 'ssl', false pour SMTP sans chiffrement).
- **`EMAIL_SMTP_ACCOUNT_DISPLAYNAME`** : Nom à afficher pour le compte de messagerie.
- **`EMAIL_SMTP_ACCOUNT_USERNAME`** : Nom du compte (ou adresse e-mail) à utiliser pour l'authentification sur le serveur SMTP.
- **`EMAIL_SMTP_ACCOUNT_PASSWORD`** : Mot de passe à utiliser pour l'authentification sur le serveur SMTP.
- **`EMAIL_SMTP_ACCOUNT_EMAIL`** : Adresse e-mail à utiliser comme expéditeur (doit être autorisée par le serveur SMTP).
- **`EMAIL_SMTP_ABUSE_EMAIL`** : Adresse e-mail pour signaler les abus.

### Exemple de fichier `config.json`

```json
{
    "EMAIL_SMTP_HOST": "SSL0.PROVIDER.NET",
    "EMAIL_SMTP_PORT": "2525",
    "EMAIL_SMTP_ENCRYPT": "tls",
    "EMAIL_SMTP_ACCOUNT_DISPLAYNAME": "Yesbabylon Symbiose",
    "EMAIL_SMTP_ACCOUNT_USERNAME": "account.username",
    "EMAIL_SMTP_ACCOUNT_PASSWORD": "password",
    "EMAIL_SMTP_ACCOUNT_EMAIL": "email.to.send.from@provider.com",
    "EMAIL_SMTP_ABUSE_EMAIL": "abuse@example.com"
}
```

## Templates

La configuration de templates permet de créer des modèles d’e-mails destinés aux clients. Chaque modèle est composé de plusieurs sections :  

- **Objet** : Définir le titre ou sujet de l'e-mail.  
- **Corps** : Rédiger le contenu principal du message.  
- **En-tête** (header) et **Pied de page** (footer) : Sections facultatives pour structurer l’e-mail.  

Ces modèles sont associés à une catégorie spécifique et à un type prédéfini, tels que :  

- Devis  
- Option  
- Contrat  
- Facture  
- Financement  

Par défaut, une catégorie de modèle est définie pour faciliter l’organisation.  

### Fichiers joints

Les modèles peuvent inclure des fichiers joints grâce à l’option "pièces jointes". Cela permet d’ajouter les documents nécessaires directement dans l’e-mail envoyé au client.  

### Traduction des Templates

Chaque partie d’un template doit être traduite dans les différentes langues prévues pour l’envoi.
Par défaut, la langue utilisée est celle définie par l’utilisateur dans les paramètres.  
Les traductions garantissent une communication adaptée aux préférences linguistiques des clients.  


## Alertes


### Modèle d'Alerte

Le modèle d'alerte définit la structure pour la gestion des alertes système. Les alertes jouent un rôle crucial dans le suivi et le traitement des processus, en particulier dans les systèmes de gestion des réservations. Chaque alerte est conçue pour notifier les utilisateurs des conditions ou erreurs spécifiques nécessitant une attention particulière.


Cette liste présente les alertes indispensables au bon fonctionnement du système de gestion des réservations :

- **Surbooking détecté** `lodging.booking.overbooking` :  
  Certaines unités locatives ne sont plus disponibles pour les dates spécifiées.
- **Liste de prix publiée** `lodging.booking.ready` :  
  La réservation est prête à être confirmée : le montant du devis se base sur une liste de prix publiée.
- **Composition incomplète** `lodging.booking.composition` :  
  La composition de la réservation est manquante ou incomplète.
- **Réservation vide** `lodging.booking.empty` :  
  La réservation ne comporte aucun service.
- **Option expirée** `lodging.booking.option.expired` :  
  L'option est expirée. La réservation est repassée en devis et les unités locatives associées ont été libérées.
- **Allocation incorrecte** `lodging.booking.rental_units_assignment` :  
  L'assignation des unités locatives du séjour est erronée : le nombre d'hôtes ne correspond pas.
- **Répartition des âges incorrecte** `lodging.booking.ages_assignment` :  
  La composition des âges des hôtes est erronée : le nombre d'hôtes ne correspond pas.
- **Incohérence logements** `lodging.booking.sojourns_accomodations` :  
  Un séjour ne contient pas de logement ; compte plus d'un type de logement ; ou contient un logement sans être un séjour ni un événement.
- **Erreur détectée** `lodging.booking.consistency` :  
  Un problème de cohérence a été détecté dans la réservation.
- **Facture invalide** `lodging.accounting.invoice.invalid` :  
  Une des lignes n'a pas de correspondance de prix ou de règle comptable.
- **Assignation de prix incorrecte** `lodging.booking.prices_assignment` :  
  Au moins un produit sélectionné n'a pas de prix défini pour la période correspondante.
- **Échec e-mail contrat** `lodging.booking.email.send` :  
  L'envoi du dernier e-mail de contact a échoué.
- **Unités locatives bloquées** `lodging.booking.quote.blocking` :  
  Cette réservation est en devis et bloque des unités locatives. 
- **Contrat non signé** `lodging.booking.contract.unsigned` :  
  Le contrat lié à la réservation n'a pas encore été marqué comme signé.
- **Vérifier les contacts** `lodging.booking.confirm` :  
  La réservation doit avoir au moins un contact avec un numéro de téléphone valide.
- **Paiement en excès** `lodging.booking.payment.overpaid` :  
  Il a été remarqué un paiement excédentaire de la part du client. Veuillez procéder au remboursement de l'excédent.
- **Données client incomplètes** `lodging.booking.customer.uncomplete` :  
  Des données client de facturation sont manquantes. Vérifiez les coordonnées et l'adresse du client.
- **Paiement en attente** `lodging.booking.payments` :  
  Un ou plusieurs paiements dus sont en retard pour cette réservation.
- **Divergence entre ouverture et fermeture** `lodging.pos.close-discrepancy` :  
  Une différence a été constatée entre le montant d'ouverture et le montant de fermeture de la caisse.

  
  