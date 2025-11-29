# Starbucks Numpy Project

Atelier Numpy sur les boissons Starbucks (portion 12 oz).

## Objectifs

- Importer le fichier `starbucks-menu-nutrition-drinks.csv` avec `np.genfromtxt`.
- Nettoyer les données :
  - gérer les valeurs manquantes (`-` → `NaN`),
  - séparer :
    - `header` : noms de colonnes,
    - `drinks` : noms des boissons,
    - `data` : données numériques (Calories, Fat, Carb, Fiber, Protein, Sodium),
  - filtrer les boissons sans aucune valeur numérique.

## Analyses réalisées

- Moyenne des calories par boisson.
- Médiane des protéines.
- Minimum et maximum de lipides (Fat).
- Identification de la boisson la plus calorique et de la moins calorique.

## Data modeling – NutriScore maison

Création d’un **niveau de calories** pour chaque boisson :

- 0–100 calories → niveau 1  
- 100–200 calories → niveau 2  
- 200–300 calories → niveau 3  
- 300+ calories → niveau 4  

Utilisation de `numpy` pour :

- créer un vecteur `niveaux_calories`,
- appliquer des masques logiques pour attribuer les niveaux,
- filtrer les boissons **NutriScore 1** (les moins caloriques) et calculer leur moyenne de calories.

## Stack

- Python
- Numpy
- Jupyter Notebook
