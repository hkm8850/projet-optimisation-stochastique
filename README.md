# Étude de méthodes d'optimisation stochastique

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243.svg)

Ce projet est une implémentation "from scratch" en Python des principaux algorithmes de descente de gradient stochastique utilisés en Machine Learning. L'objectif était de comprendre mathématiquement ce qui se passe sous le capot des librairies classiques (comme Scikit-Learn ou PyTorch) en codant moi-même les algorithmes.

## 🎯 Ce que j'ai fait dans ce projet

Sur un problème de régression logistique régularisée (norme L2), j'ai codé et comparé :
- **SGD** (Stochastic Gradient Descent)
- **Momentum**
- **Nesterov**
- **Adam**

J'ai également implémenté la **Méthode de Newton** (en calculant le Hessien exact) afin de trouver l'optimum parfait de référence $f(\theta^*)$.

## 💡 Résultats et apprentissages
- J'ai généré un dataset volontairement étiré (anisotropique) pour "piéger" les algorithmes.
- J'ai fait varier les hyperparamètres (Learning Rate et Batch Size) pour observer leur impact direct sur la courbe de convergence.
- J'ai pu constater visuellement que l'algorithme SGD classique souffre d'énormes oscillations sur des données asymétriques, et que l'introduction d'un mécanisme de "mémoire" (Momentum) ou de taux adaptatif (Adam) résout ce problème de vitesse.

## 📂 Contenu 
- `stochastic_optimization.ipynb` : Le notebook contenant toutes les matrices, les fonctions de perte, le calcul des gradients et les graphiques de performance.
