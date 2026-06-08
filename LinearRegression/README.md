# 📊 Confrontation des Résultats de Régression Linéaire

Ce dépôt regroupe et compare les métriques de performance obtenues avec un modèle de **Régression Linéaire** (`LinearRegression`) sur deux jeux de données distinctes.

## 📈 Tableau Comparatif des Performances

Les modèles ont été entraînés et évalués avec la même méthodologie (découpage **80% Entraînement / 20% Test**). Voici la confrontation directe des métriques obtenues sur l'ensemble de test :

| Métrique Évaluée | 🏠 Dataset California Housing | 🩸 Dataset Diabetes |
| :--- | :--- | :--- |
| **Coefficient $R^2$ (Score)** | **0.58** (58%) | **0.48** (48%) |
| **RMSE (Erreur Concrète)** | **0.75** (soit ~75 000 $) | **53.12** points |
| **MSE (Erreur Quadratique)** | **0.56** | **2821.75** |

---

## 🔍 Analyse des Résultats en 2 Lignes

* **California Housing ($R^2 = 0.58$) :** Le modèle linéaire est plus performant sur ce dataset car les facteurs économiques (comme le revenu moyen d'un quartier) ont une relation très directe et proportionnelle avec le prix des logements.
* **Diabetes ($R^2 = 0.48$) :** Le score est plus faible car la progression d'une maladie biologique est un phénomène complexe et courbe (non linéaire), qui dépend également de facteurs absents du dataset (alimentation, génétique).
