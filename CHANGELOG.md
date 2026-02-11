# Changelog

Toutes les modifications notables de ce projet seront documentées dans ce fichier.

Le format est basé sur [Keep a Changelog](https://keepachangelog.com/fr/1.0.0/),
et ce projet adhère au [Semantic Versioning](https://semver.org/lang/fr/).

## [2.0.0] - 2026-02-11

### ✨ Ajouté
- **Calcul automatique des dates de péremption** selon catégorie et emplacement
- **Recalcul en temps réel** lors du changement d'emplacement ou de catégorie
- **Table complète des durées de conservation** pour 9 catégories et 6 emplacements
- Fonction `calculerNouvelleDate()` pour le calcul intelligent des dates
- Fonction `afficherDuree()` pour afficher les durées en format lisible
- Event listeners automatiques sur les selects d'emplacement et catégorie

### 🎨 Modifié
- **Couleur du bouton "Tous"** changée en rouge/orange pour meilleure visibilité
- Design du bouton actif avec dégradé et ombre portée
- Message d'information sur la durée de conservation lors de l'ajout

### 🐛 Corrigé
- Correction de la clé localStorage de 'frigoProduits' vers 'frigo-items'
- Amélioration de la compatibilité avec les données existantes

### 📊 Durées de Conservation Implémentées

| Catégorie | Frigo | Congélateur | Placard | Cave |
|-----------|-------|-------------|---------|------|
| Fruits | 7j | 365j (1 an) | 3j | 14j |
| Légumes | 7j | 365j (1 an) | 5j | 30j (1 mois) |
| Viande | 3j | 180j (6 mois) | 1j | 2j |
| Poisson | 2j | 90j (3 mois) | 1j | 1j |
| Produits laitiers | 7j | 90j (3 mois) | 1j | 3j |
| Viennoiseries | 5j | 90j (3 mois) | 3j | 3j |
| Conserves | 180j (6 mois) | 730j (2 ans) | 730j (2 ans) | 1095j (3 ans) |
| Boissons | 90j (3 mois) | 180j (6 mois) | 365j (1 an) | 730j (2 ans) |
| Autre | 14j | 180j (6 mois) | 90j (3 mois) | 180j (6 mois) |

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
- Support de plus de langues
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

[2.0.0]: https://github.com/migapple/frigo-manager/compare/v1.0.0...v2.0.0
[1.0.0]: https://github.com/migapple/frigo-manager/releases/tag/v1.0.0
[Unreleased]: https://github.com/migapple/frigo-manager/compare/v2.0.0...HEAD
