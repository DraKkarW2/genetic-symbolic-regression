# genetic-symbolic-regression

## Description

Implémentation from-scratch de la régression symbolique par programmation génétique.

Ce projet consiste à faire évoluer des expressions mathématiques représentées sous forme d’arbres afin d’approximer une fonction cible à partir de données. L’algorithme utilise des mécanismes inspirés de l’évolution biologique : sélection, croisement (crossover), mutation et élitisme.

L’objectif est de découvrir automatiquement des formules mathématiques interprétables à partir de données, plutôt que d’utiliser des modèles de type boîte noire.

---

## Principe général

Chaque expression est représentée sous forme d’un **arbre d’opérations mathématiques** :

- Nœuds internes : opérations (+, ×, sin, cos)
- Feuilles : variable (x) ou constantes

Ces arbres sont ensuite optimisés au fil des générations pour minimiser une fonction de coût.

---

## Fonction objectif

L’algorithme optimise une fonction combinant :

- L’erreur quadratique moyenne (MSE)
- Une pénalité de complexité de l’arbre

Cela permet de favoriser des solutions à la fois **précises et interprétables**.

---

## Algorithme génétique

Chaque génération suit les étapes suivantes :

1. Évaluation de la population
2. Sélection des meilleurs individus
3. Croisement (crossover)
4. Mutation
5. Ajout de diversité (arbres aléatoires)
6. Remplacement de la population

---

## Résultats

Le modèle est capable de retrouver des expressions proches de fonctions connues, par exemple :

\[
x^2 + \sin(x)
\]

Ce résultat montre que la régression symbolique permet de :
- reconstruire des fonctions mathématiques à partir de données
- obtenir des expressions interprétables

---

## Exemple de convergence

On observe généralement une diminution progressive de la perte au fil des générations, ce qui indique une amélioration des solutions candidates.

---

## Technologies utilisées

- Python 
- NumPy
- Matplotlib
- IPython (affichage LaTeX)

---

## Objectif du projet

Ce projet a été réalisé dans un but d’apprentissage afin de comprendre :

- les algorithmes génétiques
- la régression symbolique
- la représentation d’expressions sous forme d’arbres
- les méthodes d’optimisation évolutive

---

## Améliorations possibles

- simplification symbolique automatique des arbres
- optimisation des opérateurs de mutation
- ajout de nouvelles fonctions (exp, log, tan…)
- parallélisation de l’évaluation
- visualisation de l’évolution des arbres

---

## Auteur

Projet personnel d’exploration en intelligence artificielle et machine learning.
