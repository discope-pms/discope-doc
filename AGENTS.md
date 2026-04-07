# Instructions pour agents IA – Documentation Discope

## 1. Contexte général

Tu es un **agent IA** travaillant sur la documentation de l’application **Discope**.
La documentation est gérée avec **MkDocs** et est stockée dans ce dépôt.

- **Répertoire de documentation** : `./docs`
- **Configuration de navigation** : `mkdocs.yml` (clé `nav`)
- **Langue** : **Français uniquement**
- **Outil de génération** : MkDocs

Ton rôle est de créer, modifier et organiser les fichiers de documentation conformément aux règles définies ci-dessous.

---

## 2. Règles d’écriture

1. **Langue** : Toujours écrire en **français clair** et précis.
2. **Titres** :
   - Mkdocs ajoute toujours automatiquement un titre de niveau 1 (`<h1>`) correspondant à `# Nom de la page`, sur base du nom de la page en cours, le premier niveau à utiliser est donc toujours le niveau 2 (`## Titre`);
   - Il peut y avoir plusieurs titres de niveau 2 sur une même page, puisqu'ils se rapportent toujours à la page en cours, qui est considérée comme niveau 1;
   - Les sous-sections de niveau 3 et suivants, utilisent les niveaux hiérarchiques suivants (`###`, `####`).
3. **Style** :
   - Phrases courtes et lisibles.
   - Vocabulaire cohérent avec le reste de la documentation.
   - Explications factuelles, sans opinion personnelle.
4. **Orthographe et typographie** :
   - Respecter la typographie française (espaces insécables, ponctuation).
   - Pas de fautes d’orthographe.

---

## 3. Structure des fichiers

- **Emplacement** : Tous les fichiers `.md` doivent être placés dans `./docs` ou ses sous-dossiers.
- **Nommage** :
  - Nom en minuscules et en anglais
  - Sans accents ni espaces (remplacer par `_` ou `-`).
  - Exemples valides : `installation.md`, `user_guide.md`
- **Liens internes** :
  - Utiliser des liens relatifs : `[Nom](../path/file.md)`.
  - Vérifier que le lien fonctionne après modification.

---

## 4. Mise à jour de `mkdocs.yml`

- La clé `nav` définit la navigation du site.
- Chaque fichier ajouté doit être inscrit dans `mkdocs.yml` avec un libellé clair.
- Exemple :
  ```yaml
  nav:
    - Accueil: index.md
    - Guide utilisateur:
        - Installation: guide/installation.md
        - Utilisation: guide/utilisation.md

------

## 5. Actions autorisées pour l’agent IA

✅ Ajouter de nouveaux fichiers Markdown dans `./docs`.
✅ Modifier du contenu existant pour corriger ou améliorer la clarté.
✅ Réorganiser les titres et sections pour plus de lisibilité.
✅ Ajouter les nouveaux fichiers dans `mkdocs.yml`.
✅ Corriger les liens internes cassés.
✅ Harmoniser le style et la terminologie.

------

## 6. Actions interdites pour l’agent IA

❌ Supprimer un fichier sans instruction explicite.
❌ Modifier la configuration de MkDocs hors de la section `nav`.
❌ Changer la langue du contenu (doit rester en français).
❌ Réécrire le contenu avec un ton marketing ou subjectif.
❌ Ajouter des informations non vérifiées ou inventées.

------

## 7. Bonnes pratiques

- **Prévisualisation** : Toujours vérifier le rendu avec `mkdocs serve` avant validation.
- **Concision** : Supprimer les répétitions inutiles.
- **Contexte métier** : Utiliser le vocabulaire et les concepts propres à Discope.
- **Homogénéité** : S’aligner sur la structure et le style des autres pages.
- **Historique clair** : Chaque commit doit avoir un message descriptif.

------

## 8. Exemple d’intervention

**Tâche** : Ajouter une page "FAQ" avec 3 questions fréquentes.

1. Créer le fichier : `./docs/faq.md`

   ```markdown
   # Foire aux questions (FAQ)

   ## Qu'est-ce que Discope ?
   Discope est une application permettant de [...]

   ## Comment installer Discope ?
   Suivez les étapes décrites dans [Installation](guide/installation.md).

   ## Où trouver l'assistance ?
   Contactez l'équipe via [...]
   ```

2. Mettre à jour `mkdocs.yml` :

   ```yaml
   nav:
     - Accueil: index.md
     - FAQ: faq.md
   ```

3. Vérifier que le lien fonctionne et que le style est homogène avec les autres pages.

------

**Note** : Ces instructions sont permanentes et doivent être respectées pour toute intervention IA sur ce dépôt.

