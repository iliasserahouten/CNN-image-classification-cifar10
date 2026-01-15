# Devoir Maison – Réseaux Convolutifs (ING2 Ingénierie Mathématiques)

**Auteur** : Iliass Erahouten  
**Date de début** : 19 Décembre 2025  
**Date de remise** : 03 Janvier 2026  
**Total** : 30 pts  

## Description

Ce devoir maison porte sur l’utilisation des **réseaux de neurones convolutifs (CNN)** pour classifier des images du jeu de données **CIFAR-10**. L’objectif est de construire et d’entraîner un modèle capable de distinguer deux classes d’images parmi les dix disponibles (par exemple : `deer` et `horse`).  

Le projet permet de mettre en pratique les concepts suivants :  

- **Chargement et prétraitement des données** : lecture des batches CIFAR, filtrage des classes, normalisation des pixels et conversion des labels en binaire.  
- **Construction d’un CNN avec Keras** :  
  - Couches de convolution (`Conv2D`) pour extraire les caractéristiques visuelles.  
  - Couches de pooling (`MaxPooling2D`) pour réduire la dimensionnalité tout en conservant l’information essentielle.  
  - Couches d’aplatissement (`Flatten`) et entièrement connectées (`Dense`) pour la classification finale.  
- **Choix des fonctions d’activation et de perte** :  
  - Softmax avec `sparse_categorical_crossentropy` pour une sortie multi-neurones.  
  - Sigmoïde avec `binary_crossentropy` pour la classification binaire.  
- **Optimisation et entraînement** : utilisation de l’optimiseur Adam avec un taux d’apprentissage adapté, suivi de l’évolution de la précision (accuracy) sur les ensembles d’entraînement et de validation.  
- **Évaluation des performances** : comparaison des deux architectures pour identifier la plus performante sur le jeu de test.  

Ce projet permet de consolider les compétences en **Deep Learning**, **prétraitement d’images**, **architecture CNN**, et **implémentation pratique avec Keras**, tout en développant une approche expérimentale pour choisir l’architecture et les hyperparamètres optimaux.

## Références

- Ian Goodfellow, Yoshua Bengio, Aaron Courville – *Deep Learning*  
- Saharon Rosset, Ji Zhu, Trevor Hastie – *Margin Maximizing Loss Functions*  
- [Jeu de données CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)
