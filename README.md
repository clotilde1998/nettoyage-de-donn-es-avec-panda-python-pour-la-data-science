# nettoyage-de-donn-es-avec-panda-python-pour-la-data-science

Objectifs

Le Data Cleaning (nettoyage de données) est l’étape la plus importante avant d’analyser ou modéliser des données mais elle peut être très fastidieuse.

Plaçons-nous dans le contexte, c’est le début d’un nouveau projet et vous êtes impatient d’appliquer certains modèles de Machine Learning. Vous examinez les données et vous réalisez rapidement que c’est la cata: les données ne sont absolument pas exploitables en l’état. Pour être tout à fait honnête, vous pouvez régulièrement vous attendre à consacrer jusqu’à 80% de votre temps à nettoyer les données.

Avant de commencer à nettoyer un dataset, il est judicieux d’avoir un aperçu des données. Après cela, vous pouvez élaborer le plan de nettoyage de données.

Il serait judicieux de se poser les questions suivantes: • Quelles sont les caractéristiques? • Quels sont les types attendus (int, float, string, boolean)? • Y a-t-il des valeurs manquantes évidentes (valeurs que la bibliothèque pandas peut détecter)? • Existe-t-il d’autres types de valeurs manquantes moins évidentes (impossible à détecter avec pandas)?

Dans cette pratique, nous allons parcourir un certain nombre de tâches de Data Cleaning à l’aide de la bibliothèque Pandas de Python. Ces traitements concernent des tâches telles que :

• Recherche et remplacement/suppression des valeurs manquantes • Renommage des colonnes • Suppression des colonnes inutiles à l’analyse • Suppression des duplications • Modification des types de données

Commencez par importer les données à partir du fichier source est nommé cleaning.csv dans une structure DataFrame.

Ensuite, nous chercherons à intégrer les pratiques de nettoyage suivantes.

Pratique 1 : Commencez par explorer l’ensemble des données : • Format • Type de données • Statistiques • Repérage des valeurs manquantes et dupliquées

Pratique 2 : Procédez par la suite à la modification des types de données que vous jugez pertinentes par rapport à la nature des données.

Pratique 3 : Repérez les valeurs manquantes dans l’ensemble des données. Comptabiliser ces valeurs manquantes par colonnes (pour juger si on procèdera à la suppression des colonnes où le nombre des valeurs manquantes est assez considérable). Procédez finalement à la suppression des valeurs manquantes par ligne et par colonne. Particulièrement pour la colonne 'Shape Reported', remplacer les valeurs manquantes par la valeur par défaut ‘VARIOUS’. Pratique 4 : repérer et supprimer les données dupliquées. Pratique 5 : Renommer les colonnes 'Shape Reported', 'Colors Reported' respectivement en ‘Forme’ et ‘Couleur’ Pratique 6 : réindexer les données selon l’ordre suivant : 'City', 'Forme', 'Couleur','State','Time'.
