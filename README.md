# Analyse des Données Mobiles - Prédiction de la Gamme de Prix

## Description du projet

Ce projet consiste en l'analyse de données mobiles afin de prédire la gamme de prix des téléphones mobiles en fonction de leurs caractéristiques techniques. L'objectif principal est de comprendre les relations entre diverses spécifications des téléphones (telles que la puissance de la batterie, la RAM, la taille de l'écran, etc.) et leur prix, en utilisant des techniques de régression, de réduction de dimensions, et d'analyse statistique.

## Objectifs

- **Évaluation de la multicolinéarité**: En utilisant des facteurs d'inflation de variance (VIF), nous avons évalué la multicollinéarité des variables, ce qui a permis de déterminer si certaines variables étaient fortement corrélées et pouvaient affecter la précision du modèle.
  
- **Hétéroscédasticité**: Le test de Breusch-Pagan a été effectué pour vérifier si les résidus du modèle suivaient une distribution homogène. Un p-value significatif a révélé une présence d'hétéroscédasticité, ce qui a permis d'affiner les modèles pour mieux gérer cette propriété.

- **Normalité des Résidus**: Le test de Shapiro-Wilk a été utilisé pour vérifier la normalité des résidus. Le test a montré que les résidus ne suivaient pas une distribution normale, ce qui a conduit à l'application de techniques pour améliorer l'adéquation du modèle.

- **Analyse en Composantes Principales (ACP)**: Une analyse PCA a été réalisée pour réduire la dimensionnalité des données tout en conservant la majeure partie de la variance. Des graphiques de type "Cercle des Corrélations" et "Projection des individus" ont été générés pour visualiser les relations entre les variables et les composantes principales.

- **Visualisation des Données**: Des graphiques tels que les boîtes à moustaches, les matrices de corrélation et les graphiques de dispersion ont été utilisés pour explorer et visualiser les données, identifier les relations et anomalies potentielles.

## Méthodologie

1. **Préparation des Données**: 
   - Sélection des caractéristiques les plus pertinentes pour le modèle.
   - Traitement des données manquantes et normalisation des variables.

2. **Modélisation**:
   - Mise en œuvre de la régression multiple pour prédire la gamme de prix des téléphones mobiles.
   - Réduction de la dimensionnalité avec l'ACP pour simplifier le modèle tout en maximisant la variance expliquée.
   - Évaluation de la performance des modèles à l’aide de différents critères statistiques et de tests d'hypothèses.

3. **Analyse des Résultats**:
   - Visualisation des résultats et évaluation de la qualité du modèle.
   - Ajustement des modèles selon les résultats des tests d'hétéroscédasticité et de normalité.

## Technologies utilisées

- **Python** (avec les bibliothèques : `Pandas`, `NumPy`, `Scikit-learn`, `Matplotlib`, `Seaborn`, `Statsmodels`)
- **Analyse des Composantes Principales (PCA)**
- **Régression linéaire et tests statistiques**

## Conclusion

Ce projet montre comment l'analyse exploratoire des données, la gestion de la multicollinéarité, et l'utilisation de l'ACP peuvent être des outils puissants pour la prédiction et la compréhension des relations entre les caractéristiques des téléphones mobiles et leur prix. La gestion de l'hétéroscédasticité et la normalisation des résidus sont également des éléments cruciaux pour la robustesse du modèle.
