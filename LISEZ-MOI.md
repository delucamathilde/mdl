# Le site — mathildedeluca.com

Ce dossier est **la source exacte de ce qui est en ligne**. Tout ce que tu changes ici et
envoies sur GitHub apparaît sur le site en 1 à 2 minutes.

## Structure

```
site/
├── index.html         (accueil)
├── essays.html         (liste des essais)
├── poems.html          (page poèmes — vide pour l'instant, en noindex)
├── definitions.html    (mots inventés, dont "huniverse" — vide pour l'instant, en noindex)
├── images/              (les 3 images du site, ne pas renommer sans me le dire)
├── CNAME                (contient le nom de domaine, ne pas toucher)
├── robots.txt            (autorise Google à tout explorer)
├── sitemap.xml            (liste des pages à indexer)
├── llms.txt                (fiche d'identité pour les IA type ChatGPT/Claude)
└── LISEZ-MOI.md              (ce fichier)
```

Les anciennes versions du site (brouillons FR, ancienne version noire) sont rangées à part,
hors de ce dossier, dans `~/Documents/site-brouillons-anciens/` — elles ne sont pas en ligne.

## Comment publier un changement

Une fois qu'un fichier est modifié (par moi, ou par toi directement) :

```bash
cd ~/Documents/site
git add -A
git commit -m "description du changement"
git push
```

Le site se met à jour tout seul en ligne, en 1 à 2 minutes. Dis-le-moi et je m'en charge.

## Remplacer une image

Même nom de fichier exactement, déposée dans `images/`, puis publier (voir ci-dessus).

## Quand tu rempliras poems.html ou definitions.html

Deux choses à faire dans le fichier concerné :
1. Retire la ligne `<meta name="robots" content="noindex, follow">` dans le `<head>`.
2. Ajoute la page dans `sitemap.xml` (copie le bloc `<url>...</url>` de essays.html).

Dis-le-moi, je peux le faire pour toi.
