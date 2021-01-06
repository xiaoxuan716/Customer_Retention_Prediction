# Customer_Retention_Prediction
Pour cette étude, la base de données d’origine contient 50,000 observations, et ils existent des données manquantes. Il est nécessaire de faire une imputation, car la méthode des réseaux de neurones ignore toutes observations possédant une valeur manquante, ce qui peut nuire aux résultats du modèle si celles-ci ne sont pas imputées au préalable. Pour la méthode des arbres de classification, elle ne nécessite pas obligatoirement que le jeu de données soit imputé, s’il y a des valeurs manquantes. Mais, le jeu de données avec imputation a un taux de mauvaise classification moins élevé, donc on va imputer pour la méthode des arbres aussi. Ici, on va utiliser le nœud « Imputation » pour remplacer les données par la méthode « tree surrogate ». Cela permet d’imputer les valeurs manquantes et à la fois de préserver la corrélation avec d'autres variables.  Avec le nœud « Data Partition », les données sont divisées en données d’apprentissage (60%) et données de validation (40%). La séparation sert principalement à faciliter la détection de la précision du modèle de prédiction. Ainsi, pour cette étude, la variable cible (le rôle « Target ») sera « churn », avec le type « binaire » (1=les clients qui ont quitté, 0=les fidèles clients). Les variables explicatives seront les variables de comportement, l’interaction avec la compagnie et des données démographiques (environ 180 variables explicatives).

## 
Modèle : Arbre de classification
##
Modèle : La méthode d’ensemble 
##
         Gradient boosting; Forêt aléatoire
##
Modèle : Réseaux de neurones
##
Seront utilisés

##
Conclusion
En se basant sur les résultats obtenus pour chaque technique de prévision (arbre, méthode d’ensemble et réseaux de neurones), il semble clair que la méthode d’ensemble (le gradient boosting) performe mieux. Le taux de bonne classification avec le gradient boosting comparé aux autres techniques est beaucoup plus élevé. De plus, en prenant compte de la sensibilité ainsi que la spécificité, le modèle du gradient boosting performe bien aussi. Voici un tableau des meilleurs modèles pour chaque méthode étudiée :
Méthode de prévision	Taux de mauvaise classification
Arbre	0.3734
Méthode d’ensemble (Gradient-boosting)	0.3598
Réseaux de neurones	0.3889
En terminant, chaque méthode (les arbres, les forets aléatoires, les gradient boosting et les réseaux de neurones) possède ses avantages et désavantages pour faire la prédiction. Il est important de bien connaitre les subtilités des données. Pour cette étude, la méthode du gradient boosting semble offrir de meilleurs résultats.



