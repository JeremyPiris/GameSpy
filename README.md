# GameSpy
Projet fil rouge de ma formation data analyst chez DataScientest

Ce projet a été fait en collaboration avec 2 autres étudiants de ma promo, entre septembre 2021 et avril 2022.

** Détail du projet **

À partir d'un dataset recensant différentes informations sur des jeux vidéos (https://www.kaggle.com/gregorut/videogamesales), l'objectif de ce projet était de prédire leurs ventes.

- Etape 1 : webscraping pour enrichir le dataset de départ (BeautifulSoup, googlesearch, Selenium)
- Etape 2 : visualisation d'hypothèses explicatives de certaines variables sur le nombre de jeux vendus (matplotlib, seaborn)
- Etape 3 : enrichissement du dataset par transformation de certaines variables en moyennes mobiles
- Etape 4 : pré-processing (gestion des NaN, transformation des variables catégorielles en variables numériques, split du dataset en train et test) et entraînement de modèles de régression et de classification pour prédire ces ventes (scikit-learn)


** Résultats du projet **

Le nombre de ventes à prédire est à la base une valeur continue. 
Notre premier réflexe a donc été de tester des modèles de machine learning de régression. Mais les résultats ont été assez mauvais, quelques soient les modèles utilisés.

On s'est alors tourné vers des modèles de classification en transformant notre variable cible en classes de ventes.
Les résultats ont alors été beaucoup plus concluants : 
73% de bonnes prédictions sur un modèle à 4 classes de ventes et 
67% sur un modèle à 6 classes.