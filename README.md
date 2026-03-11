# 🧊 Frigo Manager v2.2.0

<div align="center">

![Version](https://img.shields.io/badge/version-2.2.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Language](https://img.shields.io/badge/language-JavaScript-yellow.svg)

**Scanner de code-barres intelligent pour gérer votre frigo** 🚀

[Démo](#demo) | [Fonctionnalités](#fonctionnalités) | [Installation](#installation) | [English](#english)

</div>

---

## ✨ Nouveautés v2.20
- 🐛 Correction de la hauteur du notch
- 🐛 Correction du scroll bloqué sous le notch'
  
## ✨ Nouveautés v2.18
- ✅ Optimisé pour la majorité des utilisateurs (mobile)

### 🛒 Liste de Courses
- Saisie numérique dans les nouvelles recettes

### 📊 Export/Import
- ✅ Sauvegardes dans le dossier Frigo-Manager

### 🔄 Recalcul Automatique en Temps Réel
La version 2.1 améliore le calcul des dates avec un **recalcul automatique instantané** :
- Changez la catégorie → La date se recalcule ✨
- Changez l'emplacement → La date se recalcule ✨
- Fonctionne dans l'ajout ET la modification de produits

### 📋 Table des Durées Intégrée
Consultez facilement toutes les durées de conservation :
- Accessible via ⚙️ Paramètres → 📋 Table des durées
- 54 combinaisons affichées (9 catégories × 6 emplacements)
- Codes couleur pour identification rapide
- Conseils de conservation inclus

### 🎯 Calcul Automatique des Dates de Péremption

Le système intelligent calcule automatiquement les dates selon :
- 📍 **L'emplacement** (frigo, congélateur, placard, cave)
- 🏷️ **La catégorie** (viande, poisson, fruits, légumes, etc.)

**Exemple :**
- 🥩 Poulet au frigo → **3 jours**
- 🥩 Poulet au congélateur → **6 mois** ❄️
- 🍎 Pommes au frigo → **7 jours**  
- 🍎 Pommes au congélateur → **1 an** ❄️

Le système **recalcule automatiquement** la date quand vous changez l'emplacement !

---

## 📊 Tableau des Durées de Conservation

| Catégorie | 🧊 Frigo | ❄️ Congélo | 🚪 Placard | 🍷 Cave |
|-----------|----------|------------|------------|---------|
| 🍎 Fruits | 7 jours | **1 an** | 3 jours | 14 jours |
| 🥕 Légumes | 7 jours | **1 an** | 5 jours | 1 mois |
| 🥩 Viande | 3 jours | **6 mois** | 1 jour | 2 jours |
| 🐟 Poisson | 2 jours | **3 mois** | 1 jour | 1 jour |
| 🥛 Produits laitiers | 7 jours | **3 mois** | 1 jour | 3 jours |
| 🥐 Viennoiseries | 5 jours | **3 mois** | 3 jours | 3 jours |
| 🥫 Conserves | 6 mois | **2 ans** | **2 ans** | **3 ans** |
| 🥤 Boissons | 3 mois | 6 mois | **1 an** | **2 ans** |

---

## 🚀 Fonctionnalités

### 📱 Scanner Intelligent
- ✅ Scan de code-barres via caméra
- ✅ Détection automatique des produits (API Open Food Facts)
- ✅ Récupération automatique des infos produit
- ✅ Support multi-format (EAN-13, UPC, etc.)

### ⏰ Gestion des Dates
- ✅ **Calcul automatique** selon catégorie + emplacement
- ✅ **Recalcul en temps réel** lors du changement d'emplacement
- ✅ Alertes de péremption (urgent, périmé)
- ✅ Notifications push
- ✅ Badge de notification sur l'icône

### 🏥 Scores Santé
- ✅ **Nutri-Score** (A à E)
- ✅ **NOVA** (transformation industrielle)
- ✅ **Eco-Score** (impact environnemental)
- ✅ **Additifs** (dangereux, à risque, acceptables)

### 📸 Gestion des Photos
- ✅ Prise de photo personnalisée
- ✅ Photo automatique via code-barres
- ✅ Suppression/remplacement facile

### 🗂️ Organisation
- ✅ Catégories : Fruits, Légumes, Viande, Poisson, etc.
- ✅ Emplacements : Frigo, Congélateur, Placard, Cave, Corbeille
- ✅ Filtres multiples (frais, urgent, périmé, épuisé)
- ✅ Gestion des quantités (+/-)
- ✅ Liste "à renouveler"

### 🛒 Liste de Courses
- ✅ Génération automatique depuis les produits épuisés
- ✅ Ajout des produits "à renouveler"
- ✅ Export/partage facile

### 👨‍🍳 Suggestions de Recettes
- ✅ Basées sur vos produits disponibles
- ✅ Priorise les produits proches de la péremption
- ✅ Suggestions personnalisées
- ✅ Ajout de vos propres recettes

### 📊 Export/Import
- ✅ Export Excel (.xlsx)
- ✅ Import Excel pour restauration
- ✅ Sauvegarde/restauration complète

### 🌍 Multilingue
- ✅ Français 🇫🇷
- ✅ Anglais 🇬🇧
- ✅ Changement instantané

### 🔍 Recherche
- ✅ Recherche instantanée
- ✅ Historique des recherches
- ✅ Filtres combinés

---

## 💻 Installation

### Option 1 : Utilisation Directe (Recommandé)

1. **Téléchargez** le fichier `index.html`
2. **Ouvrez-le** dans votre navigateur web
3. **C'est tout !** 🎉

Vos données sont stockées localement dans votre navigateur (localStorage).

### Option 2 : GitHub Pages

1. **Forkez** ce repo
2. Allez dans **Settings** → **Pages**
3. Activez GitHub Pages sur la branche `main`
4. Accédez à : `https://votre-username.github.io/frigo-manager/`

### Option 3 : Installation sur Mobile (PWA)

**Sur iOS (Safari) :**
1. Ouvrez `index.html` dans Safari
2. Tapez sur l'icône **Partager** 
3. Sélectionnez **"Sur l'écran d'accueil"**
4. L'app apparaît comme une vraie application ! 📱

**Sur Android (Chrome) :**
1. Ouvrez `index.html` dans Chrome
2. Menu → **"Ajouter à l'écran d'accueil"**
3. L'app est installée ! 📱

---

## 🎨 Technologies

- **HTML5** - Structure
- **CSS3** - Design responsive
- **JavaScript (Vanilla)** - Logique
- **QuaggaJS** - Scanner de code-barres
- **SheetJS** - Export/Import Excel
- **Open Food Facts API** - Données produits
- **LocalStorage** - Stockage local

**Aucune dépendance serveur - 100% client-side !**

---

## 📖 Guide d'utilisation

### Ajouter un produit

1. **Scanner** : Cliquez sur 📷 et scannez le code-barres
2. **Manuel** : Cliquez sur ➕ et remplissez le formulaire
3. Le système calcule **automatiquement** la date selon la catégorie et l'emplacement

### Modifier un produit

1. Cliquez sur un produit
2. Modifiez les informations
3. La date se **recalcule automatiquement** si vous changez la catégorie ou l'emplacement

### Voir les alertes

- **🟢 Vert** : Produit frais (>3 jours)
- **🟠 Orange** : Urgent (0-3 jours)
- **🔴 Rouge** : Périmé (date dépassée)

### Export des données

1. Cliquez sur ⚙️ (Paramètres)
2. **Export Excel** → télécharge vos données
3. **Import Excel** → restaure vos données

---

## 🔧 Personnalisation

### Modifier les durées de conservation

Ouvrez `index.html` et cherchez :

```javascript
var dureeConservation = {
    'viande': {
        'frigo': 3,        // Changez ces valeurs
        'congelateur': 180, // en jours
        // ...
    }
}
```

### Changer les couleurs

Cherchez ces sections dans le CSS :

```css
/* Couleur principale */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Bouton actif */
.filter-btn.active {
    background: linear-gradient(135deg, #ff6b6b 0%, #ee5a6f 100%);
}
```

---

## 🐛 Dépannage

### Le scanner ne fonctionne pas
- Autorisez l'accès à la caméra dans les paramètres du navigateur
- Utilisez HTTPS ou localhost
- Vérifiez que votre appareil a une caméra

### Les données ont disparu
- Les données sont dans le localStorage du navigateur
- Ne pas vider le cache sans exporter d'abord
- Faites des exports réguliers en Excel

### Les notifications ne s'affichent pas
- Autorisez les notifications dans les paramètres du navigateur
- Vérifiez que le site n'est pas en mode silencieux

---

## 📝 Changelog

### v2.0.0 (2026-02-11)
- ✨ **NOUVEAU** : Calcul automatique des dates de péremption
- ✨ **NOUVEAU** : Recalcul en temps réel lors du changement d'emplacement
- ✨ **NOUVEAU** : Table complète des durées de conservation
- 🎨 Amélioration de la couleur du bouton "Tous" (meilleure visibilité)
- 🐛 Correction de la clé localStorage ('frigo-items')

### v1.0.0
- 🎉 Version initiale
- Scanner de code-barres
- Gestion des produits
- Scores santé
- Export Excel

---

## 🤝 Contribution

Les contributions sont les bienvenues ! 

1. **Fork** le projet
2. Créez une **branche** (`git checkout -b feature/AmazingFeature`)
3. **Commit** vos changements (`git commit -m 'Add AmazingFeature'`)
4. **Push** (`git push origin feature/AmazingFeature`)
5. Ouvrez une **Pull Request**

---

## 📄 License

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

## 👨‍💻 Auteur

**Michel Garlandat** - [migapple](https://github.com/migapple)

Développé avec l'aide d'Anthropic Claude

---

## 🙏 Remerciements

- [Open Food Facts](https://world.openfoodfacts.org/) - Base de données alimentaire
- [QuaggaJS](https://github.com/ericblade/quagga2) - Scanner de code-barres
- [SheetJS](https://sheetjs.com/) - Export/Import Excel
- [Anthropic Claude](https://www.anthropic.com/) - Assistance au développement

---

## 📞 Support

Des questions ? Des suggestions ?

- 🐛 **Issues** : [GitHub Issues](https://github.com/migapple/frigo-manager/issues)
- 💬 **Discussions** : [GitHub Discussions](https://github.com/migapple/frigo-manager/discussions)

---

<div align="center">

**⭐ Si ce projet vous aide, donnez-lui une étoile sur GitHub ! ⭐**

Made with ❤️ in France 🇫🇷

</div>

---

# English

## 🧊 Frigo Manager v2

**Smart barcode scanner to manage your fridge** 🚀

### ✨ New in v2.0

**Automatic Expiration Date Calculation**

Version 2 introduces an intelligent system that automatically calculates expiration dates based on location and category.

### 🚀 Key Features

- 📱 Smart barcode scanner
- ⏰ Automatic expiration date calculation
- 🏥 Health scores (Nutri-Score, NOVA, Eco-Score)
- 📸 Photo management
- 🛒 Shopping list generation
- 📊 Excel export/import
- 🌍 Multilingual (FR/EN)

### 💻 Installation

1. Download `index.html`
2. Open in your browser
3. Done! 🎉

### 📄 License

MIT License

### 👨‍💻 Author

**Michel Garlandat** - [migapple](https://github.com/migapple)

---

<div align="center">

**⭐ Star this project on GitHub! ⭐**

</div>
