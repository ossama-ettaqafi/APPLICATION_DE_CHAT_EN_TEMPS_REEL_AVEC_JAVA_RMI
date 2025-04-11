# 💬 Application de Chat en Temps Réel avec RMI – Cahier des charges

> Ce document présente les spécifications de l’application **de chat en temps réel développée en Java avec RMI**. Elle permet à plusieurs utilisateurs de communiquer de façon instantanée dans une salle de discussion virtuelle, via une interface simple, rapide et sécurisée.

<div align="center">
   <h3>📸 Aperçu de l'application</h3>
   <img src="https://github.com/imossama/APPLICATION_DE_CHAT_EN_TEMPS_REEL_AVEC_JAVA_RMI/assets/119759894/42ce0764-04ea-4b3b-9ff6-f11b5eec67b0" width="500"/>
</div>

## 🗂 Table des matières

- [🎯 Objectifs](#-objectifs)  
- [⚙️ Fonctionnalités](#-fonctionnalités)  
- [🧱 Technologies utilisées](#-technologies-utilisées)  
- [🚀 Installation et utilisation](#-installation-et-utilisation)

## 🎯 Objectifs

Le projet vise à développer une **application de chat simple, rapide et fonctionnelle** reposant sur le middleware **Java RMI**.  
Les objectifs spécifiques sont :

- 👤 **Interface intuitive** pour la saisie du nom d'utilisateur et l'accès à la salle.  
- 📡 **Communication instantanée** entre clients et serveur via RMI.  
- 🔐 **Sécurité basique intégrée**, avec protection contre les doublons de pseudo.  
- 🔄 **Expérience fluide** en réception et affichage des messages en temps réel.

## ⚙️ Fonctionnalités

### 🧑‍💻 Interface utilisateur

- Champ de saisie du **nom d’utilisateur** avant la connexion.
- Liste dynamique des **utilisateurs connectés**.
- Zone d’affichage des **messages en temps réel**.

### 💬 Communication instantanée

- Échange **instantané** de messages texte entre utilisateurs.
- Actualisation automatique de la discussion sans rechargement manuel.

### 🏠 Salle de chat unique

- Une seule **salle de discussion commune** à tous les utilisateurs.
- Possibilité de **rejoindre / quitter** librement la salle.

### 🛡️ Gestion des utilisateurs

- Validation de l’**unicité des pseudos** à l’entrée.
- Suppression automatique des utilisateurs déconnectés de la liste.

## 🧱 Technologies utilisées

| **Composant**        | **Technologie / Outil**              |
|----------------------|--------------------------------------|
| ☕ Langage            | Java (JDK 17+)                       |
| 🖼️ Interface UI      | Java Swing                           |
| 🌐 Communication      | Java RMI (Remote Method Invocation) |
| 🔧 Compilation       | `javac`, `rmic`, `java`              |

## 🚀 Installation et utilisation

1. 📥 **Cloner** le dépôt GitHub :
   ```bash
   git clone https://github.com/imossama/APPLICATION_DE_CHAT_EN_TEMPS_REEL_AVEC_JAVA_RMI
   ```
2. ⚙️ **Compiler** tous les fichiers `.java` :
   ```bash
   javac *.java
   rmic ChatImpl
   ```
3. 🖥️ **Lancer le serveur RMI** :
   ```bash
   start rmiregistry
   java ChatServer
   ```
4. 👥 **Démarrer un ou plusieurs clients** :
   ```bash
   java ChatClient
   ```
