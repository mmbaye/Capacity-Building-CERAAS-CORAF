# Cours de Renforcement 

## R and GitHub 

- [ ] l'objectif de ce tutoriel est de vous guider pour la publication de vos codes sous **GitHub** et la documentation de vos résultats de recherches .  Nous allons créer un projet sous **RStudio**   dans lequel nous allons organiser les dossiers en ***Docs***, ***Figures*** , ***Codes*** et ***Résultats***. Voici les contenus possibles de ces répertoires: 

1. *Docs* , ce dossier contient toute la documentation en rapport avec votre projet, par exemple  vous pouvez décrire les objectifs, le protocole expérimentale etc. 
2. Figures, ce dossier contient la liste des figures qui seront générées en prenant le soin de bien choisir le nom des figures. 
3. Codes, dans ce dossier vous devez  y mettre tous les codes écrits et prenant le choix aussi de commenter les lignes de codes quand c'est nécessaire 
4. le dossier Résultats peut contenir des résultats sous forme de données csv ou texte comme les paramètres du résultats d'une ANOVA , ou d'une régression multiple ou même les paramètres  d'une acp 

## les etapes pour connecter Github et Rstudio project

ouvrir le logiciel Rstudio 

puis aller  create new project

![image-20230713140628417](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713140628417.png)



- click sur l'icone **Open Project**

- click sur New Project  ![image-20230713140825490](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713140825490.png)



- puis dans **New Directory**



![image-20230713141038490](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713141038490.png)



dans la fenêtre suivant donner un nom a votre projet sans espace et le mettre dans  le dossier mes documents 



![image-20230713141441246](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713141441246.png)



Quand le projet R est crée, vous devrez voir une fenêtre comme illustré sur la figure suivante 



![image-20230713141819592](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713141819592.png)

## Création des fichiers du projet



il  y a plusieurs façons de créer de fichiers  et répertoires  sous **R**.  nous allons voir un exemple  en utilisant la fonction ***dir.create()*** de R



````R
dossiers<-c('Docs','Figures','Datas','Codes', 'Results')
lapply(dossiers, dir.create)
````

  Dans le tab Files, vous verrez ce qui suit. 

![image-20230713142500407](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713142500407.png)



Nous allons supposez pour l'instant que vous avez vos  scripts R et  aussi que vous avez généré des figures, des  résultats sous forme de texte, une base de données et de la documentation de votre projet. Nous allons maintenant faire la connexion  entre GitHub et ce projet sous R.  

Ainsi, il faut aller sur l'onglet **Tools**  puis **Version Control** puis **Project Setup**

![image-20230713143652542](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713143652542.png)



quand vous cliquez sur **Project Setup**, une nouvelle fenêtre va s'ouvrir  comme il est indiqué sur la figure ci-dessous. Sur la partie Version control system choisissez **Git**



![image-20230713144200000](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713144200000.png)





si vous avez correctement fait ces étapes, R va actualiser la page et vous verrez un nouvel onglet **Git**  sur R



![image-20230713145504283](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713145504283.png)



cliquez sur l'onglet **Git** pour voir les dossier que vous pouvez partager ou push vers votre GitHub. vous pouvez sélectionner les dossiers que vous voulez partager. Souvent il faut éviter de partager vos données non encore publiées mais vous pouvez bien partager résultats de recherche de données traitées. Mieux encore, vous faire des projets Github privés.

quand l'onglet Git est actif, vous verrez une fenêtre comme la figure ci-dessous 

![image-20230713145926069](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713145926069.png)

Sélectionner les dossiers que vous voulez héberger dans github , puis cliquez sur l'onglet **commit** en prenant le soin de renseigner un  message de commit . 



![image-20230713150139616](C:/Users/ceraas/AppData/Roaming/Typora/typora-user-images/image-20230713150139616.png) 
