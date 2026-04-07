# Discope Documentation

Ce dépôt contient la documentation consolidée du projet **Discope PMS**.

Il s’agit d’un **fork du dépôt [`yesbabylon/doc`](https://github.com/yesbabylon/doc.git)**, utilisé comme base standardisée pour la construction et la publication de documentations MkDocs multi-sources.

---

## Principe d’architecture

Contrairement à une documentation classique, ce dépôt **ne contient pas directement l’ensemble des sources éditoriales**.

La documentation est construite dynamiquement à partir de plusieurs dépôts via un mécanisme d’assemblage défini dans :

```text
sources.yml
```

Chaque source décrit :

* un dépôt Git
* une branche
* un chemin de documentation (`doc/`, `docs/`, …)
* une cible d’intégration dans l’arborescence finale

### Exemple

```yaml
sources:
  - name: Discope
    repo: https://github.com/discope-pms/discope.git
    branch: main
    path: doc
    target: .

  - name: CPA-Lathus
    repo: https://github.com/discope-pms/discope.git
    branch: main
    path: lathus/doc
    target: lathus
```

---

## Pipeline de génération

La construction de la documentation repose sur le script :

```bash
./build.sh
```

Ce script :

1. clone les dépôts définis dans `sources.yml`
2. extrait les dossiers de documentation
3. assemble les contenus dans `docs/`
4. fusionne les fichiers `nav.yml`
5. génère dynamiquement la section `nav` de `mkdocs.yml`

La documentation résultante est ensuite prête à être servie ou buildée avec MkDocs.

---

## Structure du dépôt

```text
.
├── sources.yml     # définition des sources de documentation
├── build.sh        # script d’assemblage
├── mkdocs.yml      # configuration MkDocs (nav injecté dynamiquement)
└── docs/           # contenu généré (ne pas éditer manuellement)
```

---

## Prévisualisation locale

### 1. Installer les dépendances

```bash
pip install mkdocs mkdocs-material mike
```

### 2. Construire la documentation

```bash
./build.sh
```

### 3. Lancer le serveur

```bash
mkdocs serve
```

Accessible sur :

```text
http://127.0.0.1:8000
```

---

## Build statique

```bash
mkdocs build
```

Le site généré se trouve dans :

```text
site/
```

---

## Hébergement

Cette documentation est destinée à être déployée sur une instance **B2** :

```text
https://github.com/yesbabylon/b2
```

B2 est utilisé comme **serveur d’hébergement statique** pour exposer la documentation MkDocs générée.

Le workflow typique est :

1. build de la documentation (`mkdocs build`)
2. déploiement du contenu du dossier `site/`
3. exposition via l’instance B2

Ce modèle permet :

* un hébergement léger et sans dépendance runtime
* une séparation claire entre build et diffusion
* une intégration simple dans des pipelines CI/CD

---

## Convention importante

* Les sources de documentation doivent être maintenues **dans les dépôts applicatifs**
* Ce dépôt agit comme une **projection consolidée**
* Le dossier `docs/` est **généré automatiquement** et ne doit pas être modifié manuellement

---

## Héritage du template

Ce dépôt hérite du modèle fourni par :

```text
yesbabylon/doc
```

Ce template définit :

* la structure standard
* le mécanisme d’assemblage (`build.sh`)
* les conventions MkDocs
* le support multi-sources

