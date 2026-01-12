# Template de site web pour IFT3150 (Projet informatique)

Ce répertoire contient un template de site web de projet pour le cours IFT3150, construit avec [MkDocs](https://www.mkdocs.org/) et le thème [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

Ce site sert à :

- documenter le projet tout au long de la session,
- structurer les livrables (description, suivi, résumé, rapport),
- centraliser le travail de l’équipe dans un format clair et accessible.

## Prérequis

Assurez-vous d’avoir les outils suivants installés :

- Python **3.11** ou plus récent
- `pip` (gestionnaire de paquets Python)

## Installation

1. Clonez ce dépôt (optionnel) :
```bash
git clone git@github.com:udem-diro/template-projet.git
```

2. Installez les dépendances (dans votre répertoire) :
```bash
pip install -r requirements.txt
```

## Utilisation

Vous devez au minimum :

1. Modifier les pages (fichiers) Markdown dans le dossier `docs/`
2. Compléter les sections prévues (ex: description, suivi, résumé, rapport)
3. Adapter le contenu à votre projet

### Travailler en local (sur votre poste)

Pour lancer un serveur local avec rechargement automatique :

```bash
mkdocs serve --livereload
```

Le site sera accessible à l'adresse [http://127.0.0.1:8000](http://127.0.0.1:8000).

> Après chaque modification de fichiers dans `/docs`, le site local est automatiquement mis à jour.

### Construction du site (optionnel)

Pour générer la version statique du site :

```bash
mkdocs build
```

Les fichiers générés seront placés dans le dossier `site/`.

### Déployer ou mettre à jour le site (public)

Pour déployer le site sur GitHub Pages :

```bash
mkdocs gh-deploy
```

> Cette commande pousse automatiquement le contenu du site sur la branche `gh-pages`.

## Structure du projet

```sh
.
├── docs/                # Contenu du site (Markdown)
│   ├── index.md         # Vue d’ensemble du projet
│   ├── suivi.md         # Suivi détaillé (hebdo / bi-hebdo)
│   ├── resume.md        # Résumé final du projet
│   └── rapport/         # Rapport final (sections)
├── mkdocs.yml           # Configuration du site et navigation
├── requirements.txt     # Dépendances Python
└── site/                # Site généré (créé lors de la construction)
```

> Tout le contenu du projet se trouve dans `docs/`.

## Personnalisation

1. Modifiez `mkdocs.yml` pour changer la configuration du site
2. Ajoutez/modifiez les fichiers Markdown (`.md`) dans `docs/`
3. Personnalisez le thème en modifiant les paramètres dans `mkdocs.yml`

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## 🙋‍♀️ Questions ou problèmes ?

En cas de problème, n'hésitez pas à ouvrir une issue sur GitHub ou à poser des questions au coordonnateur du cours.
