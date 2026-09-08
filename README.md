🔐 Portail Sécurisé IAM - Démonstration Keycloak
🎯 Objectif du projet
Ce projet démontre la mise en place d'une infrastructure de Gestion des Identités et des Accès (IAM) à l'aide de Keycloak. Il illustre de manière pratique les concepts fondamentaux de la sécurité des identités en entreprise.
🛠️ Concepts mis en œuvre
JML (Joiner, Mover, Leaver) : Gestion du cycle de vie des utilisateurs (création, promotion en changeant de rôle, désactivation au départ).
RBAC (Role-Based Access Control) : Contrôle d'accès basé sur les rôles avec la création de `role\_employe` et `role\_manager`.
Moindre Privilège : Attribution stricte des droits minimums requis par défaut.
MFA (Multi-Factor Authentication) : Sécurisation des accès par OTP (One-Time Password) via des actions requises (Required Actions).
SSO (Single Sign-On) : Authentification unique permettant d'accéder à plusieurs applications du Realm sans reconnexion.
🚀 Comment lancer le projet en local
Prérequis
Docker Desktop installé et en cours d'exécution.
Installation et Démarrage
Clonez ce dépôt sur votre machine :
```bash
   git clone <https://github.com/RamaDIA26>
   cd Projet-IAM-Keycloak
   ```
Lancez le serveur avec Docker Compose :
```bash
   docker-compose up -d
   ```
Accédez à l'interface d'administration : http://localhost:9090
Identifiant : `admin`
Mot de passe : `admin`
> \*\*Note :\*\* Au démarrage, le conteneur importe automatiquement le fichier `realm-export.json`. Toute la configuration (Realm `MaStartup`, rôles, actions MFA) est immédiatement dispo
