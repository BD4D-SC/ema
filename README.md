# EMA Cameroun - 2019
École Mathématique Africaine : bases mathématiques de l’intelligence artificielle  
Yaoudé - Cameroun - Juillet 2019 

# Cours/TP: Outils informatiques pour la science des données : Python
Ivan Keller, AXA Belgique

Ce cours, basé sur des exposés associés à des démonstrations et travaux pratiques, 
permettra aux étudiants d’apprendre à utiliser les outils Open Source de la science des données, 
et notamment l’éco-système autour du langage Python.  

Ce dépot contient :
- la présentation : `slides.pdf`
- les notebooks de cours numérotés de `1_` à `5_`
- les notebooks des TPs dans le répertoire `TPs/`
- les corrections des TPs dans le répertoire `TPs/solutions/`
- les fichiers des données utilisées dans les notebooks


## 0. Comment "cloner" ce dépot   
Pour obtenir les fichiers de ce dépot (_repository_) par exemple pour modifier les notebooks :  
    ![](img/repo.png)   
- Si vous n'avez pas `git` installé vous pouvez simplement : 
    1. téléchargez l'archive : cliquer sur le bouton vert "Clone or download" puis "Download ZIP" (flèches rouges) 
    2. décompresser l'archive à l'emplacement de votre choix (double-click sur le fichier .zip)
- Si vous avez `git` :
    1. cliquer sur le bouton vert "Clone or dowmload" et sur l'icône pour copier l'adresse du depot (flèches oranges)
    2. dans un terminal, à l'emplacement de votre choix, exécuter la commande :
    ```
    git clone <coller ici l'adresse du dépot>
    ```
    
Si vous souhaitez installer git :   
    - pour windows : https://gitforwindows.org/ et utiliser le shell `git bash`  
    - pour Mac et Linux : vous êtes assez débrouillard pour trouver :) (c'est facile).

## 1. Installation de Python
Il existe de nombreuses manière d'installer Python. Nous vous recommandons d'installer la distribution Anaconda :

### 1.1 Installation d'Anaconda  
1. Aller sur https://www.anaconda.com/distribution/  
2. Choisir l'instaleur selon votre OS (Windows, Mac ou Linux) et machine (64/32 bits) et choisir la version 3 (3.7 à ce jour).  
3. Suivre les instruction d'installation sur https://conda.io/projects/conda/en/latest/user-guide/install/index.html selon votre système.

Si vous ne bénéficiez pas d'une bonne connection internet vous pouvez installer la version légère de la distribution:  

### 1.2 Alternative: installation de Miniconda3  
1. Aller sur https://conda.io/en/latest/miniconda.html  
2. Télécharger l'installeur pour **Python 3.7** correspondant à votre machine et votre système (64-bit/32-bit et OS).  
3. Suivre les instruction d'installation sur https://conda.io/projects/conda/en/latest/user-guide/install/index.html selon votre système.  

En plus de Python 3, Anaconda et Miniconda installent l'utilitaire `conda` qui est un gestionnaire de paquets et d'environnements (_package and environment manager_) ainsi qu'un environnement de base.  

Si vous avez installé Miniconda, on commencera avec cet environnement de base puis on installera les modules nécessaires à mesure des besoins.

## 2. Exécuter du code Python
Il y a plusieurs manières d'intéragir avec Python:  
### 2.1. En session intéractive (python shell, console, REPL)
Dans un terminal, exécuter la commande **`python`** ou **`ipython`** et ensuite des commandes Python :

    $ python
    Python 3.7.1 (default, Dec 10 2018, 22:54:23) [MSC v.1915 64 bit (AMD64)] :: Anaconda, Inc. on win32
    Type "help", "copyright", "credits" or "license" for more information.
    >>> print('Hello EMA!')
    Hello EMA!
    >>>


### 2.2 En exécutant un script Python
On écrit du code à l'aide d'un éditeur de texte, par exemple le fichier `hello_ema.py` :  
    
    #!/usr/bin/python3 
    # hello_ema.py : ceci est un script élémentaire en Python 3

    print("Hello EMA!")
     
Puis on demande à l'interpréteur Python d'exécuter le script : 
    
    
    $ python hello_ema.py
    Hello EMA!
    
### 2.3. En mode intéractif dans un _notebook_ Jupyter 
Un notebook (carnet de notes) est une application web qui permet d'intéragir avec un langage de programmation, dont Python, et d'afficher le résultat de l'exécution de code ainsi que d'ajouter des notes textuelles enrichies (en Markdown comme dans le présent fichier). Tout se passe dans une page de votre navigateur web préféré.

Si vous avez Miniconda vous devez d'abord installer le module `jupyter` :   

    $ conda install jupyter
    
Puis lancer le serveur web de notebooks :     

    $ jupyter notebook

qui ouvrira une fenêtre dans le navigateur web :      
![Notebook example](img/notebook_ex1.png)   

## 3. Télécharger un fichier particulier de ce dépot  
Si vous avez installé Git il vous suffit de faire un `git pull` pour récupérer les nouveaux fichiers déposés depuis votre dernier pull.  
Sinon :
1. Sur le dépot, naviguer sur le fichier que vous voulez télécharger, par exemple `5_Scikit_Learn.ipynb` 
2. Cliquer sur le bouton "Raw" ![](img/git_raw.png) qui affiche le code source du fichier  
3. Sur votre navigateur choisir _Enregistrer sous ..._
4. Sauvegarder le fichier à la place voulue en faisant attention à l'extension du fichier (retirer l'extension `.txt` si elle a été ajoutée).



