# Développement et déploiement d’un Portail de Gestion des Comptes Clients

## 📌 Contexte

Concevoir et développer une application web permettant aux **clients** de gérer leurs comptes bancaires :
- Consulter le solde
- Voir l’historique des transactions
- Demander un chéquier
- Soumettre une demande de financement
- Suivre l’avancement de leurs requêtes

Le tout dans une **architecture sécurisée**, avec un **déploiement automatisé** grâce au CI/CD et à la conteneurisation Docker.

---

## 🛠️ Technologies et Outils

| Catégorie | Technologies / Outils |
|-----------------|-----------------------------|
| **Backend** | Spring Boot (Java) |
| **Frontend** | Thymeleaf, Tailwind CSS |
| **Base de données** | PostgreSQL |
| **Sécurité / Authentification** | Spring Security, Keycloak |
| **Gestion de versions** | Git, GitHub |
| **CI/CD** | GitHub Actions |
| **Conteneurisation** | Docker |
| **Modélisation** | UML |

---

## ✅ Architecture Backend

- **Contrôleurs REST** pour recevoir les requêtes du frontend
- **Services** pour la logique métier (validation, règles)
- **DAO/Repositories** pour communiquer avec la base PostgreSQL
- Exemple : Un client soumet une demande ➜ Contrôleur ➜ Service ➜ Base

---

## ✅ Architecture Frontend

- Génération de pages HTML dynamiques avec **Thymeleaf**
- Mise en forme moderne et responsive avec **Tailwind CSS**

---

## 🔒 Sécurité

- Authentification et gestion des rôles avec **Keycloak** et/ou **Spring Security**
- Permissions pour contrôler l’accès aux fonctionnalités selon le rôle (client, agent, admin)

---

## 🗂️ Conception et Modélisation

- Diagrammes **UML** pour illustrer :
  - Cas d’utilisation
  - Modèles de données
  - Diagramme de classes
  - Diagramme de séquence

---

## 👥 Types d’utilisateurs

| Utilisateur | Rôle |
|----------------|-------------------------------------------|
| **Client** | Gérer son compte, consulter solde et transactions, faire des demandes (chéquier, financement), suivre ses requêtes |
| **Agent Bancaire** | Gérer les comptes clients, traiter les demandes de financement, valider/refuser les requêtes |
| **Administrateur** | Gérer les utilisateurs, attribuer les rôles, superviser l’ensemble du portail |

---

## ✅ 📌 Fonctionnalités par utilisateur

### ✔️ **1) Client**

- Se connecter / créer un compte
- Consulter les informations personnelles
- Voir le solde de ses comptes
- Consulter l’historique des transactions
- Demander un chéquier
- Soumettre une demande de financement
- Suivre le statut de ses demandes

---

### ✔️ **2) Agent Bancaire**

- Accéder à la liste des clients
- Consulter la fiche client
- Valider ou suspendre un compte
- Consulter toutes les demandes de financement
- Valider / refuser une demande
- Ajouter des commentaires

---

### ✔️ **3) Administrateur**

- Gérer les comptes agents et clients
- Définir les droits d’accès
- Superviser le système (logs, statistiques)
- Configurer les paramètres de sécurité

---

## 🚀 CI/CD et Déploiement

- **GitHub Actions** : pipeline automatisé pour compiler, tester et déployer
- **Docker** : conteneurisation de l’application pour un déploiement reproductible

---

## ✅ 📌 En résumé

> **Projet :** Développement et déploiement d’un portail sécurisé de gestion des comptes clients, intégrant la gestion des demandes de financement, avec une architecture moderne et un pipeline CI/CD automatisé.

---

**🔗 Projet versionné sur GitHub, prêt à être déployé en production.**

--- 
## 📌 Remarques
### C'est quoi une demande de financement ?
👉 **Définition simple :**
Une demande de financement, c’est **quand un client (ou une entreprise) demande de l’argent à la banque** sous forme de **prêt**, **crédit**, ou **subvention**.

📌 **Exemple concret :**
Un agriculteur veut acheter un tracteur ➜ il n’a pas assez d’argent ➜ il va à AL AKHDAR BANK ➜ il **remplit une demande de financement** ➜ la banque étudie sa demande ➜ si tout est OK, la banque lui donne le crédit pour acheter le tracteur.

C’est un **processus administratif** et financier pour demander de l’argent à prêter.
