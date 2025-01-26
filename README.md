# Modèle de Reconnaissance des Émotions Faciales (FER)

Ce projet montre la création d'un modèle d'apprentissage profond pour reconnaître les émotions faciales à partir du dataset FER-2013.

## Étapes pour créer le modèle

### 1. Préparation des données

- **Dataset** : Utiliser le dataset **FER-2013**, composé de 35 887 images en niveaux de gris (48x48 pixels), étiquetées avec 7 émotions : colère, dégoût, peur, joie, tristesse, surprise, et neutre.
- **Normalisation** : Les valeurs des pixels sont normalisées entre [0, 1].
- **Encodage** : Convertir les étiquettes en format one-hot pour la classification.

### 2. Construction du modèle

- **Type de modèle** : Utiliser un **réseau de neurones convolutif (CNN)**.
- **Architecture** : Ajouter des couches convolutionnelles, des couches de pooling, et des couches fully connected.
- **Sortie** : Utiliser une couche Softmax pour la classification des 7 émotions.

### 3. Entraînement du modèle

- **Fonction de perte** : Utiliser l'**entropie croisée catégorielle**.
- **Optimiseur** : Utiliser l'optimiseur **Adam**.
- **Taille du batch** : Utiliser une taille de batch de 32 ou 64.
- **Nombre d'époques** : Entraîner le modèle pendant 50 époques.
- **Augmentation des données** : Appliquer des techniques d'augmentation (rotation, flip, zoom).

### 4. Évaluation du modèle

- **Métriques** : Utiliser la précision, le rappel et le F1-score.
- **Matrice de confusion** : Générer une matrice de confusion pour visualiser les résultats.

### 5. Amélioration du modèle

- **Ajustement des hyperparamètres** : Modifier le taux d'apprentissage, la taille du batch, etc.
- **Augmentation des données** : Appliquer des transformations plus fortes.
- **Modèles plus complexes** : Tester des architectures plus avancées comme ResNet.



