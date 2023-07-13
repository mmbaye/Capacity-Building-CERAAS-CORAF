# Intduction à l'utilisation de Git Bash sous Windows

Bonjour à tous ! Aujourd'hui, nous allons explorer Git Bash, une interface en ligne de commande pour **Git**, un système de contrôle de version très populaire. Dans cette présentation, nous allons apprendre à utiliser Git Bash sous Windows et nous allons également inclure quelques exercices pratiques pour vous aider à vous familiariser avec l'outil. Commençons !

## *Qu'est-ce que Git Bash ?*

- Git Bash est une interface en ligne de commande qui offre une expérience Git complète sur Windows.
- Il fournit un environnement Unix-like sur Windows, vous permettant d'exécuter des commandes Git et d'autres commandes Unix directement depuis l'invite de commande.

## **Installation de Git Bash **

- Rendez-vous sur le site officiel de Git ([https://git-scm.com](https://git-scm.com/)) et téléchargez l'installateur Git pour Windows.
- Exécutez l'installateur et suivez les étapes d'installation par défaut.
- Une fois l'installation terminée, vous pouvez ouvrir Git Bash à partir du menu Démarrer ou en faisant un clic droit dans n'importe quel dossier et en sélectionnant "Git Bash Here".

## **Configuration de Git Bash**

- Avant de commencer à utiliser Git Bash, vous devez configurer votre nom d'utilisateur et votre adresse e-mail. Vous pouvez le faire en exécutant les commandes suivantes dans Git Bash :
  - git config --global user.name "Votre nom"
  - git config --global user.email "[votre@email.com](mailto:votre@email.com)"
- Ces informations seront utilisées pour enregistrer vos contributions dans les projets Git.

## **Principales commandes Git Bash**

- git init : Initialise un nouveau référentiel Git dans le répertoire actuel.
- git clone <URL> : Clone un référentiel Git distant sur votre machine locale.
- git add <fichier> : Ajoute un fichier à l'index de suivi.
- git commit -m "Message de commit" : Enregistre les modifications dans le référentiel avec un message de commit.
- git push : Publie les modifications locales vers un référentiel distant.
- git pull : Récupère les dernières modifications d'un référentiel distant et les fusionne avec votre branche locale.

##  ## **Exercice pratique 1 - Initialisation d'un référentiel **

1. Ouvrez Git Bash et accédez au répertoire dans lequel vous souhaitez créer un référentiel Git.
2. Utilisez la commande "git init" pour initialiser un nouveau référentiel.
3. Vérifiez que le dossier .git a été créé dans le répertoire.

## Exercice pratique 2 - Clonage d'un référentiel distant

1. Trouvez un référentiel Git public en ligne que vous souhaitez cloner.
2. Dans Git Bash, utilisez la commande "git clone <URL>" pour cloner le référentiel sur votre machine locale.
3. Vérifiez que les fichiers du référentiel distant ont été copiés sur votre machine.

## Exercice pratique 3 - Ajout et validation de modifications 

1. Modifiez un fichier dans le référentiel cloné.
2. Dans Git Bash, utilisez la commande "git add <fichier>" pour ajouter le fichier modifié à l'index de suivi.
3. Utilisez la commande "git commit -m "Message de commit"" pour enregistrer les modifications dans le référentiel avec un message de commit.
4. Vérifiez que les modifications ont été enregistrées avec succès.

## Exercice pratique 4 - Publier et récupérer des modifications :

1. Dans Git Bash, utilisez la commande "git push" pour publier les modifications locales vers le référentiel distant.
2. Vérifiez que les modifications ont été publiées avec succès.
3. Si d'autres contributeurs ont apporté des modifications au référentiel distant, utilisez la commande "git pull" pour récupérer les dernières modifications et les fusionner avec votre branche locale.

Conclusion : Dans cette présentation, nous avons découvert Git Bash, une interface en ligne de commande pour Git sous Windows. Nous avons appris comment l'installer, le configurer et utiliser quelques-unes des commandes essentielles. N'hésitez pas à pratiquer davantage pour devenir plus à l'aise avec Git Bash. Merci de votre attention !