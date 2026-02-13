# Changelog

Toutes les modifications notables de ce projet seront documentées dans ce fichier.

Le format est basé sur [Keep a Changelog](https://keepachangelog.com/fr/1.0.0/),
et ce projet adhère au [Semantic Versioning](https://semver.org/lang/fr/).

## [2.1.5] - 2026-02-13

### 🐛 Corrigé
- **Recalcul automatique de la date de péremption** lors du changement de catégorie ou d'emplacement
- Les event listeners sont maintenant correctement attachés aux selects

### ✨ Ajouté
- La date se recalcule automatiquement en temps réel lors du changement de catégorie
- La date se recalcule automatiquement en temps réel lors du changement d'emplacement
- Fonctionne dans le formulaire d'ajout ET de modification

## [2.1.4] - 2026-02-13

### ✨ Ajouté
- **Table des durées de conservation** accessible via ⚙️ Paramètres → 📋 Table des durées
- Visualisation complète des 54 combinaisons (9 catégories × 6 emplacements)
- Codes couleur pour identifier rapidement les durées (rouge=court, bleu=congélateur, vert=long)
- Conseils et astuces de conservation alimentaire
- Avertissements de sécurité alimentaire

### 📱 Amélioré
- Interface responsive pour les tableaux (scroll horizontal sur mobile)
- Modal avec hauteur maximale adaptative (90vh)

## [2.1.3] - 2026-02-13

### 🐛 Corrigé
- **Filtres "Frais", "Urgent" et "Périmés"** excluent maintenant les produits à quantité 0
- Les produits épuisés n'apparaissent plus que dans le filtre "Épuisé"

### ✅ Amélioré
- Logique de filtrage plus cohérente et intuitive
- Élimination des doublons entre filtres
- Compteurs de produits plus précis

## [2.1.2] - 2026-02-13

### 🐛 Corrigé
- **Bouton "Saisie manuelle"** ne fonctionnait plus
- Ordre des variables dans la fonction `showForm()`
- Variable `suggestedDateStr` non définie
- Variable `defaultEmplacement` utilisée avant sa déclaration

### 🔧 Amélioré
- Initialisation sécurisée des boutons avec vérification null
- Meilleure gestion des erreurs JavaScript

## [2.1.1] - 2026-02-13

### 🎨 Modifié
- **Alignement des boutons langue/paramètres** sur iPhone pour meilleure ergonomie
- Boutons repositionnés au niveau du sous-titre "Scanner de code-barres"
- Position adaptée pour mobile (top: 55px au lieu de 10px)

### 📱 Amélioré
- Ergonomie mobile optimisée
- Meilleurs touch targets sur petit écran

## [2.1.0] - 2026-02-13

### ✨ Ajouté
- **Modification des recettes par défaut** (crée une copie personnalisée)
- Message de confirmation lors de la modification d'une recette par défaut
- Titre du formulaire adapté : "📋 Copie de la recette"
- **Export Excel inclut les scores santé** (Nutri-Score, NOVA, Additifs, Eco-Score)
- Import Excel avec lecture des scores santé
- 4 colonnes supplémentaires dans le fichier Excel (12 colonnes au total)
- **Système de versioning automatique** avec changelog intégré
- Variable `APP_VERSION` et `VERSION_DATE` globales
- Objet `CHANGELOG` multilingue (FR/EN)
- **Bouton "Quoi de neuf ?"** dans les paramètres
- Modal affichant l'historique complet des versions
- Fonction `showChangelog()` et `closeChangelog()`

### 🎨 Modifié
- **Couleur du bouton "Tous"** changée en rouge/orange pour meilleure visibilité
- Dégradé : `linear-gradient(135deg, #ef4444 0%, #dc2626 100%)`
- Ombre portée et effet 3D sur le bouton actif

## [2.0.0] - 2026-02-11

### ✨ Ajouté
- **Calcul automatique des dates de péremption** selon catégorie et emplacement
- **Recalcul en temps réel** lors du changement d'emplacement ou de catégorie (via event listeners)
- **Table complète des durées de conservation** pour 54 combinaisons
- Fonction `calculerNouvelleDate(categorie, emplacement)` pour le calcul intelligent
- Fonction `afficherDuree(jours)` pour afficher les durées en format lisible
- Event listeners automatiques sur les selects d'emplacement et catégorie
- Indication visuelle de la durée suggérée dans le formulaire

### 🔧 Modifié
- Clé localStorage changée de `'frigoProduits'` vers `'frigo-items'`
- Migration automatique des données existantes

### 📊 Durées de Conservation Implémentées

| Catégorie | Frigo | Congélateur | Placard | Cave | Corbeille | Autre |
|-----------|-------|-------------|---------|------|-----------|-------|
| **🍎 Fruits** | 7j | 365j (1 an) | 3j | 14j | 5j | 7j |
| **🥕 Légumes** | 7j | 365j (1 an) | 5j | 30j (1 mois) | 5j | 7j |
| **🥩 Viande** | 3j | 180j (6 mois) | 1j | 2j | 1j | 2j |
| **🐟 Poisson** | 2j | 90j (3 mois) | 1j | 1j | 1j | 1j |
| **🥛 Produits laitiers** | 7j | 90j (3 mois) | 1j | 3j | 3j | 5j |
| **🥐 Viennoiseries** | 5j | 90j (3 mois) | 3j | 3j | 3j | 3j |
| **🥫 Conserves** | 180j (6 mois) | 730j (2 ans) | 730j (2 ans) | 1095j (3 ans) | 365j (1 an) | 365j (1 an) |
| **🥤 Boissons** | 90j (3 mois) | 180j (6 mois) | 365j (1 an) | 730j (2 ans) | 180j (6 mois) | 365j (1 an) |
| **📦 Autre** | 14j | 180j (6 mois) | 90j (3 mois) | 180j (6 mois) | 14j | 30j (1 mois) |

## [1.0.0] - 2025-XX-XX

### ✨ Ajouté
- Scanner de code-barres avec QuaggaJS
- Intégration API Open Food Facts
- Gestion des produits (ajout, modification, suppression)
- Scores santé (Nutri-Score, NOVA, Eco-Score, Additifs)
- Gestion des photos (capture, stockage base64)
- Système de catégories (9 catégories)
- Système d'emplacements (6 emplacements)
- Gestion des quantités avec boutons +/-
- Système "à renouveler" pour liste de courses
- Alertes de péremption (frais, urgent, périmé, épuisé)
- Filtres multiples (statut + emplacement)
- Export/Import Excel (SheetJS)
- Recherche avec historique
- Suggestions de recettes basées sur produits disponibles
- Notifications push
- Badge de notification sur icône app
- Support multilingue FR/EN
- Mode PWA (Progressive Web App)
- Stockage local (localStorage)
- Interface responsive (mobile-first)

### 🎨 Modifié
- Design avec dégradé violet (#667eea → #764ba2)
- Interface optimisée pour mobile
- Animations et transitions fluides

### 📱 Compatibilité
- ✅ Chrome/Edge (Desktop & Mobile)
- ✅ Firefox (Desktop & Mobile)
- ✅ Safari (Desktop & Mobile)
- ✅ iOS WebApp
- ✅ Android WebApp

## [Unreleased]

### 🚀 À venir
- Mode sombre
- Synchronisation cloud (optionnelle)
- Widget iOS/Android
- Support de plus de langues (ES, DE, IT)
- Statistiques de consommation
- Prédictions de consommation avec IA
- Partage de liste de courses
- Intégration avec applications de livraison

---

## Types de changements

- `✨ Ajouté` : nouvelles fonctionnalités
- `🎨 Modifié` : changements dans les fonctionnalités existantes
- `🐛 Corrigé` : corrections de bugs
- `🗑️ Supprimé` : fonctionnalités supprimées
- `🔒 Sécurité` : corrections de vulnérabilités
- `📚 Documentation` : changements dans la documentation
- `⚡ Performance` : améliorations de performance
- `♻️ Refactoring` : restructuration du code

---

[2.1.5]: https://github.com/migapple/frigo-manager/compare/v2.1.4...v2.1.5
[2.1.4]: https://github.com/migapple/frigo-manager/compare/v2.1.3...v2.1.4
[2.1.3]: https://github.com/migapple/frigo-manager/compare/v2.1.2...v2.1.3
[2.1.2]: https://github.com/migapple/frigo-manager/compare/v2.1.1...v2.1.2
[2.1.1]: https://github.com/migapple/frigo-manager/compare/v2.1.0...v2.1.1
[2.1.0]: https://github.com/migapple/frigo-manager/compare/v2.0.0...v2.1.0
[2.0.0]: https://github.com/migapple/frigo-manager/compare/v1.0.0...v2.0.0
[1.0.0]: https://github.com/migapple/frigo-manager/releases/tag/v1.0.0
[Unreleased]: https://github.com/migapple/frigo-manager/compare/v2.1.5...HEAD
