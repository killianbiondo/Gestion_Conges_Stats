# Gestion des Congés Symfony

Ce projet est une application Symfony pour la gestion des congés des employés.

## Prérequis

Avant de commencer, assurez-vous d'avoir les outils suivants installés sur votre machine :

- **PHP** (version 8.0 ou supérieure) : [Installer PHP](https://www.php.net/downloads)
- **Composer** : [Installer Composer](https://getcomposer.org/download/)
- **Git** : [Installer Git](https://git-scm.com/downloads)
- **Node.js** : [Installer Node.js](https://nodejs.org/)

## Installation

1. **Cloner le dépôt GitHub**

   Ouvrez un terminal et exécutez la commande suivante pour cloner le projet sur votre machine :

   ```bash
   git clone https://github.com/killianbiondo/GestionCongesSymfony.git

2. **Accéder au répertoire du projet**

Naviguez dans le répertoire du projet cloné :

```bash
cd GestionCongesSymfony
```

3. **Installer les dépendances PHP**

Utilisez Composer pour installer les dépendances du projet :

```bash
composer install
```

4. **Configurer les variables d'environnement**

   Copiez le fichier .env vers .env.local :

```bash
cp .env.env.local
```

Ouvrez le fichier .env.local et configurez les informations de votre base de données. Par exemple :

```bash
DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/nom_de_la_base?serverVersion=8.0"
```

5. **Créer la base de données**

Créez la base de données en utilisant la commande suivante :

```bash
php bin/console doctrine:database:create
```


6. **Lancer les migrations**

Exécutez les migrations pour créer les tables nécessaires :

```bash
php bin/console doctrine:migrations:migrate
```


7.Charger les données de base (optionnel)

Si le projet inclut des fixtures, vous pouvez charger des données de test avec la commande :

```bash
php bin/console doctrine:fixtures:load
```


## Lancer le serveur

Démarrez le serveur de développement Symfony avec la commande suivante :

```bash
symfony server:start
```
Le projet sera alors accessible sur http://127.0.0.1:8000.


## Utilisation

Accéder à l'application : Ouvrez votre navigateur et allez à http://127.0.0.1:8000.
Gestion des utilisateurs et des congés : Une fois connecté, vous pourrez utiliser les différentes fonctionnalités de gestion de congés selon les rôles d’utilisateur définis.




















