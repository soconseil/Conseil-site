# Site de conseil — Hugo + PaperMod (0€, sans terminal)

**Aucune commande à taper.** Tu vas juste **glisser-déposer** les fichiers sur GitHub.

## Étapes
1. Sur GitHub, crée un dépôt **public** nommé `conseil-site` (repo vide).
2. Clique **Add file → Upload files**.
3. Depuis le ZIP, **sélectionne TOUT le dossier** `conseil-site-no-terminal` (ou tous ses fichiers) et **glisse-dépose** sur la page d’upload.
4. Clique **Commit changes** (en bas).  
5. Va dans **Settings → Pages** : l’URL de ton site apparaîtra quand le déploiement est fini.
   - Tu peux suivre le déploiement dans l’onglet **Actions** (job *Deploy Hugo site to Pages*).
6. Personnalise le contenu : modifie `config.toml` (titre, email, LinkedIn) et les fichiers dans `content/` directement depuis GitHub (bouton **Edit**).

## Pourquoi ça marche sans terminal ?
Le fichier `.github/workflows/hugo.yml` **télécharge le thème PaperMod automatiquement** pendant le build (étape *Fetch PaperMod theme*). Pas besoin de Git submodules ni de commandes locales.

## Où modifier quoi
- `config.toml` → `title`, `label.text`, liens `mailto:` et LinkedIn, texte d’accueil.
- `content/` → pages et articles.
- `static/favicon.svg` → icône du site.

Bon build !