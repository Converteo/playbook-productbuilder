# Contribuer au Playbook Product Builder

Merci pour votre contribution.

## Modèle de branches et gouvernance

- `main` est la seule branche permanente.
- Il n’y a **pas** de branche `develop`.
- Les changements directs sur `main` sont interdits.
- Toute modification passe par une Pull Request.
- Seuls les mainteneurs peuvent fusionner.
- Les contributeurs externes peuvent contribuer via un fork.

Exemples de branches courtes :

- `content/add-new-page`
- `update/revise-existing-section`
- `fix/broken-link`

## Règles éditoriales

- Contenu en français.
- Encodage UTF-8.
- Titres en sentence case.
- Noms de fichiers en kebab-case.
- Toute affirmation factuelle doit citer des sources fiables.
- Vous devez disposer des droits de publication sur les textes/images soumis.
- Aucune information confidentielle Converteo ou client.
- Aucun contenu protégé sans autorisation.
- Toute contribution reste soumise à validation des mainteneurs.

## 1) Proposer une idée de contenu (Issue)

1. Ouvrez l’onglet **Issues**.
2. Choisissez le template **Content proposal**.
3. Renseignez le contexte, l’objectif, les lecteurs visés et les sources.
4. Soumettez l’Issue pour discussion.

## 2) Modifier une page via l’interface GitHub

1. Ouvrez le fichier Markdown à modifier.
2. Cliquez sur **Edit this file**.
3. Créez une branche.
4. Ouvrez une Pull Request avec le template proposé.

## 3) Contribuer via un fork

1. Forkez le dépôt.
2. Créez une branche courte depuis `main`.
3. Commitez vos changements dans votre fork.
4. Ouvrez une Pull Request vers `Converteo/playbook-productbuilder:main`.

## 4) Travailler en local

```bash
git clone https://github.com/Converteo/playbook-productbuilder.git
cd playbook-productbuilder
git checkout -b content/ma-contribution
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## 5) Prévisualiser le site MkDocs en local

```bash
mkdocs serve
```

Ouvrez ensuite <http://127.0.0.1:8000>.

Avant Pull Request :

```bash
yamllint .
mkdocs build --strict
```
