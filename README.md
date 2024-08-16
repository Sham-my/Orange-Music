Dans le cadre d'un projet, j'ai réalisé deux types d'apprentissage à l'aide du logiciel Orange : un apprentissage supervisé et un autre non supervisé.

# Non supervisé 

Pour la partie non supervisée, j'ai sélectionné les 24 chansons les plus célèbres de Michael Jackson, que j'ai regroupées dans un fichier.
  
![/base de donnée non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/base%20de%20donn%C3%A9e%20non%20supervis%C3%A9.png)

  Une fois la base de données constituée, j'ai mis en place une chaîne de traitement intégrant l'outil "Distance" pour calculer une matrice de distances entre les chansons. J'ai ensuite utilisé "Hierarchical Clustering" en sortie pour observer un dendrogramme. Enfin, j'ai ajouté "Corpus Viewer" et "Word Cloud" en sortie de "Hierarchical Clustering" pour interpréter les résultats du dendrogramme.
  
![/chaine de traitement non supervisé](https://github.com/Sham-my/bookish-octo-giggle/blob/main/chaine%20de%20traitement%20non%20supervis%C3%A9%20.png)

Le dendrogramme généré par l’outil "Hierarchical Clustering" montre que les paroles des chansons sont réparties en trois groupes distincts :

![/classification non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/classification%20non%20supervis%C3%A9.png)

Dans le premier cluster on observe que les mots les plus fréquemment utilisé sont « love », « girl », « baby » et « remember ». Ce cluster représente les chansons d’amour de Michael Jackson.

![1er cluster non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/1er%20cluster%20non%20supervis%C3%A9.png)

Dans le deuxième cluster, le plus imposant les mots les plus utilisés sont « money », «alone», « stop », « pressurin ». Le thème mis en avant par ces mots est la pression du succès. 

![2eme cluster non supervisé .png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/2eme%20cluster%20non%20supervis%C3%A9%20.png)

Dans le dernier cluster le mot le plus utilisé est « bad ». Ce cluster encapsule les chansons parlant de malheur. Notamment le titre ‘bad’ qui parle de brigands et ‘They don’t care about us’ qui est un titre spécial qui aborde le thème de l’esclavage. 

![3eme cluster non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/3eme%20cluster%20non%20supervis%C3%A9.png)

# Supervisé 

Le jeu de donnée est un ensemble de variable qui décrit les genres musicaux. Obtenue sur le site kaggle. Vonstitué de 50 000 lignes et 18 colones comportant :

  1. 2 variables texte ( artist_name ; track_name) qui sont les auteurs et letitre des chansons ;
  2. 12 variables numériques caractérisant les genres musicaux ;
  3. 4 variables nominales dont celle à prédire(music_genre)

Je filtre mes données en retirant les variables qui n'apporte pas d'information. Suite à cela je réalise une chaine de traitement contenant plusieurs modèles d'apprentisage.

![chaine de traitement supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/chaine%20de%20traitement%20supervis%C3%A9.png)

Après analyse les matrices de confusions de chaque outil, les prédictions du Neural network semble être le meilleur et de loin comparé à d’autres comme celui de la régression logistique 

![confusion matrix neural network .png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/confusion%20matrix%20neural%20network%20.png)

Le jeu de données à prédire est constitué des dix premiers titres de chaque genre musical. On observe un taux de prédiction de 93,2 %.

 ![prediction.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/prediction.png)

Globalement, le modèle n’a aucun mal à bien prédire les musiques cependant je remarque qu'il confend le HIP-HOP avec le rap  ainsi que le Blue, Jazz et l'Alternative.
