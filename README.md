# Statistiques et Machine Learning : Concepts Essentiels

## 1. Statistiques de Base

### **Mean (Moyenne)**
La moyenne est la somme de toutes les valeurs divisée par le nombre total de valeurs.  
**Formule :**  
\[
\text{Mean} = \frac{\sum_{i=1}^n x_i}{n}
\]
- **Utilité :** Représente la tendance centrale d’un ensemble de données.

---

### **Standard Deviation (Écart-Type)**
L'écart-type mesure la dispersion des données par rapport à la moyenne.  
**Formule :**  
\[
\text{Std} = \sqrt{\frac{\sum_{i=1}^n (x_i - \text{Mean})^2}{n}}
\]
- **Interprétation :**
  - Une petite valeur indique que les données sont proches de la moyenne.
  - Une grande valeur indique une forte dispersion.

---

### **Quartiles (25%, 50%, 75%)**
Les quartiles divisent les données en quatre parties égales :
- **25% (Q1)** : 25% des données sont en dessous de cette valeur.
- **50% (Q2, médiane)** : La valeur au centre des données.
- **75% (Q3)** : 75% des données sont en dessous de cette valeur.

**Importance :** Les quartiles aident à comprendre la distribution et à détecter les valeurs aberrantes.

---

## 2. Machine Learning

### **Logistic Regression**
- **Principe :** La régression logistique est un algorithme de classification qui prédit la probabilité qu’un point de données appartienne à une classe.  
  **Formule :**  
  \[
  \sigma(z) = \frac{1}{1 + e^{-z}}, \quad \text{où } z = w^T x + b
  \]
  - \( \sigma(z) \) : Fonction sigmoïde transformant \( z \) en probabilité.
  - \( w, b \) : Coefficients appris pendant l’entraînement.

- **Différence avec la Régression Linéaire :**
  - La **régression linéaire** prédit une valeur continue (\( y \)).
  - La **régression logistique** prédit une probabilité (valeur entre 0 et 1) pour classifier les données.

---

### **Importance de la Normalisation des Données**
- **Pourquoi normaliser ?**
  - Les algorithmes (comme la régression logistique) sont sensibles à l’échelle des données.
  - Normaliser les données (par exemple, centrer et réduire) permet une convergence plus rapide et évite les biais dus à des échelles différentes.

---

### **One-vs-All Method (OvA)**
- **Définition :**
  - Technique utilisée pour étendre des algorithmes binaires (comme la régression logistique) à des tâches de classification multi-classes.
  - On entraîne un modèle pour chaque classe, en considérant cette classe comme positive et toutes les autres comme négatives.
- **Exemple :**
  Pour classifier en 3 classes (\(A, B, C\)), on entraîne trois modèles :
  - Modèle 1 : Classe \(A\) vs \(B\) et \(C\)
  - Modèle 2 : Classe \(B\) vs \(A\) et \(C\)
  - Modèle 3 : Classe \(C\) vs \(A\) et \(B\)

---

Ce résumé couvre les bases nécessaires pour comprendre ces concepts de manière claire et concise.
