#  🚀 Guide d'Installation et de Déploiement 🚀

Ce guide vous aidera à cloner le dépôt Git, configurer votre environnement sur Azure, et déployer l'application à l'aide de GitHub Actions.

## 1ère étape : Clonage du dépôt Git

```bash
git clone https://github.com/enzo0039/devops2.git
cd devops2
```

## 2ème étape : Création du dépôt Git

Créez un nouveau dépôt sur GitHub. Assurez-vous d'avoir les droits de lecture et d'écriture sur ce dépôt.

## 3ème étape : Connexion au portail Azure

Connectez-vous au [Portail Azure](https://portal.azure.com).

## 4ème étape : Création d'une Web App

Dans le portail Azure, créez une nouvelle Web App. Choisissez le plan d'hébergement qui convient le mieux à vos besoins.

## 5ème étape : Configuration du Centre de Déploiement

Accédez au centre de déploiement de votre Web App dans le portail Azure. Sélectionnez GitHub comme source de déploiement, puis suivez les instructions pour vous connecter à votre compte GitHub et sélectionner le dépôt que vous venez de créer.

## 6ème étape : Intégration de l'Action GitHub

Une fois votre dépôt connecté à Azure, accédez à l'onglet Actions dans votre dépôt GitHub. Activez les actions GitHub et modifier le fichier YAML (main_tp2devops.yml) pour votre flux de travail.

## 7ème étape : Configuration des paramètres Azure

Copiez ces crédentials à la fin de votre fichier .yml :

```bash
client-id: ${{ secrets.__clientidsecretname__ }}
tenant-id: ${{ secrets.__tenantidsecretname__ }}
subscription-id: ${{ secrets.__subscriptionidsecretname__ }}
```

## 8ème étape : Lancement de l'Action GitHub

Effectuez un commit et un push sur votre dépôt Git pour déclencher le flux de travail GitHub Actions. Suivez les étapes de déploiement et vérifiez que votre application est correctement déployée sur Azure Web App.

Vous avez maintenant déployé avec succès votre application Python sur Azure Web App en utilisant GitHub Actions ! 🚀🚀🚀🚀
