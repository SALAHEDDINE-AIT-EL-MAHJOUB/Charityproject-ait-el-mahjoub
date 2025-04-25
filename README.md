# Projet de Charité

Une application web complète de gestion de dons et d'actions caritatives développée avec Spring Boot. Cette plateforme permet de connecter les donateurs avec les organisations caritatives et de gérer efficacement les campagnes de dons.

## Fonctionnalités Principales

- **Gestion des Utilisateurs**
  - Authentification sécurisée avec JWT
  - Gestion des rôles (Super Admin, Organisation, Utilisateur)
  - Profils utilisateurs personnalisables

- **Gestion des Campagnes**
  - Création et gestion de campagnes caritatives
  - Suivi des objectifs de dons
  - Catégorisation des campagnes
  - Tableau de bord des statistiques

- **Système de Dons**
  - Processus de don sécurisé
  - Historique des donations
  - Système de paiement intégré
  - Reçus de dons automatisés

- **Gestion des Organisations**
  - Profils d'organisations vérifiés
  - Suivi des actions caritatives
  - Rapports d'impact

- **Notifications**
  - Système de notifications en temps réel
  - Alertes par email
  - Suivi des activités

## Technologies Utilisées

### Backend
- Java 17
- Spring Boot
- Spring Security avec JWT
- Spring Data JPA
- Maven
- MongoDB

### Sécurité
- JWT (JSON Web Tokens)
- Spring Security
- Gestion des sessions
- Authentification personnalisée

## Prérequis

- JDK 17 ou supérieur
- Maven 3.6+
- MongoDB 4.4+
- Un IDE Java (IntelliJ IDEA recommandé)

## Installation

1. Clonez le dépôt :
```bash
git clone https://github.com/votre-username/Charityproject1.git
cd Charityproject1
```

2. Configurez MongoDB :
   - Installez MongoDB
   - Le serveur doit être accessible sur : `mongodb://localhost:27017`
   - La base de données sera automatiquement créée au démarrage

3. Configurez l'application :
   - Ouvrez `src/main/resources/application.properties`
   - Vérifiez les paramètres de connexion à MongoDB
   - Ajustez les paramètres de sécurité si nécessaire

4. Construisez le projet :
```bash
mvn clean install
```

5. Lancez l'application :
```bash
mvn spring-boot:run
```

L'application sera accessible à l'adresse : `http://localhost:8080`

## Structure du Projet

```
src/
├── main/
│   ├── java/org/project/
│   │   ├── config/          # Configuration Spring et Sécurité
│   │   ├── controller/      # Contrôleurs REST
│   │   ├── model/          # Entités JPA
│   │   ├── repository/     # Repositories Spring Data
│   │   ├── service/       # Logique métier
│   │   ├── DTOs/          # Objets de transfert de données
│   │   ├── util/          # Classes utilitaires
│   │   └── filter/        # Filtres de sécurité
│   └── resources/
│       └── application.properties  # Configuration
└── test/                  # Tests unitaires et d'intégration
```

## API Endpoints Principaux

- `/api/auth/*` - Authentification et gestion des utilisateurs
- `/api/campagnes/*` - Gestion des campagnes
- `/api/organisations/*` - Gestion des organisations
- `/api/dons/*` - Gestion des dons
- `/api/admin/*` - Administration système

## Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Forkez le projet
2. Créez une branche pour votre fonctionnalité
3. Committez vos changements
4. Poussez vers la branche
5. Ouvrez une Pull Request

## Support

Pour toute question ou problème, veuillez ouvrir une issue sur GitHub.

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.
