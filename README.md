# Playbook Product Builder

Le dépôt **Converteo Product Builder Playbook** prépare une base technique et
de gouvernance pour une documentation collaborative open source publiée avec
MkDocs.

Le contenu du playbook existe actuellement dans Coda et sera migré ensuite.
À ce stade, ce dépôt contient **uniquement le scaffold initial**.

## Objectif du dépôt

- Publier une documentation Markdown avec MkDocs + Material for MkDocs.
- Organiser la contribution interne/externe via Issues et Pull Requests.
- Appliquer une modération avant publication.
- Déployer automatiquement le site après fusion sur `main`.

Après migration depuis Coda, **GitHub devient la source de vérité** pour le
contenu.

## Lire, proposer, contribuer

- **Lire** : consultez le site publié (quand activé).
- **Ouvrir une Issue** : proposez une idée de contenu ou signalez une
  correction.
- **Soumettre une Pull Request** : proposez une modification concrète des
  fichiers Markdown.

Workflow de contribution :

`contribution → Pull Request → review → merge → deployment`

## Installation locale et prévisualisation

Prérequis : Python 3.12.

```bash
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Puis ouvrez <http://127.0.0.1:8000>.

Validation locale recommandée :

```bash
yamllint .
mkdocs build --strict
```

## Contribution

Consultez [`CONTRIBUTING.md`](CONTRIBUTING.md) pour les règles éditoriales,
le modèle de branches et les procédures détaillées.

## Important avant migration Coda

Ne créez pas de hiérarchie alternative (chapitres, sections, dossiers) tant
que la migration Coda n’est pas terminée.

## Configuration manuelle GitHub Pages

Dans les paramètres GitHub du dépôt, activez **Settings → Pages → Source: GitHub Actions**.
