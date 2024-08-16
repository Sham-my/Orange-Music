Dans le cadre d'un projet, j'ai réalisé deux types d'apprentissage à l'aide du logiciel Orange : un apprentissage supervisé et un autre non supervisé.

# Non supervisé 

Pour la partie non supervisée, j'ai sélectionné les 24 chansons les plus célèbres de Michael Jackson, que j'ai regroupées dans un fichier.
  
![/base de donnée non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/base%20de%20donn%C3%A9e%20non%20supervis%C3%A9.png)

  Une fois la base de données constituée, j'ai mis en place une chaîne de traitement intégrant l'outil "Distance" pour calculer une matrice de distances entre les chansons. J'ai ensuite utilisé "Hierarchical Clustering" en sortie pour observer un dendrogramme. Enfin, j'ai ajouté "Corpus Viewer" et "Word Cloud" en sortie de "Hierarchical Clustering" pour interpréter les résultats du dendrogramme.
  
![/chaine de traitement non supervisé](https://github.com/Sham-my/bookish-octo-giggle/blob/main/chaine%20de%20traitement%20non%20supervis%C3%A9%20.png)

Le dendrogramme généré par l’outil "Hierarchical Clustering" montre que les paroles des chansons sont réparties en trois groupes distincts :

![/classification non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/classification%20non%20supervis%C3%A9.png)

Dans le premier cluster on observe que les mots les plus fréquemment u lisé sont « love », « girl », « baby » et « remember ». Ce cluster représente les chansons d’amour de Michael Jackson.

![1er cluster non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/1er%20cluster%20non%20supervis%C3%A9.png)

Dans le deuxième cluster, le plus imposant les mots les plus u lisés sont « money », «alone», « stop », « pressurin ». Le thème mis en avant par ces mots est la pression du succès. 

![2eme cluster non supervisé .png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/2eme%20cluster%20non%20supervis%C3%A9%20.png)

Dans le dernier cluster le mot le plus u lisé est « bad ». Ce cluster encapsule les chansons parlant de malheur. Notamment le tre ‘bad’ qui parle de brigands et ‘They don’t care about us’ qui est un tre spécial qui aborde le thème de l’esclavage. 

![3eme cluster non supervisé.png](https://github.com/Sham-my/bookish-octo-giggle/blob/main/3eme%20cluster%20non%20supervis%C3%A9.png)

# Supervisé 
