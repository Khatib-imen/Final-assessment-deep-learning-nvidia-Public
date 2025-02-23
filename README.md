# Final-assessment-deep-learning-nvidia
# Classification de fruits frais et pourris avec PyTorch

Ce projet consiste à entraîner un modèle de classification d'images pour distinguer les fruits frais des fruits pourris. Le modèle est basé sur l'architecture VGG16 pré-entraînée sur ImageNet, et utilise des techniques de transfer learning, d'augmentation de données et de fine-tuning pour atteindre une précision de validation d'au moins 92%.

## Contexte

Le dataset utilisé provient de [Kaggle](https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification) et contient des images de six catégories de fruits : pommes fraîches, bananes fraîches, oranges fraîches, pommes pourries, bananes pourries et oranges pourries. L'objectif est de classer correctement ces images en utilisant un modèle de deep learning.

## Structure du projet

Le projet est structuré en plusieurs étapes :

1. **Chargement du modèle de base** : Utilisation de VGG16 pré-entraîné sur ImageNet.
2. **Gel des couches du modèle de base** : Pour préserver les connaissances acquises sur ImageNet.
3. **Ajout de couches personnalisées** : Ajout de couches fully connected pour adapter le modèle à notre problème de classification.
4. **Compilation du modèle** : Définition de la fonction de perte et de l'optimiseur.
5. **Préparation des données** : Application de transformations et d'augmentations sur les images.
6. **Chargement des datasets** : Chargement des ensembles d'entraînement et de validation.
7. **Entraînement du modèle** : Entraînement du modèle sur les données d'entraînement.
8. **Fine-tuning** : Dégel des couches du modèle de base et ajustement fin avec un taux d'apprentissage réduit.
9. **Évaluation du modèle** : Évaluation de la précision du modèle sur l'ensemble de validation.
10. **Exécution de l'évaluation** : Vérification que le modèle atteint une précision de validation d'au moins 92%.

## Résultats

Le modèle a atteint une précision de validation de **92%** ou plus, ce qui est le seuil requis pour réussir l'évaluation. Les résultats détaillés sont disponibles dans le notebook `07_assessment.ipynb`.

## Comment exécuter le code

1. **Cloner le dépôt** :
   ```bash
   git clone https://github.com/votre-utilisateur/fruits-classification.git
   cd fruits-classification
2- Installer les dépendances :
Assurez-vous d'avoir installé les bibliothèques nécessaires, notamment torch, torchvision, et PIL.

3- Exécuter le notebook :
Ouvrez le notebook 07_assessment.ipynb dans un environnement Jupyter et exécutez les cellules dans l'ordre.

4- Entraînement et évaluation :
Le notebook contient des instructions pour entraîner le modèle et évaluer sa précision sur l'ensemble de validation.

Dépendances
Python 3.8 ou supérieur

PyTorch

TorchVision

PIL (Pillow)



Ce projet a été réalisé dans le cadre du cours NVIDIA DLI sur le deep learning. Merci à NVIDIA pour leur support et leurs ressources éducatives.
