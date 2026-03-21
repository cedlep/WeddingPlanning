# 💒 Laury-Ann & Cédric — Site de mariage

Site web statique pour le mariage du **23 mai 2026**, déployé via **GitHub Pages**.

---

## 📁 Structure du projet

```
mariage-site/
│
├── index.html              ← Page d'accueil neutre (racine)
├── 404.html                ← Page d'erreur discrète
├── .nojekyll               ← Désactive Jekyll sur GitHub Pages
│
├── famille-amis/
│   └── index.html          ← Version complète (programme + soirée + voyage)
│
└── collegues/
    └── index.html          ← Version tronquée (jusqu'au vin d'honneur uniquement)
```

---

## 🌐 URLs après déploiement

| Audience | URL |
|---|---|
| Famille & amis | `https://[username].github.io/[repo]/famille-amis/` |
| Collègues | `https://[username].github.io/[repo]/collegues/` |

> Remplacez `[username]` par votre nom d'utilisateur GitHub et `[repo]` par le nom du dépôt.

---

## 🚀 Mise en ligne sur GitHub Pages — étape par étape

### 1. Créer le dépôt GitHub

1. Connectez-vous sur [github.com](https://github.com)
2. Cliquez sur **"New repository"**
3. Choisissez un nom, par exemple `mariage` (le dépôt peut être **privé** ou public)
4. Ne cochez rien d'autre, cliquez **"Create repository"**

### 2. Pousser les fichiers

Depuis votre terminal, dans le dossier du projet :

```bash
git init
git add .
git commit -m "Initial commit — site mariage"
git branch -M main
git remote add origin https://github.com/[username]/[repo].git
git push -u origin main
```

### 3. Activer GitHub Pages

1. Allez dans **Settings** → **Pages**
2. Sous **Source**, choisissez **"Deploy from a branch"**
3. Sélectionnez la branche **`main`** et le dossier **`/ (root)`**
4. Cliquez **Save**

Le site sera disponible en quelques minutes à l'adresse affichée.

### 4. Partager les liens

Transmettez uniquement le lien correspondant à chaque groupe :

- Aux **famille & amis** : `https://[username].github.io/[repo]/famille-amis/`
- Aux **collègues** : `https://[username].github.io/[repo]/collegues/`

---

## 🔒 Cloisonnement des versions

- Aucun lien ne relie les deux versions entre elles
- La page racine (`/`) affiche uniquement un message neutre
- La page `404.html` affiche le même message discret en cas d'URL incorrecte
- Aucun menu global, aucun sitemap exposant les deux URLs

---

## ✏️ Modifier le contenu

Tout le contenu est dans les deux fichiers HTML :
- `famille-amis/index.html`
- `collegues/index.html`

Après modification, poussez les changements :

```bash
git add .
git commit -m "Mise à jour du contenu"
git push
```

GitHub Pages se met à jour automatiquement en 1 à 2 minutes.

---

## 🎨 Stack technique

- HTML5 / CSS3 / JavaScript vanilla
- Polices : Cormorant Garamond + Jost (Google Fonts)
- Aucune dépendance externe, aucun framework
- Optimisé mobile-first
