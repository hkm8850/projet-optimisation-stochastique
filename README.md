<div align="center">
  <h1>Étude de méthodes d'optimisation stochastique</h1>

  <p>
    <a href="#"><img src="https://img.shields.io/badge/Python-3.8+-blue.svg" alt="Python" /></a>
    <a href="#"><img src="https://img.shields.io/badge/NumPy-Scientific%20Computing-013243.svg" alt="NumPy" /></a>
    <a href="#"><img src="https://img.shields.io/badge/Machine%20Learning-Optimization-FF6F00.svg" alt="ML" /></a>
    <a href="#"><img src="https://img.shields.io/badge/Matplotlib-Data%20Viz-11557c.svg" alt="Matplotlib" /></a>
  </p>
</div>

<br />

Ce dépôt documente un projet d'algorithmique mathématique et de *Machine Learning* axé sur l'implémentation de A à Z (from scratch) des principaux algorithmes abstraits de descente de gradient stochastique. 
L'objectif est d'étudier la mécanique de la convergence sur un problème complexe de perte logistique régularisée avec topologie mal conditionnée (forte anisotropie).

## 🎯 Périmètre Technique
- **Algorithmique** : Systématisation et comparaison des approches **SGD (Stochastic Gradient Descent)**, de l'inertie de **Momentum**, du gradient de **Nesterov**, et de l'optimiseur à taux adaptatif **Adam**.
- **Modélisation Appliquée** : Implémentation mathématique de la fonction Objectif (*Log-Loss* avec norme L2), de sa dérivée première (Jacobien) et de sa dérivée seconde (Matrice Hessienne) pour trouver un optimum parfait via la méthode de **Newton**.
- **Tuning d'Hyperparamètres** : Étude dynamique sur l'influence croisée et combinatoire du *Learning rate* dynamique et de la taille d'échantillonnage (*Batch Size*).

## 📂 Contenu 

```text
├── projet_opti.ipynb   # Laboratoire de recherche avec code source matriciel et graphiques
└── README.md           # Documentation
```

## 💡 Objectifs d'apprentissage démontrés
Ce travail permet de démystifier les "boîtes noires" de Scikit-Learn ou PyTorch, en codant soi-même les optimisations matricielles sous-jacentes. Il met en lumière pourquoi un espace topologique étiré cause de fortes oscillations à l'algorithme "Vanilla SGD", et prouve empiriquement l'ingéniosité des mécanismes de "mémoire" (Momentum) à accélérer la convergence $f(\theta^*)$.
