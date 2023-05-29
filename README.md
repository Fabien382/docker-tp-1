Ce projet Docker Compose est conçu pour créer un environnement de développement local comprenant WordPress, MySQL/MariaDB, phpMyAdmin et d'autres services connexes. Il vous permettra de facilement lancer et gérer votre site WordPress localement.

Prérequis
Avant de commencer, assurez-vous d'avoir installé Docker et Docker Compose sur votre machine. Vous pouvez les télécharger et les installer à partir des liens suivants :

Docker : https://www.docker.com/get-started
Docker Compose : https://docs.docker.com/compose/install/
Instructions
Clonez ce référentiel sur votre machine locale :

shell
Copy code
git clone https://github.com/Fabien382/docker-tp-1
Accédez au répertoire du projet :

cd docker-wordpress
Démarrez les conteneurs Docker en utilisant Docker Compose :

docker-compose up -d
Cette commande lancera les conteneurs Docker en arrière-plan (option -d) en se basant sur la configuration définie dans le fichier docker-compose.yml.

Attendez que tous les services soient démarrés et opérationnels. Vous pouvez vérifier l'état des conteneurs avec la commande :

docker-compose ps
Accédez à votre site WordPress dans votre navigateur en utilisant l'URL suivante :

http://localhost:8080
Vous pourrez alors procéder à l'installation de WordPress et configurer votre site.

Vous pouvez également accéder à phpMyAdmin pour gérer votre base de données MySQL/MariaDB en utilisant l'URL suivante :

http://localhost:8081
Utilisez les informations de connexion suivantes pour vous connecter à phpMyAdmin :

Serveur : mysql
Utilisateur : root
Mot de passe : admin
Pour arrêter les conteneurs Docker, exécutez la commande suivante dans le répertoire du projet :

docker-compose down
Cela arrêtera les conteneurs Docker associés à ce projet.

Configuration personnalisée
Vous pouvez personnaliser les paramètres du projet en modifiant le fichier docker-compose.yml. Vous pouvez ajuster les variables d'environnement, les volumes, les ports exposés, etc. en fonction de vos besoins spécifiques.

N'oubliez pas de sauvegarder vos modifications et de relancer les conteneurs à l'aide de la commande docker-compose up -d pour appliquer les changements.
