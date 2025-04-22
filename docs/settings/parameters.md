# Paramètres



## Tableaux récapitulatifs



### Sections disponibles

| d    | Section                   | Functional Name                   | Main Usage                                                   |
| ---- | ------------------------- | --------------------------------- | ------------------------------------------------------------ |
| 1    | `locale`                  | 🌍 Localization & Compliance       | Formats, timezones, languages, currencies, units & measures  |
| 2    | [`main`] → `organization` | (deprecated)                      |                                                              |
| 3    | `security`                | 🔐 Security & Access Control       | Auth, MFA, roles, sessions, audit logs                       |
| 4    | [`units`] → `locale`      | (deprecated)                      |                                                              |
| 5    | `accounting`              | 🧾 Accounting (not only financial) | Sequences, accounts, VAT, billing logic                      |
| 11   | `analytics`               | 📈 Reporting & Analytics           | Logs, metrics, KPIs, scheduled reports                       |
| 12   | `features`                | 💬 Customization & UI              | Labels, UI settings, templates                               |
| 13   | `storage`                 | 📦 Storage & Data                  | File paths, quotas, persistence                              |
| 14   | `integration`             | 🔄 Integrations & Connectors       | APIs, tokens, endpoints, webhooks                            |
| 15   | `system`                  | 🛠️ Technical & Maintenance         | Debug mode, technical notifications, versions                |
| 16   | `workflow`                | 📐 Business Logic & Processes      | Statuses, transitions, automation rules                      |
| 17   | `schedule`                | ⏱️ Scheduling & Time Config        | Calendars, working hours, cron jobs                          |
| 18   | `organization`            | 🏢 Structure & Organization        | Internal org setup that do not fit within Organization entity<br />Entities, departments, fiscal/HR periods |

### Paramètres définis 

| Setting Key                                             | Description                                                  |
| ------------------------------------------------------- | ------------------------------------------------------------ |
| discope.features.custom_package                         |                                                              |
| discope.features.has_custom_package                     |                                                              |
| finance.accounting.account.discount                     |                                                              |
| finance.accounting.account.downpayment                  |                                                              |
| finance.accounting.account.sales                        |                                                              |
| finance.accounting.account.sales_taxes                  |                                                              |
| finance.accounting.account.trade_debtors                |                                                              |
| finance.accounting.fiscal_year                          |                                                              |
| finance.accounting.fiscal_year.date_from                |                                                              |
| finance.accounting.fiscal_year.date_to                  |                                                              |
| finance.accounting.invoice.export_type                  |                                                              |
| identity.accounting.customer_account.prefix             |                                                              |
| identity.accounting.customer_account.sequence           |                                                              |
| identity.accounting.customer_account.sequence_format    |                                                              |
| identity.organization.country_default                   | pays par défaut (pour les identités)                         |
| lodging.locale.i18n.activities_details                  |                                                              |
| lodging.locale.i18n.activity                            |                                                              |
| lodging.locale.i18n.activity_schedule                   |                                                              |
| lodging.locale.i18n.advantage                           |                                                              |
| lodging.locale.i18n.advantage_included                  |                                                              |
| lodging.locale.i18n.already_paid                        |                                                              |
| lodging.locale.i18n.amount                              |                                                              |
| lodging.locale.i18n.amount_to_be_refunded               |                                                              |
| lodging.locale.i18n.balance_of                          |                                                              |
| lodging.locale.i18n.booking_contract                    |                                                              |
| lodging.locale.i18n.booking_invoice                     |                                                              |
| lodging.locale.i18n.booking_quote                       |                                                              |
| lodging.locale.i18n.booking_ref                         |                                                              |
| lodging.locale.i18n.children                            |                                                              |
| lodging.locale.i18n.communication                       |                                                              |
| lodging.locale.i18n.company_registry                    |                                                              |
| lodging.locale.i18n.consumptions_details                |                                                              |
| lodging.locale.i18n.credit_note                         |                                                              |
| lodging.locale.i18n.customer_address                    |                                                              |
| lodging.locale.i18n.customer_name                       |                                                              |
| lodging.locale.i18n.customer_num                        |                                                              |
| lodging.locale.i18n.date                                |                                                              |
| lodging.locale.i18n.date_and_signature                  |                                                              |
| lodging.locale.i18n.day                                 |                                                              |
| lodging.locale.i18n.discount_short                      |                                                              |
| lodging.locale.i18n.downpayments                        |                                                              |
| lodging.locale.i18n.email                               |                                                              |
| lodging.locale.i18n.fare_category                       |                                                              |
| lodging.locale.i18n.freebies_short                      |                                                              |
| lodging.locale.i18n.installment                         |                                                              |
| lodging.locale.i18n.invoice                             |                                                              |
| lodging.locale.i18n.left_to_pay                         |                                                              |
| lodging.locale.i18n.meal_evening                        |                                                              |
| lodging.locale.i18n.meals                               |                                                              |
| lodging.locale.i18n.meals                               |                                                              |
| lodging.locale.i18n.meals_midday                        |                                                              |
| lodging.locale.i18n.meals_morning                       |                                                              |
| lodging.locale.i18n.member                              |                                                              |
| lodging.locale.i18n.must_be_paid_before                 |                                                              |
| lodging.locale.i18n.nights                              |                                                              |
| lodging.locale.i18n.no                                  |                                                              |
| lodging.locale.i18n.number_short                        |                                                              |
| lodging.locale.i18n.origin                              |                                                              |
| lodging.locale.i18n.paid                                |                                                              |
| lodging.locale.i18n.payment                             |                                                              |
| lodging.locale.i18n.payments_history                    |                                                              |
| lodging.locale.i18n.payments_schedule                   |                                                              |
| lodging.locale.i18n.people                              |                                                              |
| lodging.locale.i18n.period                              |                                                              |
| lodging.locale.i18n.price                               |                                                              |
| lodging.locale.i18n.price_tax_excl                      |                                                              |
| lodging.locale.i18n.product_label                       |                                                              |
| lodging.locale.i18n.quantity_short                      |                                                              |
| lodging.locale.i18n.quote                               |                                                              |
| lodging.locale.i18n.received                            |                                                              |
| lodging.locale.i18n.snack                               |                                                              |
| lodging.locale.i18n.status                              |                                                              |
| lodging.locale.i18n.stay_total_tax_incl                 |                                                              |
| lodging.locale.i18n.taxes                               |                                                              |
| lodging.locale.i18n.the_amount_of                       |                                                              |
| lodging.locale.i18n.time_slot                           |                                                              |
| lodging.locale.i18n.to_be_paid_before                   |                                                              |
| lodging.locale.i18n.to_pay                              |                                                              |
| lodging.locale.i18n.to_refund                           |                                                              |
| lodging.locale.i18n.total                               |                                                              |
| lodging.locale.i18n.total_tax_excl                      |                                                              |
| lodging.locale.i18n.total_tax_incl                      |                                                              |
| lodging.locale.i18n.unit_price                          |                                                              |
| lodging.locale.i18n.vat                                 |                                                              |
| lodging.locale.i18n.vat_number                          |                                                              |
| lodging.locale.i18n.yes                                 |                                                              |
| lodging.locale.i18n.your_reference                      |                                                              |
| lodging.locale.i18n.your_stay_at                        |                                                              |
| sale.accounting.invoice.downpayment_account             |                                                              |
| sale.accounting.invoice.sequence                        |                                                              |
| sale.accounting.invoice.sequence.1                      |                                                              |
| sale.accounting.invoice.sequence_format                 |                                                              |
| sale.features.booking.activity                          | Active les fonctionnalités liés à la gestion des  activités  |
| sale.features.booking.activity_schedule_table           | assignation alternative des activités (vue en tableau)       |
| sale.features.booking.archive_delay                     |                                                              |
| sale.features.booking.channel_manager                   | Active les fonctionnalités lées à l'utilisation d'un  channel manager |
| sale.features.booking.checkin.default                   | Heure de checkin par défaut pour les réservations            |
| sale.features.booking.checkout.default                  | Heure de checkout par défaut pour les réservations           |
| sale.features.booking.consumption_meters                | relevés de compteurs de consommation                         |
| sale.features.booking.employee_planning                 | planning des employés                                        |
| sale.features.booking.employee_planning                 | planning des employés                                        |
| sale.features.booking.loyalty_points                    | gestion des points de fidélité                               |
| sale.features.booking.loyalty_points                    | gestion des points de fidélité                               |
| sale.features.booking.meal                              |                                                              |
| sale.features.booking.tasks_table                       | utilisation du tableau de suivi pour les tâches liées  à une réservation |
| sale.features.booking.tasks_table                       | utilisation du tableau de suivi pour les tâches liées  à une réservation |
| sale.features.contract.remind_auto                      | rappels auto pour les contrats                               |
| sale.features.contract.remind_delay                     |                                                              |
| sale.features.employee.activity_filter                  | filtrage par activité                                        |
| sale.features.invoice.downpayment                       |                                                              |
| sale.features.invoice.remind_auto                       | rappels auto pour les factures                               |
| sale.features.invoice.remind_delay                      |                                                              |
| sale.features.option.remind_auto                        | rappels auto pour les options                                |
| sale.features.option.remind_delay                       |                                                              |
| sale.features.option.validity_delay                     |                                                              |
| sale.features.payment.bank_check                        | Active les fonctionnalités liées aux paiements par  chèque bancaire |
| sale.features.payment.financial_help                    | Active les fonctionnalités liées à la gestion des  aides financières |
| sale.features.payment.instant                           | Active les fonctionnalités liées paiement rapide  (caisse)   |
| sale.features.quote.remind_auto                         | rappels auto pour les devis                                  |
| sale.features.quote.remind_delay                        |                                                              |
| sale.features.quote.validity_delay                      |                                                              |
| sale.features.templates.quote.activities                |                                                              |
| sale.features.templates.quote.consumption_table         | Affichage du récap des consommations dans les devis          |
| sale.features.ui.booking.accommodations_folded          | Affichage plié de l’écran "logements"  (unités locatives)    |
| sale.features.ui.booking.activities_folded              | Affichage plié de l’écran "activités"                        |
| sale.features.ui.booking.identification_folded          | Affichage plié de l’écran "identification"  (groupe de service) |
| sale.features.ui.booking.meals_folded                   | Affichage plié de l’écran "repas"                            |
| sale.features.ui.booking.products_folded                | Affichage plié de l’écran "produits"                         |
| sale.features.ui.booking.store_folded_settings          | Stockage de l'état de pli/dépli des sections du côté  client |
| sale.organization.age_range_default                     |                                                              |
| sale.organization.booking.channel_manager.client_domain |                                                              |
| sale.organization.booking.reference_type                | type de communication pour les virements                     |
| sale.organization.booking.sequence                      |                                                              |
| sale.organization.booking.sequence.1                    |                                                              |
| sale.organization.booking.sequence_format               |                                                              |
| sale.organization.contract.output_level_default         |                                                              |
| sale.organization.customer.number_assignment            |                                                              |
| sale.organization.customer.number_format                |                                                              |
| sale.organization.invoice.output_level_default          |                                                              |
| sale.organization.option.output_level_default           |                                                              |
| sale.organization.payment_terms_default                 | conditions de paiement par défaut                            |
| sale.organization.quote.output_level_default            |                                                              |
| sale.organization.sku.bed_linens                        |                                                              |
| sale.organization.sku.downpayment.1                     |                                                              |
| sale.organization.sku.make_beds                         |                                                              |
| sale.organization.sku.transport                         |                                                              |




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

Le fichier `config.json` permet de configurer le fuseau horaire et la langue de l'application. Ces paramètres sont cruciaux pour adapter l'application aux préférences régionales des utilisateurs.

### Fuseau Horaire 
Le fuseau horaire de l’application est défini dans le paramètre `L10N_TIMEZONE`. Ce paramètre suit le format `"Continente/Ville"` pour indiquer la zone horaire. 

Par exemple, pour le fuseau horaire de Bruxelles, la configuration serait la suivante :

```json
"L10N_TIMEZONE": "Europe/Brussels",
```

### Langue 

La langue est définie par le paramètre `DEFAULT_LANG `et a niveau local `L10N_LOCALE`. 

Discope permet le choix parmi trois langues:

- **Français** : fr
- **Néerlandais** :nl
- **Anglais** : en

  ​      

Exemple de `config.json`

```json
{
    "DEFAULT_LANG": "fr",
    "L10N_TIMEZONE": "Europe/Brussels",
    "L10N_LOCALE": "fr"
}
```