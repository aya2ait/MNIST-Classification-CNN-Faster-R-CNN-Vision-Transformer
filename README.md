# MNIST-Classification-CNN-Faster-R-CNN-Vision-Transformer
Ce projet explore différentes architectures de classification d'images sur le jeu de données MNIST
Voici une version épurée et professionnelle de votre README sans extraits de code :

# MNIST Classification Benchmark

## Présentation du Projet
- **CNN Classique** : Architecture de référence pour la vision par ordinateur
- **Faster R-CNN Adapté** : Version simplifiée du modèle de détection d'objets
- **Vision Transformer** : Approche innovante basée sur l'attention

## Résultats Principaux

### Performances Globales

| Architecture       | Accuracy | Temps d'Entraînement | Paramètres | Mémoire GPU |
|--------------------|----------|----------------------|------------|-------------|
| CNN                | 99.20%   | 53s                  | 0.42M      | 1.2GB       |
| Faster R-CNN       | 99.16%   | 180s                 | 1.1M       | 2.5GB       |
| Vision Transformer | 95.54%   | 134s                 | 0.04M      | 1.8GB       |
| VGG16 (fine-tuned) | 99.63%   | 1778s                | 138M       | 4.3GB       |

## Analyse Comparative

### CNN Traditionnel
- **Avantages** :
  - Rapidité d'entraînement optimale
  - Architecture simple et efficace
  - Faible consommation mémoire
- **Limitations** :
  - Performance plafonnée sur tâches complexes

### Faster R-CNN Adapté
- **Points Forts** :
  - Performance comparable au CNN
  - Architecture adaptable
- **Contraintes** : 
  - Surdimensionné pour MNIST
  - Consommation mémoire élevée

### Vision Transformer
- **Innovations** :
  - Approche basée sur l'attention
  - Nombre de paramètres très réduit
- **Défis** :
  - Courbe d'apprentissage plus lente
  - Accuracy légèrement inférieure

## Configuration Technique

### Environnement Recommandé
- **Matériel** : GPU  ≥8GB mémoire
- **Logiciels** :
  - Python 3.8+
  - PyTorch 1.12+
  - CUDA 11.3 (si GPU )

### Méthodologie
1. **Prétraitement** : Normalisation des images (28×28 pixels)
2. **Entraînement** :
   - 10 epochs pour les modèles custom
   - Fine-tuning sur 3 epochs pour VGG16/AlexNet
3. **Évaluation** : 
   - Jeu de test standard MNIST
   - Métriques : Accuracy, F1-Score, temps d'inférence

## Conclusions

1. **Pour MNIST**, le CNN reste l'architecture de référence
2. **Faster R-CNN** montre ses limites pour la classification simple
3. **ViT** présente un potentiel intéressant malgré sa performance légèrement inférieure
4. **Le transfer learning** (VGG16) offre des gains marginaux à coût élevé



