# 📊 Portfolio Live Dashboard

Dashboard interactif pour suivre votre portefeuille d'investissements, hébergé gratuitement sur GitHub Pages.

## 🚀 Mise en place (10 minutes)

### Étape 1 — Créer le repo GitHub

1. Allez sur [github.com/new](https://github.com/new)
2. Nom du repo : `portfolio` (ou ce que vous voulez)
3. Cochez **Public** (requis pour GitHub Pages gratuit)
4. Cliquez **Create repository**

### Étape 2 — Uploader le fichier

1. Dans votre nouveau repo, cliquez **Add file → Upload files**
2. Glissez-déposez le fichier `index.html` (le dashboard)
3. Cliquez **Commit changes**

### Étape 3 — Activer GitHub Pages

1. Allez dans **Settings → Pages** (menu de gauche)
2. Source : **Deploy from a branch**
3. Branch : **main** / dossier **/ (root)**
4. Cliquez **Save**
5. Attendez ~1 minute, votre site est en ligne à :
   ```
   https://VOTRE-USERNAME.github.io/portfolio/
   ```

### Étape 4 — Configurer l'URL de l'API

Ajoutez votre URL Apps Script en paramètre dans l'URL :

```
https://VOTRE-USERNAME.github.io/portfolio/?api=https://script.google.com/macros/s/AKfycb.../exec
```

**Astuce** : cette URL complète (avec le `?api=...`) est celle que vous ajouterez en favori / sur l'écran d'accueil.

### Étape 5 — Ajouter à l'écran d'accueil du téléphone

**iPhone (Safari) :**
1. Ouvrez l'URL complète (avec `?api=...`) dans Safari
2. Appuyez sur le bouton **Partager** (carré avec flèche)
3. Choisissez **Sur l'écran d'accueil**
4. Nommez-le "Portfolio" → **Ajouter**

**Android (Chrome) :**
1. Ouvrez l'URL complète dans Chrome
2. Menu ⋮ → **Ajouter à l'écran d'accueil**
3. Nommez-le "Portfolio" → **Ajouter**

## ✅ C'est fait !

Votre dashboard se lance comme une app, se rafraîchit toutes les 5 minutes, et lit les données live de votre Google Sheet.

## 🔄 Mettre à jour le dashboard

Si je vous fournis une nouvelle version du HTML :
1. Allez dans votre repo GitHub
2. Cliquez sur `index.html` → crayon (Edit)
3. Remplacez tout le contenu → **Commit**
4. GitHub Pages met à jour automatiquement en ~1 minute

## 📁 Fichiers

| Fichier | Description |
|---------|-------------|
| `index.html` | Le dashboard (à uploader sur GitHub) |
| `apps_script_v2.js` | Le code à coller dans Google Apps Script |
| `flux_template.xlsx` | Template pour l'onglet "Flux" (suivi des apports) |

## 🔒 Sécurité

- Le repo est public mais vos **données restent privées** : elles ne sont pas dans le repo, elles sont chargées dynamiquement depuis votre Google Apps Script
- L'URL de l'API est dans votre barre d'adresse uniquement, pas dans le code source du repo
- Personne ne peut accéder à vos données sans connaître l'URL exacte de votre Apps Script
