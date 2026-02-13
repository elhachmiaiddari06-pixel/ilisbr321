# 💎 The Golden Pearl - Site Web E-Commerce

![The Golden Pearl](https://img.shields.io/badge/Status-Ready%20to%20Deploy-success)
![License](https://img.shields.io/badge/License-MIT-blue)

## 📋 Description

Site web e-commerce complet pour **The Golden Pearl** - boutique de sacs de luxe et clutches premium au Maroc.

**Caractéristiques :**
- ✅ Design luxueux et responsive
- ✅ Système de panier fonctionnel
- ✅ Checkout en 3 étapes
- ✅ 8 produits pré-configurés
- ✅ Optimisé SEO pour Google
- ✅ Multi-langues (Français)
- ✅ 100% gratuit et sans dépendances externes

---

## 🚀 Déploiement Rapide (5 minutes)

### Option 1 : GitHub Pages (Recommandé)

1. Créez un compte sur [github.com](https://github.com)
2. Créez un nouveau repository nommé `thegoldenpearl`
3. Téléchargez le fichier `index.html`
4. Allez dans Settings → Pages
5. Activez Pages avec la branch "main"
6. Votre site sera sur : `https://votreusername.github.io/thegoldenpearl/`

**Guide détaillé :** Voir `GUIDE-GITHUB-PAGES.md`

### Option 2 : Netlify

1. Allez sur [netlify.com](https://netlify.com)
2. Glissez-déposez le fichier `index.html`
3. Site en ligne instantanément !

### Option 3 : Vercel

1. Allez sur [vercel.com](https://vercel.com)
2. Importez le projet
3. Deploy !

---

## 📁 Structure du Projet

```
thegoldenpearl-website/
│
├── index.html                      # Site web principal (tout-en-un)
├── README.md                       # Ce fichier
├── GUIDE-GITHUB-PAGES.md          # Guide déploiement GitHub
├── GUIDE-REFERENCEMENT-GOOGLE.md  # Guide SEO complet
├── sitemap.xml                    # Sitemap pour Google
└── robots.txt                     # Fichier robots.txt
```

---

## ✨ Fonctionnalités

### 🛍️ E-Commerce
- Catalogue de 8 produits (sacs et clutches)
- Filtres par catégorie
- Système de panier avec localStorage
- Calcul automatique des totaux
- Gestion des stocks

### 💳 Checkout
- Formulaire en 3 étapes :
  1. Informations de livraison
  2. Méthode de paiement
  3. Confirmation de commande
- Validation des formulaires
- Page de confirmation
- 3 méthodes de paiement :
  - Carte bancaire
  - Cash à la livraison
  - Virement bancaire

### 🎨 Design
- Thème luxueux doré et violet
- Animations fluides
- Glass-morphism
- Totalement responsive
- Compatible tous navigateurs

### 🔍 SEO
- Meta tags optimisés
- Open Graph pour réseaux sociaux
- Données structurées JSON-LD
- Sitemap inclus
- Mots-clés ciblés Maroc

---

## 🛠️ Personnalisation

### Modifier les produits

Ouvrez `index.html` et trouvez la section `mockProducts` (ligne ~150) :

```javascript
const mockProducts = [
  {
    id: 1,
    title: "Votre Produit",
    description: "Description du produit",
    category: "Catégorie",
    image: "URL de l'image",
    rating: 4.9,
    reviews: 127,
    variants: [
      { 
        id: 101, 
        title: "Variante", 
        price_in_cents: 89900,  // Prix en centimes (899.00 MAD)
        sale_price_in_cents: 69900,  // Prix soldé
        currency_info: { symbol: "MAD ", code: "MAD" },
        manage_inventory: true,
        available_quantity: 8
      }
    ]
  },
  // Ajoutez plus de produits ici...
]
```

### Modifier les informations de contact

Cherchez et remplacez :
- Email : `elhachmiaiddari06@gmail.com`
- Téléphone : `+212 XXX-XXXXXX`
- Adresse : `Casablanca, Morocco`

### Changer les couleurs

Dans la section `<style>` (ligne ~13), modifiez :

```css
.text-gold {
  color: #d4af37;  /* Changez cette couleur */
}

.bg-gold {
  background-color: #d4af37;  /* Et celle-ci */
}
```

### Ajouter Google Analytics

Ajoutez ce code dans le `<head>` après les autres scripts :

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');  // Remplacez par votre ID
</script>
```

---

## 📊 Référencement Google

### Étapes essentielles :

1. **Google Search Console**
   - Soumettez votre URL
   - Uploadez `sitemap.xml`
   - Demandez l'indexation

2. **Google My Business**
   - Créez votre fiche entreprise
   - Ajoutez photos et informations
   - Demandez des avis clients

3. **Réseaux Sociaux**
   - Instagram : @thegoldenpearl.ma
   - Facebook Page
   - TikTok
   - Pinterest

**Guide complet :** Voir `GUIDE-REFERENCEMENT-GOOGLE.md`

---

## 🌐 Technologies Utilisées

- **React 18** - Framework JavaScript
- **Tailwind CSS** - Framework CSS
- **Font Awesome** - Icônes
- **Google Fonts** - Polices (Playfair Display, Poppins)
- Pur JavaScript (ES6+)
- HTML5
- CSS3

**Tous chargés via CDN - Aucune installation requise !**

---

## 📱 Compatibilité

✅ Chrome, Firefox, Safari, Edge  
✅ Mobile, Tablette, Desktop  
✅ iOS & Android  
✅ Tous les navigateurs modernes  

---

## 🔧 Dépannage

### Le site ne s'affiche pas

1. Vérifiez que le fichier s'appelle bien `index.html`
2. Videz le cache du navigateur (Ctrl + F5)
3. Vérifiez la console développeur (F12)
4. Assurez-vous d'avoir une connexion internet (pour les CDN)

### Les images ne chargent pas

Les images sont hébergées sur Unsplash via CDN. Assurez-vous d'avoir internet.

Pour utiliser vos propres images :
1. Hébergez-les sur [imgur.com](https://imgur.com) (gratuit)
2. Remplacez les URLs dans `mockProducts`

### Le panier ne sauvegarde pas

Le panier utilise `localStorage`. Vérifiez que :
1. Vous n'êtes pas en navigation privée
2. Le localStorage n'est pas désactivé
3. Le navigateur supporte localStorage

---

## 📞 Support

**Email :** elhachmiaiddari06@gmail.com  
**Site Web :** [À venir après déploiement]

---

## 📄 Licence

MIT License - Libre d'utilisation et de modification

---

## 🎯 Prochaines Étapes

### Immédiat (Aujourd'hui)
- [ ] Déployer sur GitHub Pages
- [ ] Créer Google My Business
- [ ] Soumettre à Google Search Console
- [ ] Créer compte Instagram
- [ ] Premier post sur Instagram

### Cette Semaine
- [ ] Publier sur Avito.ma
- [ ] Créer Facebook Page
- [ ] Créer TikTok
- [ ] 10 posts Instagram
- [ ] Demander premiers avis

### Ce Mois
- [ ] 100 followers Instagram
- [ ] 10 avis Google
- [ ] Première vente
- [ ] Optimiser SEO
- [ ] Collaborer avec influenceuse

---

## 🎨 Captures d'écran

### Page d'accueil
![Hero Section](https://via.placeholder.com/800x400?text=Hero+Section)

### Catalogue Produits
![Products](https://via.placeholder.com/800x400?text=Products+Grid)

### Panier
![Shopping Cart](https://via.placeholder.com/800x400?text=Shopping+Cart)

### Checkout
![Checkout](https://via.placeholder.com/800x400?text=Checkout+Page)

---

## 💡 Conseils Marketing

1. **Photos Professionnelles**
   - Investissez dans de bonnes photos de produits
   - Fond neutre et lumineux
   - Plusieurs angles

2. **Instagram Strategy**
   - Publiez quotidiennement
   - Utilisez Reels (très efficace)
   - Hashtags marocains
   - Stories interactives

3. **Avis Clients**
   - Demandez après chaque vente
   - Offrez 10% de réduction pour un avis
   - Partagez les meilleurs avis

4. **Influenceurs**
   - Contactez micro-influenceuses marocaines
   - Offrez un sac gratuit pour une story
   - ROI excellent au Maroc

---

## 🏆 Succès Rapide

**Suivez ce plan pendant 30 jours :**

- 📸 1-2 posts Instagram/jour
- 🎵 1-2 TikToks/jour  
- 📱 Stories quotidiennes
- 🔍 1 article de blog/semaine
- ⭐ Demandez 1 avis/jour
- 💬 Répondez aux messages en <1h

**Résultat attendu :** Première vente en 1-2 semaines ! 🎉

---

## 🙏 Remerciements

Merci d'utiliser The Golden Pearl Website Template !

Bonne chance avec votre boutique ! 🚀💎

---

**Version :** 1.0.0  
**Date :** Février 2026  
**Créé pour :** The Golden Pearl Maroc
