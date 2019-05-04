# EMA Cameroun - 2019
Material for EMA Summer School - Yaoudé - Cameroun - July 2019    

Cours : Outils Informatiques pour la science des données : Python

## Installation de Python
Il existe de nombreuses manière d'installer Python. Nous vous recommandons d'installer la distribution Miniconda :  

### Installation de Miniconda3  
1. Aller sur https://conda.io/en/latest/miniconda.html  
2. Télécharger l'installeur pour **Python 3.7** correspondant à votre machine et votre système (64-bit/32-bit et OS).  
3. Suivre les instruction d'installation sur https://conda.io/projects/conda/en/latest/user-guide/install/index.html selon votre système.  

En plus de Python 3, Miniconda installe l'utilitaire `conda` qui est un gestionnaire de paquets et d'environnements (_package and environment manager_) ainsi qu'un environnement de base.  

On commencera avec cet environnement de base puis on installera les modules nécessaires à mesure des besoins.

## Exécuter du code Python
Il y a plusieurs manières d'intéragir avec Python:  
1. En session intéractive : dans un terminal, exécuter la commande **`python`** ou **`ipython`** et ensuite des commandes Python :
    ```
    $ python
    Python 3.7.1 (default, Dec 10 2018, 22:54:23) [MSC v.1915 64 bit (AMD64)] :: Anaconda, Inc. on win32
    Type "help", "copyright", "credits" or "license" for more information.
    >>> print('Hello EMA!')
    Hello EMA!
    >>>
    ```

2. En écrivant du code Python dans un éditeur de texte, par exemple :  
    ```
    # hello_ema.py : un script élémentaire en Python 3

    print("Hello EMA!")
    ```   
    et en demandant à l'interpréteur Python d'exécuter le script : 
    ```
    $ python hello_ema.py
    Hello EMA!
    ```  
3. En mode intéractif dans un _notebook_ (carnet de notes) Jupyter. Un notebook est une application web (un programme avec lequel on intéragit avec un navigateur web) qui permet d'intéragir avec un langage de programmation, dont Python, et d'afficher le résultat de l'exécution de code ainsi que d'ajouter des notes textuelles enrichies (en Markdown comme dans le présent fichier).

    Nous devons d'abord installer le module Jupyter:
    ```
    $ conda install jupyter
    ```
    Puis lancer le serveur web de notebooks qui ouvrira une fenêtre dans le navigateur web :  
    ```
    $ jupyter notebook
    ```

Dans ce cours nous utiliserons principalement des notebooks.
