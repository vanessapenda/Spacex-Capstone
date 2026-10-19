# Prédire l'atterrissage du premier étage du Falcon 9 de SpaceX

Projet Capstone du **IBM Data Science Professional Certificate**.

SpaceX propose des lancements Falcon 9 à environ 62 millions de dollars, contre plus de 165 millions chez ses concurrents, car le premier étage est réutilisé. L'objectif est de prédire si le premier étage va atterrir avec succès, afin d'estimer le coût d'un lancement.

## Contenu du dépôt

| Étape | Fichier |
|---|---|
| 1. Collecte des données — API SpaceX | [jupyter-labs-spacex-data-collection-api.ipynb](jupyter-labs-spacex-data-collection-api.ipynb) |
| 2. Collecte des données — Web scraping Wikipedia | [jupyter-labs-webscraping.ipynb](jupyter-labs-webscraping.ipynb) |
| 3. Préparation des données (data wrangling) | [labs-jupyter-spacex-data-wrangling.ipynb](labs-jupyter-spacex-data-wrangling.ipynb) |
| 4. EDA avec SQL | [jupyter-labs-eda-sql-coursera_sqllite.ipynb](jupyter-labs-eda-sql-coursera_sqllite.ipynb) |
| 5. EDA avec visualisation | [edadataviz.ipynb](edadataviz.ipynb) |
| 6. Carte interactive Folium | [lab_jupyter_launch_site_location.ipynb](lab_jupyter_launch_site_location.ipynb) |
| 7. Dashboard Plotly Dash | [spacex-dash-app.py](spacex-dash-app.py) |
| 8. Analyse prédictive (Machine Learning) | [SpaceX_Machine_Learning_Prediction_Part_5.ipynb](SpaceX_Machine_Learning_Prediction_Part_5.ipynb) |
| Présentation finale | [Rapport_Capstone_SpaceX.pdf](Rapport_Capstone_SpaceX.pdf) |

Les captures d'écran (fichiers .png) et les cartes Folium interactives (fichiers .html) sont à la racine du dépôt.

## Résultats clés

- Taux d'atterrissage réussi global : **66,7 %** (90 vols Falcon 9). Il passe de 0 % (2010-2013) à 90 % (2019).
- Meilleur site : **KSC LC-39A** avec 76,9 % de succès.
- Orbites ES-L1, GEO, HEO, SSO : 100 % de succès ; GTO : 52 %.
- Modèles testés : régression logistique, SVM, arbre de décision, KNN (GridSearchCV, cv = 10).
- Meilleur modèle : **arbre de décision**, 86,3 % en validation croisée et 83,3 % sur le jeu de test.

## Outils

Python, Pandas, NumPy, Requests, BeautifulSoup, SQLite, Matplotlib, Seaborn, Folium, Plotly Dash, scikit-learn.
