# Financement

## Comptabilité

### Plan comptable
Le plan comptable est associé à une organisation et regroupe toutes les règles comptables qui lui sont liées. Par défaut, un plan comptable est défini pour correspondre à l'organisation par défaut.

### Règles de TVA 

La **Règle de TVA** permet de spécifier quel taux de TVA s'applique à un type d'opération donné, comme un achat ou une vente. Elle est utilisée dans le contexte de la gestion financière pour automatiser l'application des règles fiscales concernant la taxe sur la valeur ajoutée.

Propriétés principales :

1. **Nom** : Le nom de la règle de TVA.
2. **Taux** : Le taux de TVA associé à la règle.
3. **Type** : Le type d'opération auquel cette règle de TVA s'applique. 

Les règles de TVA* disponibles :

| **ID** | **Nom**            | **Taux** |
|--------|--------------------|----------|
| **1**  | Vente TVA 0%       | 0.00     |
| **2**  | Vente TVA 6%       | 0.06     |
| **3**  | Vente TVA 12%      | 0.12     |
| **4**  | Vente TVA 21%      | 0.21     |


### Règles comptables

La règle comptable permet de définir les critères pour l'imputation des opérations sur les comptes appropriés. Ces règles sont liées à des opérations spécifiques, comme les achats et les ventes, et peuvent inclure des lignes détaillant les différentes impositions ou ajustements. Cette classe comprend également des propriétés pour spécifier les règles fiscales associées et pour établir des relations avec les prix concernés par la règle.

Propriétés principales :

1. **Nom** : Nom de la règle comptable, utilisé pour identifier la règle.
2. **Description** : Brève description de la règle, qui sert de mémo pour l'utilisateur.
3. **Type** : Type d'opération auquel cette règle se rapporte, comme "achat" ou "vente".
4. **Lignes de règle comptable** : Référence vers les lignes détaillant les opérations comptables liées à cette règle.
5. **Règle de TVA** : Référence à la règle de TVA associée à cette ligne.
6. **Code historique** : Ancien nom de la règle comptable, pour la compatibilité avec des versions précédentes.

## Facture

### Facture

Une facture est un document légal émis par un vendeur à un acheteur qui concerne une vente, et fait partie du système comptable.

Propriétés principales :

1. **Nom** : Le nom de la facture.
2. **Organisation** : L'organisation qui a émis la facture.
3. **Équipe de gestion** : Le centre de gestion à l'origine de la facture.
4. **Client** : Le client associé à la facture.
5. **Statut** : Le statut actuel de la facture, tel que 'proforma', 'facture' ou 'annulée'.
6. **Type** : Le type de la facture, comme 'facture' ou 'note de crédit'.
7. **Date** : La date d'émission de la facture.
8. **Date d'échéance** : La date limite de paiement.
9. **Prix** : Le montant total facturé avec les taxes incluses.
10. **Total** : Le montant total de la facture, hors taxes.
11. **Solde** : Le montant restant à payer par le client.
12. **Lignes de facture** : Les lignes détaillées de la facture.
13. **Conditions de paiement** : Les conditions de paiement à appliquer à la facture.

### Ligne de facture

Une ligne de facture décrit les produits et les quantités qui font partie d'une facture. Chaque ligne représente un élément ou un service spécifique facturé, avec des informations sur le produit, la quantité, le prix unitaire, le taux de TVA, les remises et les montants totaux, tant avant qu'après l'application des taxes. Elle est reliée à une facture spécifique et peut être groupée avec d'autres lignes dans un groupe de lignes de facture. La ligne contient également des informations relatives aux paiements d'acompte, le cas échéant.

Propriétés principales :

1. **Nom** : Le libellé par défaut de la ligne, basé sur le produit.
2. **Facture** : La facture à laquelle la ligne est liée.
3. **Produit** : Le produit (SKU) auquel la ligne est associée.
4. **Prix unitaire** : Le prix unitaire du produit relatif à la ligne.
5. **Taux de TVA** : Le taux de TVA appliqué à la ligne.
6. **Quantité** : La quantité de produit associée à la ligne.
7. **Quantité gratuite** : La quantité gratuite associée à la ligne, si applicable.
8. **Remise** : Le montant total de la remise appliquée à la ligne, le cas échéant.
9. **Total** : Le prix total hors taxes de la ligne.
10. **Prix** : Le prix final de la ligne, taxes incluses.
