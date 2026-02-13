# 📁 ASSETS - Guide d'Organisation

## 🎯 Structure Recommandée

Si vous voulez ajouter vos propres images/fichiers :

```
thegoldenpearl-website/
│
├── index.html
├── README.md
├── sitemap.xml
├── robots.txt
│
└── assets/                    ← Créez ce dossier
    ├── images/
    │   ├── logo.png
    │   ├── products/
    │   │   ├── sac-1.jpg
    │   │   ├── sac-2.jpg
    │   │   └── ...
    │   └── banners/
    │       ├── hero.jpg
    │       └── about.jpg
    │
    ├── icons/
    │   ├── favicon.ico
    │   └── apple-touch-icon.png
    │
    └── documents/
        ├── conditions-vente.pdf
        └── politique-retour.pdf
```

---

## 📸 ACTUELLEMENT : Images par CDN

Votre site utilise actuellement des images hébergées sur **Unsplash CDN** (gratuit).

**Avantages :**
- ✅ Gratuit
- ✅ Rapide
- ✅ Aucun fichier à gérer
- ✅ Fonctionne partout

**Inconvénient :**
- ❌ Pas vos vrais produits

---

## 🖼️ AJOUTER VOS PROPRES IMAGES

### Option 1 : Imgur (Recommandé - GRATUIT)

1. Allez sur **imgur.com**
2. Créez un compte gratuit
3. Uploadez vos photos de sacs
4. Cliquez droit → "Copier l'adresse de l'image"
5. Remplacez les URLs dans `index.html`

**Exemple :**
```javascript
// Avant
image: "https://images.unsplash.com/photo-1566150905458..."

// Après
image: "https://i.imgur.com/VotreFichier.jpg"
```

### Option 2 : Cloudinary (GRATUIT)

1. Créez compte sur **cloudinary.com**
2. Uploadez vos images
3. Copiez les URLs
4. Remplacez dans le code

### Option 3 : GitHub Assets (si vous utilisez GitHub)

1. Dans votre repository GitHub
2. Créez un dossier `assets/images/`
3. Uploadez vos images
4. URL sera : `https://iliass123.github.io/thegoldenpearl/assets/images/votre-image.jpg`

---

## 🎨 LOGO & FAVICON

### Créer un Logo Gratuit

**Canva.com** (gratuit) :
1. Créez un compte
2. Cherchez "Logo"
3. Créez votre logo
4. Téléchargez en PNG transparent

### Créer un Favicon

**Favicon.io** (gratuit) :
1. Uploadez votre logo
2. Générez le favicon
3. Téléchargez le pack
4. Ajoutez dans `index.html` :

```html
<link rel="icon" type="image/png" sizes="32x32" href="assets/icons/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="assets/icons/favicon-16x16.png">
```

---

## 📄 DOCUMENTS PDF

### Conditions de Vente / Politique de Retour

1. Créez vos PDFs avec **Google Docs** ou **Canva**
2. Uploadez sur votre hébergement
3. Ajoutez les liens dans le footer

**Exemple :**
```html
<a href="assets/documents/conditions-vente.pdf" target="_blank">
  Conditions de Vente
</a>
```

---

## 🎥 VIDÉOS

### Option 1 : YouTube
1. Uploadez sur YouTube
2. Intégrez avec iframe

### Option 2 : Vimeo
Plus professionnel, sans pubs

---

## 📊 TAILLES D'IMAGES RECOMMANDÉES

### Photos de Produits
- **Format :** JPEG ou PNG
- **Taille :** 800x800 pixels (carré)
- **Poids :** < 200 KB
- **Qualité :** 85%

### Bannière Hero
- **Format :** JPEG
- **Taille :** 1920x1080 pixels
- **Poids :** < 500 KB

### Logo
- **Format :** PNG transparent
- **Taille :** 512x512 pixels
- **Poids :** < 50 KB

### Favicon
- **Format :** PNG ou ICO
- **Tailles :** 16x16, 32x32, 192x192

---

## 🔧 OPTIMISATION IMAGES

### Compresser vos images (GRATUIT)

**TinyPNG.com** :
1. Glissez-déposez vos images
2. Téléchargez versions compressées
3. Économisez 50-70% de poids !

**Squoosh.app** :
- Outil Google
- Compression avancée
- Avant/Après en temps réel

---

## 📝 CHECKLIST ASSETS

- [ ] Logo créé (PNG transparent)
- [ ] Favicon créé (16x16, 32x32)
- [ ] Photos de produits prises (800x800)
- [ ] Photos compressées (TinyPNG)
- [ ] Images uploadées (Imgur/Cloudinary)
- [ ] URLs remplacées dans index.html
- [ ] Conditions de vente PDF créé
- [ ] Politique de retour PDF créée
- [ ] Vidéo démo créée (optionnel)

---

## 💡 CONSEIL PRO

**Photos Professionnelles = Plus de Ventes**

Investissez du temps dans de belles photos :
- Fond neutre (blanc/gris)
- Lumière naturelle
- Plusieurs angles
- Photos lifestyle (sac porté)
- Détails (coutures, fermeture)

**Budget 0 MAD :**
- Utilisez votre smartphone
- Photographiez près d'une fenêtre
- Drap blanc comme fond
- Éditez avec Snapseed (gratuit)

---

## 🎯 PROCHAINES ÉTAPES

1. Prenez de belles photos de vos sacs
2. Uploadez sur Imgur
3. Remplacez les URLs dans le code
4. Créez votre logo sur Canva
5. Ajoutez votre favicon

**Temps nécessaire :** 2-3 heures

**Résultat :** Site 100% personnalisé ! ✨

---

**Note :** Pour l'instant, vous pouvez lancer le site avec les images actuelles et les remplacer progressivement.
