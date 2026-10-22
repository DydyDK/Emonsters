# Emonsters

*Apprivoiser ses émotions, ensemble.*

Emonsters est un jeu web où chacun crée le monstre d’une émotion difficile, explore La Clairière, répond à des questions de psychologie pour progresser et affronte le Donjon de l’Imposteur. Boby, le cyclope noir à la bouche orange, en est la mascotte.

Le jeu tient en un seul fichier HTML (JavaScript, Canvas et SVG), sans serveur ni installation : il tourne directement sur GitHub Pages.

## Contenu du dépôt

| Chemin | Contenu |
| --- | --- |
| `index.html` | Le jeu : écran d’accueil, créateur de monstre, La Clairière, Donjon de l’Imposteur |
| `docs/gdd/` | Game Design Documents v1 et v2 (Word) |

## Mettre le jeu en ligne avec GitHub Pages

1. Sur GitHub, crée un nouveau dépôt (par exemple `emonsters`).
2. Dans le dépôt vide, clique sur **Add file › Upload files** et glisse **le contenu** du dossier `emonsters` (pas le dossier lui-même), y compris le fichier caché `.nojekyll`. Valide avec **Commit changes**.
3. Va dans **Settings › Pages**, choisis **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après une à deux minutes, le jeu est disponible à l’adresse `https://<ton-pseudo>.github.io/emonsters/`.

Les libellés exacts de l’interface GitHub peuvent varier légèrement.

## Bon à savoir

- **Sauvegardes** : la progression est enregistrée dans le navigateur (`localStorage`). Chaque joueur a ses propres sauvegardes, liées à son navigateur et à l’adresse du site.
- **La Capitale** : elle est mise de côté pour le moment. Le jeu contient encore un appel vers `boby_capitale.html`, absent du dépôt.
- **Police** : le jeu charge Fredoka depuis Google Fonts ; hors connexion, une police de secours s’affiche.
- **Visibilité** : un dépôt public rend aussi les GDD publics. Pour les garder confidentiels, retire le dossier `docs/` ou passe le dépôt en privé (GitHub Pages sur un dépôt privé nécessite un abonnement payant).

## Tester en local

Ouvre `index.html` dans ton navigateur, ou lance un petit serveur depuis le dossier :

```bash
python3 -m http.server 8000
```

puis ouvre `http://localhost:8000`.

© 2026 Emonsters
