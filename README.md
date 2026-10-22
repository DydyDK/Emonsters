# Emonsters

*Apprivoiser ses émotions, ensemble.*

Emonsters est un jeu web où chacun crée le monstre d’une émotion difficile, explore un monde ouvert, répond à des questions de psychologie pour progresser et traverse des donjons émotionnels. Boby, le cyclope noir à la bouche orange, en est la mascotte.

Le projet est 100 % statique (HTML, JavaScript, SVG), sans serveur ni installation : il tourne directement sur GitHub Pages.

## Contenu du dépôt

| Chemin | Contenu |
| --- | --- |
| `index.html` | Page d’accueil : bouton pour lancer le jeu et les deux affiches |
| `jeu/boby_onboarding.html` | Le jeu : onboarding, créateur de monstre, La Clairière, Donjon de l’Imposteur |
| `affiches/version-boby.html` | Affiche cartouche Nº 01, le gentil (Boby) |
| `affiches/version-murmure.html` | Affiche cartouche Nº 02, le méchant (Murmure) |
| `docs/gdd/` | Game Design Documents v1 et v2 (Word) |


## Mettre le projet en ligne avec GitHub Pages

1. Sur GitHub, crée un nouveau dépôt (par exemple `emonsters`).
2. Dans le dépôt vide, clique sur **Add file › Upload files** et glisse **le contenu** du dossier `emonsters` (pas le dossier lui-même), y compris le fichier caché `.nojekyll`. Valide avec **Commit changes**.
3. Va dans **Settings › Pages**, choisis **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après une à deux minutes, le site est disponible à l’adresse `https://<ton-pseudo>.github.io/emonsters/`.

Les libellés exacts de l’interface GitHub peuvent varier légèrement.

## Bon à savoir

- **Sauvegardes** : le jeu enregistre la progression dans le navigateur (`localStorage`). Chaque joueur a donc ses propres sauvegardes, liées à son navigateur et à l’adresse du site.
- **Polices** : les affiches et la page d’accueil chargent Unbounded, IBM Plex Mono et Nunito depuis Google Fonts. Hors connexion, une police de secours s’affiche.
- **Visibilité** : un dépôt public rend aussi les documents de conception (GDD) publics. Si tu veux les garder confidentiels, retire le dossier `docs/` ou passe le dépôt en privé (GitHub Pages sur un dépôt privé nécessite un abonnement payant).
- **Licence** : aucune licence n’est incluse. Sans licence, le code reste protégé par défaut ; ajoutes-en une si tu veux autoriser la réutilisation.

## Tester en local

Ouvre `index.html` dans ton navigateur. Pour un comportement identique à GitHub Pages, lance un petit serveur depuis le dossier :

```bash
python3 -m http.server 8000
```

puis ouvre `http://localhost:8000`.

© 2026 Emonsters
