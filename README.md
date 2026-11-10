<p align="center">
  <img src="images/LOGO%20EventHUB.png" width="160" alt="EventHub Logo">
</p>

<h1 align="center">EventHub – Gestion des événements et des salles de l'IHEC</h1>

<p align="center">
  <b>Projet universitaire en équipe • Java • POO • Swing</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/POO-8A2BE2" alt="POO">
  <img src="https://img.shields.io/badge/Swing-5382A1" alt="Swing">
  <img src="https://img.shields.io/badge/UML-blue" alt="UML">
</p>

---

## Présentation du projet
EventHub est une application de bureau en **Java** qui gère les événements organisés par les clubs de l'IHEC et les réservations des salles. Chaque utilisateur accède à un espace adapté à son rôle : administrateur, responsable de club ou étudiant.

Projet réalisé en équipe dans le cadre du module de programmation orientée objet.

## Mon rôle
Dans l'équipe, j'ai pris en charge **la conception** de l'application : la modélisation UML, notamment le diagramme de classes (utilisateurs et rôles, salles, événements, réservations), qui a servi de base à l'organisation du code.

---

## Fonctionnalités
- **Authentification et rôles** : administrateur, responsable de club, étudiant
- **Administrateur** : gestion des salles et de leurs équipements, validation ou refus des demandes de réservation avec motif, gestion des utilisateurs, statistiques globales
- **Responsable de club** : création d'événements, demandes de réservation de salle, suivi et annulation de ses demandes
- **Étudiant** : consultation des salles disponibles et du calendrier des événements
- **Version console** : un menu texte complet en plus de l'interface graphique

---

## Architecture
Le code suit une organisation en trois couches :

| Dossier | Contenu |
|---|---|
| `src/models` | Les classes métier : `Utilisateur` et ses sous-classes (`Admin`, `ResponsableClub`, `Etudiant`), `Salle`, `Evenement`, `Reservation`, `Equipement` et les énumérations |
| `src/service` | La logique métier : `GestionUtilisateurs`, `GestionSalles`, `GestionEvenements`, `GestionReservations` (pattern **Singleton**) |
| `src/ui` | L'interface graphique **Swing** : écran de connexion, tableaux de bord par rôle et fenêtres de gestion |
| `src/Main/java` | Les points d'entrée : `MainUI` (interface graphique) et `Main` (version console) |

Les données sont gérées en mémoire avec les collections Java, sans base de données.

---

## Aperçu de l'interface
<p align="center">
  <img src="images/1.png" width="260" alt="Capture 1">
  <img src="images/2.png" width="260" alt="Capture 2">
  <img src="images/3.png" width="260" alt="Capture 3">
</p>
<p align="center">
  <img src="images/4.png" width="260" alt="Capture 4">
  <img src="images/5.png" width="260" alt="Capture 5">
  <img src="images/6.png" width="260" alt="Capture 6">
</p>
<p align="center">
  <img src="images/7.png" width="260" alt="Capture 7">
  <img src="images/8.png" width="260" alt="Capture 8">
  <img src="images/9.png" width="260" alt="Capture 9">
</p>
<p align="center">
  <img src="images/10.png" width="260" alt="Capture 10">
  <img src="images/11.png" width="260" alt="Capture 11">
  <img src="images/12.png" width="260" alt="Capture 12">
</p>
<p align="center">
  <img src="images/13.png" width="260" alt="Capture 13">
</p>

---

## Technologies
- Java
- Programmation orientée objet : héritage, encapsulation, énumérations
- Swing (interface graphique)
- Pattern Singleton
- UML (conception)

---

## Lancer le projet
1. Importer le projet dans Eclipse ou IntelliJ IDEA, avec `src` comme dossier source.
2. Lancer la classe `MainUI` (dans `src/Main/java`) pour l'interface graphique, ou `Main` pour la version console.

---

<p align="center">
  <i>Dépôt destiné à la présentation du projet dans un cadre académique (portfolio).</i>
</p>
