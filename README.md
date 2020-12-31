# <center> Projet_AnalyseNumerique</center>
## Intégration Numérique :
## Table des matières :

- [À propos du projet:](#heading)
  * [Utilité](#sub-heading)
  * [Outil de développement]
- [Documentation sur IntegrationProject.py:](#heading-1)
  * [Documentation de la classe Rectangle]
  * [Documentation de la classe mclass]
  * [Méthodes de la classe mclass:](#sub-heading-1)



     


## À propos du projet:
Ce petit projet consiste à modéliser quatres méthodes d'intégration numériques avec une interface graphique réalisé à l’aide du « Tkinter ». 
Cette dernière vous permet de saisir la fonction, puis choisir les bornes d'intégrale (a et b) et fixer le nombre de subdivisons. Finalement, appuyer:
* Soit sur le bouton _**"plot"**_ : pour afficher le graphe de la méthode désirée, sa valeur d’intégrale et son erreur.
* Soit sur le bouton _**"plotAll"**_: pour afficher les quatre graphes relié à chaque méthode d’intégration l’intégrité des valeurs approchées des méthodes et leurs erreurs(qui représente la différence entre  la valeur exacte de l’intégrale et la valeur approchée donné par chaque méthode) 

Les méthodes d’intégrations étudiées dans ce projet : 

1. Méthode des Rectangles Gauches

2. Méthode des Trapèzes

3. Méthode des Points Milieux

4. Méthode de Simpson

#### Voici un démo sur la réalisation de l’interface graphique :

![](gif1.gif)

### Utilité:
L’intégration est un des problémes les plus importants que l’on rencontre en analyse. En effet, on rencontre souvent des intégrales dont le calcul par des méthodes analytiques est trés compliqué ou même impossible, car il n’existe pas d’expression analytique d’une primitive de la fonctionà intégrer.
Dans ces cas, on peut appliquer des méthodes numériques qui permettent de calculer rapidement une valeur approchée I de l’intégrale à calculer. Cette petite application facilite cette tâche de calcul et même de comparaison entre les méthodes d'integrations prise en considération (méthode des rectangles à gauche, méthode des trapèzes, méthode des points milieux et la méthode de simpson)


### Outil de développement:
Le langage Python 3 a été utilisé pour coder les différentes méthodes. Les bibliothèques utilisées sont principalement numpy et matplotlib et certaines parties du code nécessitent pylab.

Le projet est constitué des fichiers suivants:
* _**"IntegrationProject.py"**_ : contient le code source du projet.
* _**"Project.gif"**_  : contient un démo sur le projet.
* _**"Rapport.pdf"**_  : Vous pouvez consulter le rapport détaillé sur le projet et sur les parties théroqies des quatres méthodes d'intégration.

## Documentation sur IntegrationProject.py:
Ce fichier contient 5 classes (class Rectangle,class Trapezoidal,class Simpson,class Milieu,class mclass) 
### Documentation de la classe Rectangle
Cette classe permet la modélisation d’intégration par la méthodes des Rectangles Gauches.
* Le constructeur de la classe se fait avec la fonction à intégrer, les valeurs des bornes d’intégrale et le nombre de subdivision en argument.
* Avant toutes autres étapes d’affichage, il faut calculer dans la classe rectangle la valeur d’intégrale. Pour cela, il y a la méthodes _**integrate**_. Cette dernière va être appelé dans la méthode _**Graph**_ qui est la méthode "de base" pour l’affichage.
* _**La méthode integrate**_ fait le calcul de la valeur d’intégrale  
* _**La méthode  Graph**_ trace la fonction à intégrer sur les points donnés en argument et retourne l'erreur et la valeur approchée d’intégrale de cette méthode.
### Déclaration des attributs :Fonctionnement de la classe Rectangle
* f : la fonction à intégrer, déterminée par le constructeur et modifiable
* a : Borne inférieur d’intégrale (modifiable )
* b : Borne supérieur d’intégrale ( modifiable)
* n : nombre de subdivisions ( modifiable)
### Remarques:
Ces méthodes sont pareils pour class Trapezoidal,class Simpson et class Milieu

### Documentation de la classe mclass :
C'est la classe qui initialise tout les éléments de la fenêtre
L'interface du projet contient trois cadres (frames) pour la composition de la fenêtre:
 * **frame1:** dédié à la saisie des champs telle que la fonction f à intégrer , les valeurs du bornes (a et b) et le nombre de subdivisions (n) et aux bouttons _**Plot**_ , _**PlotAll**_ , _**Reset**_ et _**Quit**_
 * **frame2:** dédié à l'affichage de(s) graphe(s).
 * **frame3:** dédié à l'affichage des valeurs approchées d'intégrale et l'erreur.
 ### Méthodes de la classe mclass:
* Méthode init : pour l'initialisation de la fenêtre , des frames , les labels, des boxes et des bouttons .
* Méthode plot : pour l'affichage d'une seule graphe.En effet,le Combobox inséré dans l'interface vous permet de choisir la méthode d'intégration désiré , il suffit de choisir la méthode , le graphe va être affiché , ainsi la valeur approchée de l'intégral et l'erreur.
* Méthode plotall: C'est le même principe de la méthode plot sauf celle-ci permet l'affichage des quatre ghraphes de chaque méthode simultanément ainsi leurs valeurs approchées  et leurs erreurs.

## Execution :
Le fichier peut également être exécuté sous forme de script :











