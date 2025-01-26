# Paramètres

## Locale

- **Séparateur de milliers** (`numbers.thousands_separator`) : Détermine le caractère utilisé comme séparateur de milliers dans les nombres.
- **Position de devise** (`currency.symbol_position`) : Indique la position du symbole de la monnaie par rapport à la valeur.
- **Nombre de décimales (Prix)** (`currency.decimal_precision`) : Nombre de décimales utilisées pour afficher les prix.
- **Séparateur de décimales** (`numbers.decimal_separator`) : Détermine le type de séparateur décimal utilisé.
- **Nombre de décimales** (`numbers.decimal_precision`) : Définit le nombre de décimales à afficher pour les nombres.
- **Format de date** (`date_format`) : Format utilisé pour afficher la date.
- **Format des heures** (`time_format`) : Format utilisé pour afficher l'heure.

### Général

- **Entreprise** (`company.id`) : Identifiant de l'entreprise principale de l'installation courante.
- **Format du papier** (`formats.paper`) : Taille du papier par défaut pour l'impression des documents.

### Sécurité

- **Création de compte** (`account_creation`) : Permet aux visiteurs de créer un compte utilisateur (*vrai* / *faux*).
- **Importation de données** (`import`) : Autorise les utilisateurs à importer des données à partir de fichiers (*vrai* / *faux*).
- **Exportation de données** (`export`) : Autorise les utilisateurs à exporter des données vers des fichiers (*vrai* / *faux*).

### Unités de mesure

- **Devise** (`currency`) : Devise à utiliser pour les champs à usage 'Price' (ISO 4217).
- **Longueur** (`length`) : Unité par défaut pour les mesures de longueur.
- **Poids** (`weight`) : Unité par défaut pour les mesures de poids (par exemple, 'kg' pour kilogramme, 'lb' pour livre).
- **Volume** (`volume`) : Unité par défaut pour les unités de volume (par exemple, 'm3' pour mètre cube, 'ft3' pour pied cube).
- **Surface** (`surface`) : Unité par défaut pour les unités de surface (par exemple, 'm2' pour mètre carré, 'ft2' pour pied carré).

## Ventes

### Facturation

- **Séquence de facturation** (`invoice.sequence.1`) : Séquence utilisée pour la numérotation des factures dans le système de facturation.
- **Factures d'acompte** (`downpayment.enable`) : Active ou désactive la possibilité d'émettre des factures d'acompte.
- **Produit pour les acomptes** (`downpayment.sku.1`) : Le SKU à utiliser pour les factures d'acompte.

### Réservation

- **Format de réservation** (`booking.sequence_format`) : Format de la numérotation des réservations.
- **Jours de validité d'une option** (`option.validity`) : Nombre de jours pendant lesquels une option est valide.
- **Délai de rappel d'une offre** (`quote.remind_delay`) : Délai en jours avant d'envoyer un rappel après l'envoi de devis.

### Locale

- **Traduction du terme "contrat"** (`terms.contract`)
- **Traduction du terme "facture"** (`terms.invoice`)
- **Traduction du terme "acompte"** (`terms.downpayments`)
- **Traduction du terme "versement"** (`terms.installment`)
- **Traduction du terme "devis"** (`terms.quote`)

## Financement

### Facturation

- **Année comptable** (`fiscal_year`) : Année courante d'exercice comptable.
- **Format de séquence des factures finance** (`invoice.invoice.sequence_format`) : Format de séquence pour les factures (selon les conventions comptables).
- **Numéro du compte pour les acomptes** (`downpayment.account`) : Code de compte dans le plan comptable pour les acomptes.
- **Compte de vente** (`account.sales`) : Numéro du compte à utiliser pour les écritures de ventes et prestations de services.
- **Taxes à payer** (`account.sales_taxes`) : Numéro du compte à utiliser pour les taxes dues sur les ventes.
- **Compte des créances commerciales** (`account.trade_debtors`) : Numéro du compte à utiliser pour les écritures de créances commerciales.

## Configuration

Le fichier config.json permet de configurer le fuseau horaire et la langue de l'application. Ces paramètres sont cruciaux pour adapter l'application aux préférences régionales des utilisateurs.

### Fuseau Horaire 
Le fuseau horaire de l’application est défini dans le paramètre `L10N_TIMEZONE`. Ce paramètre suit le format `"Continente/Ville"` pour indiquer la zone horaire. 

Par exemple, pour le fuseau horaire de Bruxelles, la configuration serait la suivante :

```json
"L10N_TIMEZONE": "Europe/Brussels",
```

### Langue 
La langue est définie par le paramètre `DEFAULT_LANG `et a niveau local `L10N_LOCALE`. 

Discope permet de définir trois langues:

- **Français** : fr
- **Néerlandais** :nl
- **Anglais** : en

        
Exemple de config.json

```json
{
    "DEFAULT_LANG": "fr",
    "L10N_TIMEZONE": "Europe/Brussels",
    "L10N_LOCALE": "fr"
}
```