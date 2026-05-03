# Bella Hair - Système de Gestion de Salon de Coiffure

## 📋 Vue d'ensemble

Bella Hair est une solution complète composée de deux applications distinctes mais interconnectées :

1. **Backoffice** : Application de gestion interne pour l'administration du salon (Laravel + React/Inertia.js)
2. **Site Client** : Site web public Next.js pour les clients (Next.js 16 + React 19)

Cette architecture permet une séparation claire des responsabilités tout en assurant une synchronisation des données via une API RESTful.

---

# 🏢 PARTIE BACKOFFICE

## 📋 Description

Le backoffice est l'application de gestion interne utilisée par le personnel du salon (administrateurs, gérants, coiffeurs, caissiers, agents). Il permet de gérer tous les aspects opérationnels et administratifs du salon.

---

## 🛠️ Stack Technique Backoffice

### Backend
- **Laravel 12** : Framework PHP robuste
- **MySQL/SQLite** : Base de données
- **Sanctum** : Authentification API
- **Socialite** : Authentification sociale (Google)
- **Media Library** : Gestion des fichiers médias
- **DomPDF** : Génération de PDF
- **Excel** : Export Excel (Maatwebsite)
- **Twilio** : Envoi de SMS
- **ZKTeco** : Intégration pointage biométrique
- **QR Code** : Génération de codes QR (Simple-QRCode)

### Frontend
- **React 18** : Bibliothèque JavaScript
- **Inertia.js** : Bridge Laravel-React sans API
- **TypeScript** : Typage statique
- **Tailwind CSS 4** : Framework CSS utilitaire
- **Radix UI** : Composants UI accessibles
- **Recharts** : Graphiques et visualisations
- **React Hook Form** : Gestion des formulaires
- **Zod** : Validation de schémas
- **Tremor React** : Composants de dashboard
- **Sonner** : Notifications toast

### Outils de Développement
- **Vite** : Build tool ultra-rapide
- **ESLint** : Linting JavaScript
- **Prettier** : Formatage de code
- **PHPUnit** : Tests unitaires

---

## 🎯 Fonctionnalités Backoffice

### 1. Gestion des Rendez-vous

- **Calendrier interactif** pour visualiser et gérer les créneaux
- **Gestion des statuts** : en attente, confirmé, annulé, terminé
- **Rendez-vous à domicile** avec gestion des frais de déplacement
- **Notifications SMS** automatiques pour rappels et confirmations
- **Paiement échelonné** : acomptes et soldes
- **Historique complet** des rendez-vous par client
- **Confirmation et annulation** par le personnel
- **Messagerie client** intégrée

### 2. Gestion des Clients (CRM)

- **Profils clients complets** : informations personnelles, préférences
- **Historique d'achat** et de visites
- **Système de favoris** pour services et produits
- **Avatars personnalisables**
- **Verification email** et sécurité des comptes
- **Réinitialisation de mot de passe** par SMS/email
- **Création rapide** de clients lors des ventes
- **Statistiques client** : fréquence, montant total, etc.

### 3. Catalogue de Services

- **Services de coiffure** : coupe, coloration, brushing, etc.
- **Catégorisation** des services par type
- **Gestion des prix** et durées
- **Promotions** et prix promotionnels
- **Visibilité contrôlée** (actif/inactif, visible/caché)
- **Images et descriptions** détaillées
- **Statistiques** sur les services les plus demandés
- **Gestion des images** multiples par service

### 4. Gestion des Produits

- **Catalogue de produits** : shampoings, laques, accessoires, etc.
- **Gestion des stocks** en temps réel
- **Alertes de rupture** de stock
- **Catégorisation** des produits
- **Prix d'achat et de vente**
- **Promotions** et soldes
- **Gestion des images** multiples
- **Transfert de stocks** entre succursales
- **Stock global** par produit

### 5. Point de Vente (POS)

- **Vente de produits et services**
- **Facturation automatique** avec codes uniques
- **Modes de paiement** multiples
- **Gestion des remises**
- **Acomptes** et paiements partiels
- **Impression de reçus**
- **Historique des ventes**
- **Statistiques journalières** de ventes
- **Gestion des promotions** en caisse

### 6. Gestion du Personnel (RH)

- **Fiches agents** complètes (informations personnelles, CNSS, etc.)
- **Matricules automatiques**
- **Photos et signatures** numériques
- **Gestion des contrats** de travail
- **Références professionnelles**
- **Assignation aux succursales**
- **Rôles et permissions** : admin, gérant, coiffeur, caissier, agent, community manager
- **Dashboard personnel** pour les agents

### 7. Gestion des Présences

- **Pointage biométrique** (intégration ZKTeco)
- **Pointage manuel** avec notes
- **Suivi des heures** de travail
- **Gestion des pauses**
- **Rapports de présence** quotidiens/mensuels
- **Grilles de pointage** imprimables
- **Historique complet** des présences
- **Génération automatique** des pointages

### 8. Gestion des Congés

- **Demandes de congés** (annuel, maladie, etc.)
- **Workflow d'approbation** par les gestionnaires
- **Suivi des soldes** de congés
- **Statistiques** sur les congés
- **Impression des attestations**
- **Historique** des demandes
- **Types de congés** personnalisables

### 9. Gestion de la Paie

- **Calcul automatique** des salaires
- **Gestion des acomptes** sur salaire
- **Fiches de paie** détaillées
- **Rapports de paie** (PDF, Excel)
- **Historique des paiements**
- **Intégration avec les pointages**
- **Rapports consolidés** de paie

### 10. Programme de Fidélité

- **Système de points** cumulables
- **Cadeaux d'anniversaire** automatiques
- **Configuration flexible** des règles de fidélité
- **Suivi des achats** et montants
- **Niveaux de fidélité**
- **Récompenses personnalisables
- **Statistiques de fidélisation**

### 11. Gestion Multi-Succursales

- **Création de plusieurs succursales**
- **Gestion des stocks** par succursale
- **Transferts de stocks** entre succursales
- **Personnel assigné** par succursale
- **Rapports consolidés** ou par succursale
- **Permissions basées** sur la succursale
- **Validation des transferts**

### 12. Gestion Financière

- **Suivi des dépenses** par catégorie
- **Budgets prévisionnels**
- **Catégories de dépenses** personnalisables
- **Sorties de fonds** avec validation
- **Rapports financiers**
- **Gestion multi-devises** avec taux de change
- **Caisse et encaissements**
- **Acomptes clients**

### 13. Rapports et Statistiques

- **Tableau de bord** avec KPIs en temps réel
- **Statistiques de ventes** (journalières, mensuelles)
- **Analyse des produits** et services les plus vendus
- **Performance des vendeurs**
- **Rapports PDF** exportables
- **Graphiques et visualisations**
- **Filtres par période** et succursale
- **Rapports de synthèse**

### 14. Marketing et Communication

- **Galerie photos** des réalisations
- **Témoignages clients** avec modération
- **Promotions** et offres spéciales
- **Notifications SMS** (Twilio)
- **Alertes internes** pour le personnel
- **Publication de contenu** (community manager)

### 15. Sécurité et Audit

- **Authentification sécurisée** (Sanctum)
- **Rôles et permissions** granulaires
- **Journal d'audit** complet des actions
- **Logs utilisateur** traçables
- **Protection CSRF**
- **Validation des données**
- **Gestion des devices** autorisés

---

## 🔐 Rôles et Permissions Backoffice

- **Admin** : Accès total à toutes les fonctionnalités
- **Gérant** : Gestion de la succursale, rapports, personnel
- **Coiffeur** : Rendez-vous, ventes, pointage
- **Caissier** : Ventes, encaissements, stocks
- **Agent** : Pointage, congés, acomptes, dashboard personnel
- **Community Manager** : Galerie, témoignages, promotions

---

## 📱 Modules Backoffice

1. **Dashboard** : Vue d'ensemble avec statistiques
2. **Rendez-vous** : Gestion complète des appointments
3. **Clients** : CRM et gestion de la clientèle
4. **Services** : Catalogue des prestations
5. **Produits** : Gestion du catalogue et stocks
6. **Ventes** : Point de vente et facturation
7. **Personnel** : Gestion RH et employés
8. **Pointages** : Suivi des présences
9. **Congés** : Gestion des absences
10. **Paie** : Gestion salariale
11. **Stocks** : Gestion des inventaires
12. **Succursales** : Multi-sites
13. **Dépenses** : Comptabilité et budgets
14. **Rapports** : Analytics et export
15. **Fidélité** : Programme de récompenses
16. **Galerie** : Portfolio et médias
17. **Témoignages** : Avis clients
18. **Configuration** : Paramètres système
19. **Audit** : Journal des actions
20. **Alertes** : Notifications internes

---

# 🌐 PARTIE SITE CLIENT

## 📋 Description

Le site client est une application Next.js moderne et responsive qui permet aux clients de :
- Découvrir les services et produits du salon
- Prendre rendez-vous en ligne
- Créer un compte personnel
- Gérer leurs rendez-vous et favoris
- Voir la galerie et laisser des témoignages

Le site communique avec le backoffice via une API RESTful.

---

## 🛠️ Stack Technique Site Client

### Frontend
- **Next.js 16** : Framework React avec App Router
- **React 19** : Bibliothèque JavaScript
- **TypeScript** : Typage statique
- **Tailwind CSS 4** : Framework CSS utilitaire
- **Radix UI** : Composants UI accessibles
- **Shadcn UI** : Composants pré-construits
- **Framer Motion** : Animations fluides
- **Lucide React** : Icônes
- **next-themes** : Gestion du thème (sombre/clair)
- **Base UI** : Composants UI supplémentaires

### Outils de Développement
- **ESLint** : Linting JavaScript
- **PostCSS** : Traitement CSS
- **TypeScript** : Compilation

---

## 🎯 Fonctionnalités Site Client

### 1. Page d'Accueil

- **Hero section** animée avec appel à l'action
- **Présentation des services** populaires
- **Slider des produits** disponibles
- **Témoignages clients** en carousel
- **Galerie photos** des réalisations
- **Design moderne** et responsive
- **Animations fluides** (Framer Motion)

### 2. Authentification

- **Inscription** avec email et mot de passe
- **Connexion** email/mot de passe
- **Authentification Google** (OAuth)
- **Réinitialisation de mot de passe** par email
- **Vérification d'email** avec code
- **Session sécurisée** via API token

### 3. Catalogue de Services

- **Liste complète** des services disponibles
- **Filtrage par catégorie**
- **Détails de chaque service** : description, prix, durée
- **Images des services**
- **Bouton de réservation** directe
- **Pages SEO optimisées** pour chaque service

### 4. Catalogue de Produits

- **Grille de produits** avec images
- **Filtrage par catégorie**
- **Détails produits** : description, prix
- **Gestion des favoris** (pour clients connectés)
- **Pages SEO optimisées** pour chaque produit

### 5. Prise de Rendez-vous

- **Formulaire de réservation** en ligne
- **Sélection du service**
- **Choix de la date et heure**
- **Sélection de la succursale**
- **Options de rendez-vous** : salon ou domicile
- **Calcul automatique** des frais de déplacement
- **Confirmation immédiate** ou en attente

### 6. Espace Client (Dashboard)

- **Profil personnalisé** avec avatar
- **Statistiques** : RDV à venir, commandes, favoris, points fidélité
- **Gestion de l'avatar** (upload/suppression)
- **Informations personnelles** modifiables
- **Liste des favoris** (services et produits)
- **Navigation intuitive** entre les sections

### 7. Gestion des Rendez-vous

- **Liste des rendez-vous** avec pagination
- **Détails de chaque RDV** : date, heure, service, montant
- **Statuts visuels** : confirmé, en attente, annulé
- **Informations sur la succursale**
- **Gestion du paiement** (acompte/solde)
- **Historique complet** des rendez-vous

### 8. Galerie Photos

- **Portfolio visuel** des réalisations
- **Slider automatique** des photos
- **Catégorisation par type** de service
- **Design immersif**
- **Optimisation des images**

### 9. Témoignages

- **Liste des témoignages** clients
- **Possibilité de laisser** un avis (clients connectés)
- **Modération** par le backoffice
- **Affichage des notes**
- **Design attrayant**

### 10. Pages SEO

- **Page "À propos"** : présentation du salon
- **Pages spécialisées** : coiffure mariage, maquillage professionnel
- **Optimisation SEO** : meta tags, sitemap, robots.txt
- **Breadcrumbs** pour la navigation
- **FAQ sections** pour le référencement

### 11. Expérience Utilisateur

- **Design responsive** : mobile, tablette, desktop
- **Mode sombre/clair** avec persistance
- **Animations fluides** et transitions
- **Chargement rapide** (Next.js optimization)
- **Navigation intuitive**
- **Feedback utilisateur** (toasts, loaders)
- **PWA ready** : installation possible sur mobile

### 12. Intégration API

- **Communication RESTful** avec le backoffice
- **Authentification via token**
- **Gestion des erreurs** graceful
- **Loading states** optimisés
- **Cache intelligent** des données

---

## 📱 Pages du Site Client

1. **Accueil** : Hero, services, produits, témoignages, galerie
2. **Services** : Catalogue complet des services
3. **Détail Service** : Page individuelle de service
4. **Produits** : Catalogue des produits
5. **Détail Produit** : Page individuelle de produit
6. **Galerie** : Portfolio des réalisations
7. **Témoignages** : Avis clients
8. **Connexion** : Formulaire de connexion
9. **Inscription** : Formulaire d'inscription
10. **Mot de passe oublié** : Récupération
11. **Réinitialisation** : Nouveau mot de passe
12. **Vérification email** : Validation compte
13. **Dashboard Client** : Espace personnel
14. **Mes Rendez-vous** : Liste des RDV
15. **Détail RDV** : Détails d'un rendez-vous
16. **Nouveau RDV** : Formulaire de réservation
17. **Détail RDV Public** : Vue publique d'un RDV
18. **À propos** : Présentation du salon
19. **Coiffure Mariage** : Page spécialisée
20. **Maquillage Pro** : Page spécialisée

---

# 🔗 INTÉGRATION BACKOFFICE - SITE CLIENT

## Communication API

Le site client communique avec le backoffice via une API RESTful sécurisée :

- **Authentification** : Tokens Sanctum
- **Endpoints publics** : Services, produits, galerie, témoignages
- **Endpoints protégés** : Rendez-vous, profil client, favoris
- **Synchronisation en temps réel** des données
- **Gestion des erreurs** centralisée

## Flux de Données

1. **Client s'inscrit** sur le site → Données stockées dans le backoffice
2. **Client prend RDV** → Création dans le backoffice, confirmation par email/SMS
3. **Personnel valide RDV** → Statut mis à jour, notification client
4. **Client laisse témoignage** → Modération via backoffice
5. **Promotions créées** → Affichage automatique sur le site client

---

# 🚀 Avantages de l'Architecture

## Séparation des Responsabilités

- **Backoffice** : Focus sur la gestion interne et l'administration
- **Site Client** : Focus sur l'expérience utilisateur et le marketing
- **Évolution indépendante** : Chaque partie peut évoluer séparément

## Performance

- **Next.js** : Optimisations automatiques (SSR, SSG, ISR)
- **CDN ready** : Site client facilement déployable sur Vercel/Netlify
- **Backoffice dédié** : Performance optimale pour les opérations internes

## Sécurité

- **Isolation** : Site client n'a accès qu'aux endpoints nécessaires
- **Permissions granulaires** : Chaque rôle a accès limité
- **Audit complet** : Toutes les actions sont tracées

## Maintenance

- **Code organisé** : Séparation claire des projets
- **Déploiement indépendant** : Mises à jour sans impact sur l'autre partie
- **Tests séparés** : Tests unitaires par application

---

# 📊 Statistiques et KPIs

## Backoffice
- **Chiffre d'affaires** journalier/mensuel/annuel
- **Nombre de rendez-vous** par période
- **Taux de remplissage** du planning
- **Produits/services** les plus vendus
- **Performance du personnel**
- **Taux de fidélisation** des clients
- **Stocks** en alerte
- **Dépenses** par catégorie

## Site Client
- **Nombre de visiteurs** uniques
- **Taux de conversion** (visite → RDV)
- **Pages les plus visitées**
- **Temps passé sur le site**
- **Taux de rebond**
- **Inscriptions** nouvelles
- **Témoignages** déposés

---

# 🎨 Interface Utilisateur

## Backoffice
- **Design professionnel** et fonctionnel
- **Responsive** : Adapté mobile, tablette, desktop
- **Navigation fluide** avec Inertia.js
- **Composants réutilisables** (Radix UI)
- **Feedback utilisateur** en temps réel
- **Tableaux de bord** personnalisables par rôle

## Site Client
- **Design moderne** et attractif
- **Animations fluides** (Framer Motion)
- **Mode sombre/clair**
- **Navigation intuitive**
- **Expérience mobile** optimisée
- **SEO friendly**

---

# 🔧 Personnalisation

## Backoffice
- **Configuration des points** de fidélité
- **Catégories personnalisables** (services, produits, dépenses)
- **Taux de change** multi-devises
- **Règles de congés** et soldes
- **Templates de rapports**
- **Notifications** personnalisables

## Site Client
- **Thème de couleurs** personnalisable
- **Contenu éditable** (textes, images)
- **SEO configurable** (meta tags, descriptions)
- **Pages statiques** modifiables

---

# 📈 Évolutivité

## Backoffice
- Nouveaux modules métier
- Intégrations tierces (comptabilité, marketing)
- Passerelles de paiement supplémentaires
- CRM avancé
- Système de réservation IA

## Site Client
- Application mobile native (React Native)
- Chatbot intelligent
- Système de recommandation
- Intégration réseaux sociaux
- E-commerce complet

---

# 🎯 Cas d'Utilisation

### Salon Indépendant
Gérez votre salon avec le backoffice et offrez un site de réservation moderne à vos clients.

### Chaîne de Salons
Backoffice multi-succursales avec site client unifié ou personnalisé par succursale.

### Franchise
Offrez à vos franchisés un système de gestion standardisé avec site web corporatif.

---

# 💡 Points Forts

✅ **Architecture moderne** : Séparation backoffice/site client
✅ **Next.js 16** : Dernières technologies web
✅ **Performance optimale** : SSR, SSG, ISR
✅ **SEO natif** : Référencement optimisé
✅ **Expérience utilisateur** : Design moderne et animations
✅ **Sécurisé** : Authentification robuste et permissions
✅ **Évolutif** : Architecture modulaire
✅ **Support local** : Développé pour le marché africain (RDC)
✅ **Multi-devises** : Adapté aux économies locales
✅ **SMS intégré** : Communication directe avec les clients

---

# 📞 Support et Maintenance

L'application est conçue pour être maintenue et évolutive, avec :
- Code structuré et documenté
- Tests automatisés
- Mises à jour régulières
- Possibilité de formation des équipes
- Documentation technique complète

---

*Bella Hair - La solution complète pour moderniser votre salon de coiffure*
# Bella Hair - Système de Gestion de Salon de Coiffure

## 📋 Vue d'ensemble

Bella Hair est une solution complète composée de deux applications distinctes mais interconnectées :

1. **Backoffice** : Application de gestion interne pour l'administration du salon (Laravel + React/Inertia.js)
2. **Site Client** : Site web public Next.js pour les clients (Next.js 16 + React 19)

Cette architecture permet une séparation claire des responsabilités tout en assurant une synchronisation des données via une API RESTful.

---

# 🏢 PARTIE BACKOFFICE

## 📋 Description

Le backoffice est l'application de gestion interne utilisée par le personnel du salon (administrateurs, gérants, coiffeurs, caissiers, agents). Il permet de gérer tous les aspects opérationnels et administratifs du salon.

---

## 🛠️ Stack Technique Backoffice

### Backend
- **Laravel 12** : Framework PHP robuste
- **MySQL/SQLite** : Base de données
- **Sanctum** : Authentification API
- **Socialite** : Authentification sociale (Google)
- **Media Library** : Gestion des fichiers médias
- **DomPDF** : Génération de PDF
- **Excel** : Export Excel (Maatwebsite)
- **Twilio** : Envoi de SMS
- **ZKTeco** : Intégration pointage biométrique
- **QR Code** : Génération de codes QR (Simple-QRCode)

### Frontend
- **React 18** : Bibliothèque JavaScript
- **Inertia.js** : Bridge Laravel-React sans API
- **TypeScript** : Typage statique
- **Tailwind CSS 4** : Framework CSS utilitaire
- **Radix UI** : Composants UI accessibles
- **Recharts** : Graphiques et visualisations
- **React Hook Form** : Gestion des formulaires
- **Zod** : Validation de schémas
- **Tremor React** : Composants de dashboard
- **Sonner** : Notifications toast

### Outils de Développement
- **Vite** : Build tool ultra-rapide
- **ESLint** : Linting JavaScript
- **Prettier** : Formatage de code
- **PHPUnit** : Tests unitaires

---

## 🎯 Fonctionnalités Backoffice

### 1. Gestion des Rendez-vous

- **Calendrier interactif** pour visualiser et gérer les créneaux
- **Gestion des statuts** : en attente, confirmé, annulé, terminé
- **Rendez-vous à domicile** avec gestion des frais de déplacement
- **Notifications SMS** automatiques pour rappels et confirmations
- **Paiement échelonné** : acomptes et soldes
- **Historique complet** des rendez-vous par client
- **Confirmation et annulation** par le personnel
- **Messagerie client** intégrée

### 2. Gestion des Clients (CRM)

- **Profils clients complets** : informations personnelles, préférences
- **Historique d'achat** et de visites
- **Système de favoris** pour services et produits
- **Avatars personnalisables**
- **Verification email** et sécurité des comptes
- **Réinitialisation de mot de passe** par SMS/email
- **Création rapide** de clients lors des ventes
- **Statistiques client** : fréquence, montant total, etc.

### 3. Catalogue de Services

- **Services de coiffure** : coupe, coloration, brushing, etc.
- **Catégorisation** des services par type
- **Gestion des prix** et durées
- **Promotions** et prix promotionnels
- **Visibilité contrôlée** (actif/inactif, visible/caché)
- **Images et descriptions** détaillées
- **Statistiques** sur les services les plus demandés
- **Gestion des images** multiples par service

### 4. Gestion des Produits

- **Catalogue de produits** : shampoings, laques, accessoires, etc.
- **Gestion des stocks** en temps réel
- **Alertes de rupture** de stock
- **Catégorisation** des produits
- **Prix d'achat et de vente**
- **Promotions** et soldes
- **Gestion des images** multiples
- **Transfert de stocks** entre succursales
- **Stock global** par produit

### 5. Point de Vente (POS)

- **Vente de produits et services**
- **Facturation automatique** avec codes uniques
- **Modes de paiement** multiples
- **Gestion des remises**
- **Acomptes** et paiements partiels
- **Impression de reçus**
- **Historique des ventes**
- **Statistiques journalières** de ventes
- **Gestion des promotions** en caisse

### 6. Gestion du Personnel (RH)

- **Fiches agents** complètes (informations personnelles, CNSS, etc.)
- **Matricules automatiques**
- **Photos et signatures** numériques
- **Gestion des contrats** de travail
- **Références professionnelles**
- **Assignation aux succursales**
- **Rôles et permissions** : admin, gérant, coiffeur, caissier, agent, community manager
- **Dashboard personnel** pour les agents

### 7. Gestion des Présences

- **Pointage biométrique** (intégration ZKTeco)
- **Pointage manuel** avec notes
- **Suivi des heures** de travail
- **Gestion des pauses**
- **Rapports de présence** quotidiens/mensuels
- **Grilles de pointage** imprimables
- **Historique complet** des présences
- **Génération automatique** des pointages

### 8. Gestion des Congés

- **Demandes de congés** (annuel, maladie, etc.)
- **Workflow d'approbation** par les gestionnaires
- **Suivi des soldes** de congés
- **Statistiques** sur les congés
- **Impression des attestations**
- **Historique** des demandes
- **Types de congés** personnalisables

### 9. Gestion de la Paie

- **Calcul automatique** des salaires
- **Gestion des acomptes** sur salaire
- **Fiches de paie** détaillées
- **Rapports de paie** (PDF, Excel)
- **Historique des paiements**
- **Intégration avec les pointages**
- **Rapports consolidés** de paie

### 10. Programme de Fidélité

- **Système de points** cumulables
- **Cadeaux d'anniversaire** automatiques
- **Configuration flexible** des règles de fidélité
- **Suivi des achats** et montants
- **Niveaux de fidélité**
- **Récompenses personnalisables
- **Statistiques de fidélisation**

### 11. Gestion Multi-Succursales

- **Création de plusieurs succursales**
- **Gestion des stocks** par succursale
- **Transferts de stocks** entre succursales
- **Personnel assigné** par succursale
- **Rapports consolidés** ou par succursale
- **Permissions basées** sur la succursale
- **Validation des transferts**

### 12. Gestion Financière

- **Suivi des dépenses** par catégorie
- **Budgets prévisionnels**
- **Catégories de dépenses** personnalisables
- **Sorties de fonds** avec validation
- **Rapports financiers**
- **Gestion multi-devises** avec taux de change
- **Caisse et encaissements**
- **Acomptes clients**

### 13. Rapports et Statistiques

- **Tableau de bord** avec KPIs en temps réel
- **Statistiques de ventes** (journalières, mensuelles)
- **Analyse des produits** et services les plus vendus
- **Performance des vendeurs**
- **Rapports PDF** exportables
- **Graphiques et visualisations**
- **Filtres par période** et succursale
- **Rapports de synthèse**

### 14. Marketing et Communication

- **Galerie photos** des réalisations
- **Témoignages clients** avec modération
- **Promotions** et offres spéciales
- **Notifications SMS** (Twilio)
- **Alertes internes** pour le personnel
- **Publication de contenu** (community manager)

### 15. Sécurité et Audit

- **Authentification sécurisée** (Sanctum)
- **Rôles et permissions** granulaires
- **Journal d'audit** complet des actions
- **Logs utilisateur** traçables
- **Protection CSRF**
- **Validation des données**
- **Gestion des devices** autorisés

---

## 🔐 Rôles et Permissions Backoffice

- **Admin** : Accès total à toutes les fonctionnalités
- **Gérant** : Gestion de la succursale, rapports, personnel
- **Coiffeur** : Rendez-vous, ventes, pointage
- **Caissier** : Ventes, encaissements, stocks
- **Agent** : Pointage, congés, acomptes, dashboard personnel
- **Community Manager** : Galerie, témoignages, promotions

---

## 📱 Modules Backoffice

1. **Dashboard** : Vue d'ensemble avec statistiques
2. **Rendez-vous** : Gestion complète des appointments
3. **Clients** : CRM et gestion de la clientèle
4. **Services** : Catalogue des prestations
5. **Produits** : Gestion du catalogue et stocks
6. **Ventes** : Point de vente et facturation
7. **Personnel** : Gestion RH et employés
8. **Pointages** : Suivi des présences
9. **Congés** : Gestion des absences
10. **Paie** : Gestion salariale
11. **Stocks** : Gestion des inventaires
12. **Succursales** : Multi-sites
13. **Dépenses** : Comptabilité et budgets
14. **Rapports** : Analytics et export
15. **Fidélité** : Programme de récompenses
16. **Galerie** : Portfolio et médias
17. **Témoignages** : Avis clients
18. **Configuration** : Paramètres système
19. **Audit** : Journal des actions
20. **Alertes** : Notifications internes

---

# 🌐 PARTIE SITE CLIENT

## 📋 Description

Le site client est une application Next.js moderne et responsive qui permet aux clients de :
- Découvrir les services et produits du salon
- Prendre rendez-vous en ligne
- Créer un compte personnel
- Gérer leurs rendez-vous et favoris
- Voir la galerie et laisser des témoignages

Le site communique avec le backoffice via une API RESTful.

---

## 🛠️ Stack Technique Site Client

### Frontend
- **Next.js 16** : Framework React avec App Router
- **React 19** : Bibliothèque JavaScript
- **TypeScript** : Typage statique
- **Tailwind CSS 4** : Framework CSS utilitaire
- **Radix UI** : Composants UI accessibles
- **Shadcn UI** : Composants pré-construits
- **Framer Motion** : Animations fluides
- **Lucide React** : Icônes
- **next-themes** : Gestion du thème (sombre/clair)
- **Base UI** : Composants UI supplémentaires

### Outils de Développement
- **ESLint** : Linting JavaScript
- **PostCSS** : Traitement CSS
- **TypeScript** : Compilation

---

## 🎯 Fonctionnalités Site Client

### 1. Page d'Accueil

- **Hero section** animée avec appel à l'action
- **Présentation des services** populaires
- **Slider des produits** disponibles
- **Témoignages clients** en carousel
- **Galerie photos** des réalisations
- **Design moderne** et responsive
- **Animations fluides** (Framer Motion)

### 2. Authentification

- **Inscription** avec email et mot de passe
- **Connexion** email/mot de passe
- **Authentification Google** (OAuth)
- **Réinitialisation de mot de passe** par email
- **Vérification d'email** avec code
- **Session sécurisée** via API token

### 3. Catalogue de Services

- **Liste complète** des services disponibles
- **Filtrage par catégorie**
- **Détails de chaque service** : description, prix, durée
- **Images des services**
- **Bouton de réservation** directe
- **Pages SEO optimisées** pour chaque service

### 4. Catalogue de Produits

- **Grille de produits** avec images
- **Filtrage par catégorie**
- **Détails produits** : description, prix
- **Gestion des favoris** (pour clients connectés)
- **Pages SEO optimisées** pour chaque produit

### 5. Prise de Rendez-vous

- **Formulaire de réservation** en ligne
- **Sélection du service**
- **Choix de la date et heure**
- **Sélection de la succursale**
- **Options de rendez-vous** : salon ou domicile
- **Calcul automatique** des frais de déplacement
- **Confirmation immédiate** ou en attente

### 6. Espace Client (Dashboard)

- **Profil personnalisé** avec avatar
- **Statistiques** : RDV à venir, commandes, favoris, points fidélité
- **Gestion de l'avatar** (upload/suppression)
- **Informations personnelles** modifiables
- **Liste des favoris** (services et produits)
- **Navigation intuitive** entre les sections

### 7. Gestion des Rendez-vous

- **Liste des rendez-vous** avec pagination
- **Détails de chaque RDV** : date, heure, service, montant
- **Statuts visuels** : confirmé, en attente, annulé
- **Informations sur la succursale**
- **Gestion du paiement** (acompte/solde)
- **Historique complet** des rendez-vous

### 8. Galerie Photos

- **Portfolio visuel** des réalisations
- **Slider automatique** des photos
- **Catégorisation par type** de service
- **Design immersif**
- **Optimisation des images**

### 9. Témoignages

- **Liste des témoignages** clients
- **Possibilité de laisser** un avis (clients connectés)
- **Modération** par le backoffice
- **Affichage des notes**
- **Design attrayant**

### 10. Pages SEO

- **Page "À propos"** : présentation du salon
- **Pages spécialisées** : coiffure mariage, maquillage professionnel
- **Optimisation SEO** : meta tags, sitemap, robots.txt
- **Breadcrumbs** pour la navigation
- **FAQ sections** pour le référencement

### 11. Expérience Utilisateur

- **Design responsive** : mobile, tablette, desktop
- **Mode sombre/clair** avec persistance
- **Animations fluides** et transitions
- **Chargement rapide** (Next.js optimization)
- **Navigation intuitive**
- **Feedback utilisateur** (toasts, loaders)
- **PWA ready** : installation possible sur mobile

### 12. Intégration API

- **Communication RESTful** avec le backoffice
- **Authentification via token**
- **Gestion des erreurs** graceful
- **Loading states** optimisés
- **Cache intelligent** des données

---

## 📱 Pages du Site Client

1. **Accueil** (`/`) : Hero, services, produits, témoignages, galerie
2. **Services** (`/services`) : Catalogue complet des services
3. **Détail Service** (`/services/[uuid]`) : Page individuelle de service
4. **Produits** (`/produits`) : Catalogue des produits
5. **Détail Produit** (`/produits/[uuid]`) : Page individuelle de produit
6. **Galerie** (`/gallerie`) : Portfolio des réalisations
7. **Témoignages** (`/temoignages`) : Avis clients
8. **Connexion** (`/login`) : Formulaire de connexion
9. **Inscription** (`/inscription`) : Formulaire d'inscription
10. **Mot de passe oublié** (`/forgot-password`) : Récupération
11. **Réinitialisation** (`/reset-password`) : Nouveau mot de passe
12. **Vérification email** (`/verify-email`) : Validation compte
13. **Dashboard Client** (`/client/dashboard`) : Espace personnel
14. **Mes Rendez-vous** (`/client/appointments`) : Liste des RDV
15. **Détail RDV** (`/client/rdv/[ref]`) : Détails d'un rendez-vous
16. **Nouveau RDV** (`/rdv/nouveau`) : Formulaire de réservation
17. **Détail RDV Public** (`/rdv/[ref]`) : Vue publique d'un RDV
18. **À propos** (`/apropos`) : Présentation du salon
19. **Coiffure Mariage** (`/coiffure-mariage-kinshasa`) : Page spécialisée
20. **Maquillage Pro** (`/maquillage-professionnel-kinshasa`) : Page spécialisée

---

# 🔗 INTÉGRATION BACKOFFICE - SITE CLIENT

## Communication API

Le site client communique avec le backoffice via une API RESTful sécurisée :

- **Authentification** : Tokens Sanctum
- **Endpoints publics** : Services, produits, galerie, témoignages
- **Endpoints protégés** : Rendez-vous, profil client, favoris
- **Synchronisation en temps réel** des données
- **Gestion des erreurs** centralisée

## Flux de Données

1. **Client s'inscrit** sur le site → Données stockées dans le backoffice
2. **Client prend RDV** → Création dans le backoffice, confirmation par email/SMS
3. **Personnel valide RDV** → Statut mis à jour, notification client
4. **Client laisse témoignage** → Modération via backoffice
5. **Promotions créées** → Affichage automatique sur le site client

---

# 🚀 Avantages de l'Architecture

## Séparation des Responsabilités

- **Backoffice** : Focus sur la gestion interne et l'administration
- **Site Client** : Focus sur l'expérience utilisateur et le marketing
- **Évolution indépendante** : Chaque partie peut évoluer séparément

## Performance

- **Next.js** : Optimisations automatiques (SSR, SSG, ISR)
- **CDN ready** : Site client facilement déployable sur Vercel/Netlify
- **Backoffice dédié** : Performance optimale pour les opérations internes

## Sécurité

- **Isolation** : Site client n'a accès qu'aux endpoints nécessaires
- **Permissions granulaires** : Chaque rôle a accès limité
- **Audit complet** : Toutes les actions sont tracées

## Maintenance

- **Code organisé** : Séparation claire des projets
- **Déploiement indépendant** : Mises à jour sans impact sur l'autre partie
- **Tests séparés** : Tests unitaires par application

---

# 📊 Statistiques et KPIs

## Backoffice
- **Chiffre d'affaires** journalier/mensuel/annuel
- **Nombre de rendez-vous** par période
- **Taux de remplissage** du planning
- **Produits/services** les plus vendus
- **Performance du personnel**
- **Taux de fidélisation** des clients
- **Stocks** en alerte
- **Dépenses** par catégorie

## Site Client
- **Nombre de visiteurs** uniques
- **Taux de conversion** (visite → RDV)
- **Pages les plus visitées**
- **Temps passé sur le site**
- **Taux de rebond**
- **Inscriptions** nouvelles
- **Témoignages** déposés

---

# 🎨 Interface Utilisateur

## Backoffice
- **Design professionnel** et fonctionnel
- **Responsive** : Adapté mobile, tablette, desktop
- **Navigation fluide** avec Inertia.js
- **Composants réutilisables** (Radix UI)
- **Feedback utilisateur** en temps réel
- **Tableaux de bord** personnalisables par rôle

## Site Client
- **Design moderne** et attractif
- **Animations fluides** (Framer Motion)
- **Mode sombre/clair**
- **Navigation intuitive**
- **Expérience mobile** optimisée
- **SEO friendly**

---

# 🔧 Personnalisation

## Backoffice
- **Configuration des points** de fidélité
- **Catégories personnalisables** (services, produits, dépenses)
- **Taux de change** multi-devises
- **Règles de congés** et soldes
- **Templates de rapports**
- **Notifications** personnalisables

## Site Client
- **Thème de couleurs** personnalisable
- **Contenu éditable** (textes, images)
- **SEO configurable** (meta tags, descriptions)
- **Pages statiques** modifiables

---

# 📈 Évolutivité

## Backoffice
- Nouveaux modules métier
- Intégrations tierces (comptabilité, marketing)
- Passerelles de paiement supplémentaires
- CRM avancé
- Système de réservation IA

## Site Client
- Application mobile native (React Native)
- Chatbot intelligent
- Système de recommandation
- Intégration réseaux sociaux
- E-commerce complet

---

# 🎯 Cas d'Utilisation

### Salon Indépendant
Gérez votre salon avec le backoffice et offrez un site de réservation moderne à vos clients.

### Chaîne de Salons
Backoffice multi-succursales avec site client unifié ou personnalisé par succursale.

### Franchise
Offrez à vos franchisés un système de gestion standardisé avec site web corporatif.

---

# 💡 Points Forts

✅ **Architecture moderne** : Séparation backoffice/site client
✅ **Next.js 16** : Dernières technologies web
✅ **Performance optimale** : SSR, SSG, ISR
✅ **SEO natif** : Référencement optimisé
✅ **Expérience utilisateur** : Design moderne et animations
✅ **Sécurisé** : Authentification robuste et permissions
✅ **Évolutif** : Architecture modulaire
✅ **Support local** : Développé pour le marché africain (RDC)
✅ **Multi-devises** : Adapté aux économies locales
✅ **SMS intégré** : Communication directe avec les clients

---

# 📞 Support et Maintenance

L'application est conçue pour être maintenue et évolutive, avec :
- Code structuré et documenté
- Tests automatisés
- Mises à jour régulières
- Possibilité de formation des équipes
- Documentation technique complète

---

*Bella Hair - La solution complète pour moderniser votre salon de coiffure*
