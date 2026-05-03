# Présentation de l'application Bella Hair

## Vue d'ensemble

Bella Hair est une application complète de gestion pour salon de coiffure et institut de beauté. Elle centralise les opérations quotidiennes du salon : rendez-vous, clients, ventes, services, produits, stocks, finances, personnel, paie, présences, fidélité, statistiques et contenu du site web.

L'application est conçue pour aider la direction, les gérants, les caissiers, les coiffeurs, les agents et l'équipe communication à travailler dans un seul espace, avec des accès adaptés à chaque rôle.

## Objectif principal

L'objectif de Bella Hair est de digitaliser la gestion du salon afin de réduire les tâches manuelles, mieux suivre les revenus, sécuriser les opérations, améliorer l'expérience client et donner à la direction une vision claire de l'activité.

## Fonctionnalités principales

### Tableau de bord

- Tableau de bord général pour les administrateurs et gérants.
- Tableau de bord spécifique pour les agents.
- Vue rapide des indicateurs importants de l'activité.
- Accès rapide aux modules selon le rôle connecté.
- Recherche dans le menu de navigation pour retrouver rapidement un onglet.

### Gestion des rendez-vous

- Création, consultation, modification et suppression des rendez-vous.
- Suivi des statuts : en attente, confirmé, annulé, terminé ou absent.
- Association d'un rendez-vous à un client, une succursale et des prestations.
- Gestion des montants liés au rendez-vous : total, montant payé, reste à payer, frais de déplacement.
- Paiements liés aux rendez-vous avec historique.
- Confirmation de rendez-vous.
- Envoi de messages personnalisés aux clients.
- Compteur des rendez-vous confirmés à venir.
- API client pour créer et suivre les rendez-vous depuis un espace ou site externe.

### Gestion des clients

- Fiche client complète : nom, téléphone, email, adresse, notes, date de naissance, succursale.
- Création rapide de clients pendant les opérations.
- Historique des ventes et interactions liées au client.
- Gestion de l'avatar client.
- Authentification client côté API avec inscription, connexion, Google OAuth, vérification email et réinitialisation du mot de passe.
- Suivi des statistiques client.

### Produits, accessoires et stocks

- Gestion complète des produits : création, modification, fiche détaillée, images, statut actif/inactif.
- Catégories de produits.
- Gestion des accessoires et utilitaires.
- Gestion du stock global.
- Gestion du stock par succursale.
- Suivi des seuils d'alerte stock.
- API de détection des stocks en rupture, en alerte ou proches du seuil.
- Transferts de stock entre entités ou succursales.
- Validation ou refus des transferts.
- Statistiques par produit et par catégorie.

### Services du salon

- Gestion des services proposés par le salon.
- Catégories de services.
- Images des services.
- Activation ou désactivation des services.
- Statistiques des services.
- Exposition des services via API pour le site web ou une application cliente.

### Ventes et caisse

- Création et suivi des ventes de produits et services.
- Association de la vente à un client, une succursale, un vendeur et une caisse.
- Codes de vente générés automatiquement.
- Gestion des remises.
- Gestion des modes de paiement.
- Gestion des paiements complets ou partiels.
- Impression de ventes/factures.
- Historique des paiements.
- Suivi des acomptes et paiements restants.
- Mise à jour des soldes de caisse.
- Rapport personnel de vente pour les caissiers.

### Programme de fidélité

- Suivi des points de fidélité par client.
- Configuration des règles de points.
- Calcul des points selon les achats.
- Consultation du programme de fidélité.
- Possibilité d'utiliser les points dans certains paiements.
- Gestion de cadeaux ou avantages client, notamment liés aux anniversaires.

### Finances

- Gestion des caisses par succursale.
- Consultation des soldes et transactions de caisse.
- Gestion des dépenses.
- Catégories de dépenses.
- Budgets.
- Sorties financières avec statuts, activation et éléments associés.
- Pièces jointes sur certaines dépenses ou demandes.
- Suivi des paiements et des dépenses par statut.

### Gestion du personnel

- Gestion des agents/personnels.
- Fiches d'identification.
- Affectation aux succursales.
- Gestion des statuts des agents.
- Contrats du personnel.
- Références liées aux agents.
- Gestion de paie.
- Impression de fiches de paie.
- Rapports de paie.
- Export des rapports de paie en PDF et Excel.

### Présences, pointages et pauses

- Gestion des pointages du personnel.
- Présences, absences, congés, maladies, formations et missions.
- Génération journalière ou mensuelle des pointages.
- Calcul des retards et départs anticipés.
- Rapport de présence.
- Impression des pointages et grilles de présence.
- Intégration prévue avec dispositifs de pointage/ZKTeco.
- Gestion des devices de pointage.
- Gestion des pauses/congés avec approbation, rejet, pièces jointes et suivi des statuts.
- Espace personnel pour consulter ses présences, pauses et données de compte.

### Alertes et notifications

- Création et consultation d'alertes.
- Marquage d'une alerte comme lue.
- Alertes côté API pour les clients.
- Notifications email pour plusieurs événements : bienvenue, vérification, mot de passe, rendez-vous confirmé, en attente, annulé, terminé, paiement confirmé, congé accepté.
- Intégration SMS/Twilio présente dans le projet.

### Statistiques et rapports

- Rapport de vente global.
- Rapport de vente détaillé.
- Export PDF des rapports.
- Rapport synthèse.
- Statistiques des ventes.
- Statistiques des vendeurs.
- Statistiques des produits.
- Statistiques des services.
- Statistiques par catégorie de produits.
- Statistiques par catégorie de services.
- Données graphiques pour le suivi des ventes et des performances.
- Rapports individuels pour les caissiers.

### Site web et contenu public

- Gestion des témoignages.
- Publication ou suppression des témoignages.
- Gestion de la galerie.
- Images multiples via médiathèque.
- API publique pour afficher produits, services, branches, témoignages et galerie sur un site web.
- Espace client API pour favoris, rendez-vous, témoignages et profil.

### Administration et sécurité

- Gestion des utilisateurs.
- Gestion des rôles : admin, gérant, caissier, coiffeur, agent, community manager, super admin.
- Menus et accès filtrés selon le rôle.
- Activation/désactivation des utilisateurs.
- Affectation des utilisateurs aux succursales.
- Gestion des succursales.
- Gestion des devises et taux.
- Audit des actions utilisateurs.
- Authentification, vérification email, réinitialisation du mot de passe.
- API protégée par Laravel Sanctum.
- Suppression logique sur plusieurs entités importantes pour préserver l'historique.

## Avantages pour le salon

- Centralisation des informations dans un seul outil.
- Meilleur suivi des ventes, paiements, caisses et dépenses.
- Réduction des pertes grâce au suivi des stocks et seuils d'alerte.
- Organisation plus professionnelle des rendez-vous.
- Meilleure visibilité sur les performances des vendeurs, services et produits.
- Suivi RH complet : personnel, contrats, présences, congés, paie.
- Historique et audit pour mieux contrôler les opérations.
- Programme de fidélité pour encourager les clients à revenir.
- Expérience client améliorée grâce aux confirmations, notifications et espace client.
- Support multi-succursales pour accompagner la croissance du salon.
- Rapports PDF/Excel utiles pour la direction, la comptabilité et les réunions.

## Profils utilisateurs prévus

- Administrateur : accès complet à la gestion, aux statistiques, aux finances, aux utilisateurs et à la configuration.
- Gérant : supervision des opérations, finances, personnel, stocks, rapports et succursales selon les permissions.
- Caissier : ventes, paiements, caisse, rendez-vous, clients, dépenses autorisées et rapport personnel.
- Coiffeur : accès aux clients, rendez-vous, ventes/services selon les droits, dépenses autorisées et données personnelles.
- Agent : tableau de bord personnel, compte, présences et pauses.
- Community manager : gestion orientée contenu, services, produits visibles, galerie, témoignages et rendez-vous selon les droits.
- Client : accès API pour inscription, connexion, favoris, rendez-vous, paiements, témoignages et profil.

## Points forts à présenter au client

- L'application ne gère pas seulement les ventes : elle couvre tout le fonctionnement du salon.
- Le système est adapté à une entreprise multi-branches.
- Les droits d'accès sont séparés par rôle, ce qui limite les erreurs et protège les données sensibles.
- Les statistiques donnent une vision claire des performances commerciales.
- Les modules RH et paie permettent de suivre le personnel sans outil séparé.
- Le programme de fidélité aide à transformer les clients occasionnels en clients réguliers.
- L'application peut alimenter un site web ou une application mobile grâce aux API publiques et client.
- Les impressions et exports facilitent les justificatifs, les rapports et la comptabilité.

## Technologies utilisées

- Backend : Laravel.
- Frontend : React avec Inertia.js.
- Interface : Tailwind CSS, composants UI et icônes Lucide.
- Base API : Laravel Sanctum.
- PDF : DomPDF et FPDF.
- Exports : Excel.
- Médias : Spatie Media Library.
- Graphiques : Recharts.
- Notifications : emails Laravel, intégration SMS/Twilio présente.
- Pointage : intégration ZKTeco présente dans les dépendances et routes.

## Résumé commercial

Bella Hair est une solution de gestion tout-en-un pour salon de coiffure. Elle permet de piloter les rendez-vous, les clients, les ventes, les stocks, les finances, le personnel, la paie, la fidélité et les statistiques depuis une seule plateforme. Pour un client, l'intérêt principal est d'avoir un outil qui améliore l'organisation, renforce le contrôle, professionnalise le service client et donne à la direction les informations nécessaires pour prendre de meilleures décisions.
