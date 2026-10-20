# dewiweb.github.io

Site personnel construit avec [Hugo](https://gohugo.io/) et le thème [Hextra](https://imfing.github.io/hextra/), publié sur GitHub Pages : <https://dewiweb.github.io>

## Prérequis

- Hugo **extended** ≥ 0.112 (testé avec 0.140.0)
- Go ≥ 1.20 (nécessaire au chargement du thème via les modules Hugo)

## Développement local

```bash
hugo server -D
```

Le site est accessible sur <http://localhost:1313>.

## Build

```bash
hugo --gc --minify
```

Le site statique est généré dans `public/`.

## Structure

- `content/fr/` — pages en français (langue par défaut, à la racine)
- `content/en/` — pages en anglais (sous `/en/`)
- `hugo.yaml` — configuration du site
- `layouts/` — gabarits et shortcodes locaux
- `static/` — fichiers statiques (images)

## Déploiement

Le workflow GitHub Actions (`.github/workflows/deploy.yml`) compile le site
sur chaque pull request et sur chaque push vers `main`, puis publie `public/`
sur la branche `gh-pages` via GitHub Pages.
