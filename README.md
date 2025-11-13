✈️ Flight Booking App

Une application Android moderne permettant d’afficher des vols, leurs détails, et le billet électronique (E-Ticket) d’un passager.
L’interface est conçue avec Material Design, des RecyclerView, et des CardView pour une présentation claire et esthétique.

📱 Fonctionnalités principales

🔍 Liste des vols disponibles avec le nom de la compagnie, les horaires, la durée et le prix.

📊 Filtres dynamiques : trier les vols du plus cher au moins cher, ou inversement.

🧾 Détails d’un vol : visualiser le billet complet avec toutes les informations de vol.

🎫 E-Ticket : affichage d’un ticket électronique avec code-barres, détails du passager et conditions.

🎨 Interface moderne et responsive utilisant CardView, LinearLayout, ScrollView et des icônes personnalisées.

🧩 Structure du projet
1. activity_main.xml

Affiche la liste des vols avec :

En-tête indiquant la date, les codes des aéroports de départ et d’arrivée.

Filtres horizontaux (High to Low, Low to High, Airlines Type).

Un RecyclerView (rvFlightList) listant tous les vols disponibles.

Fichier associé : MainActivity.kt
Layout item : item_flight.xml

2. item_flight.xml

Élément individuel de la liste des vols :

Logo et nom de la compagnie aérienne.

Code et heure de départ et d’arrivée.

Durée du vol, prix, et informations supplémentaires (repas gratuits, code promo, etc.).

Design basé sur CardView avec bordure violette (@color/purple_500).

3. activity_flight_detail.xml

Affiche le billet électronique (E-Ticket) du passager :

Logo de la compagnie aérienne.

Détails du vol (lieux, durée, horaire, terminal, siège).

Informations sur le passager et les services inclus.

Code-barres et numéro de ticket.

Bouton de téléchargement du E-Ticket.

Fichier associé : FlightDetailActivity.kt

🖼️ Ressources graphiques

Les fichiers d’images et d’icônes se trouvent dans res/drawable/ :

Ressource	Description
ic_back_arrow.xml	Icône retour
ic_edit.xml	Icône édition
ic_filter.xml	Icône de filtre
ic_airline_placeholder.xml	Logo par défaut pour les compagnies
header_gradient_background.xml	Dégradé pour l’en-tête
badge_background.xml	Fond des badges
promo_background.xml	Fond des codes promo
button_bg.xml	Bouton de téléchargement du billet
barcode_sample.png	Image exemple du code-barres
⚙️ Technologies utilisées

Langage : Kotlin / Java

Android SDK : 21+

Layout : XML

Composants :

RecyclerView

CardView

ScrollView

LinearLayout

FrameLayout

Design System : Material Components for Android

🧠 Fonctionnement simplifié

L’utilisateur ouvre l’application → voit la liste des vols (RecyclerView).

Il peut appliquer un filtre ou trier les résultats.

En cliquant sur un vol, il accède au détail complet (FlightDetailActivity).

Il peut ensuite télécharger ou afficher son E-Ticket.

🚀 Améliorations possibles

Ajouter une base de données locale (Room) ou une API pour les données réelles.

Implémenter une fonction de recherche par ville ou compagnie.

Ajouter une authentification utilisateur (connexion/inscription).

Génération dynamique du code-barres selon le ticket.

Ajout du mode sombre (Dark Mode).

👩‍💻 Auteur

Asma Blh
Étudiante en Développement Digital – Option Mobile
📍 Maroc
💬 Passionnée par la création d’applications Android modernes et intuitives.
