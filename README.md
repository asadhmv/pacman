# pacman

**Objectif : Implémenter des algorithmes de recherche tel le Depth First Search et A* pour le jeu de 
Pacman afin qu’il atteigne l’objectif qui est la nourriture. Ensuite nous devrons comparer les résultats 
des deux algorithmes, ainsi trouver quel sera le meilleur pour le jeu.**

1. Depth First Search

L'algorithme commence par initialiser une pile avec l'état initial du problème et une liste vide 
d'actions. Il visite ensuite chaque état dans la pile en enlevant le dernier état ajouté, et 
explore ses successeurs. Pour chaque successeur, il vérifie s'il a déjà été visité. S'il ne l'a pas 
encore été, il l'ajoute à la pile avec la liste d'actions jusqu'à cet état. L'algorithme continue 
ainsi jusqu'à ce qu'il atteigne un état final ou que la pile soit vide.
La fonction renvoie le chemin le plus court de l'état initial à l'état final sous forme d'une liste 
d'actions (ou une liste vide si l'état final n'a pas été trouvé).
Big Maze 390
Medium Maze 146
Tiny Maze 15

2. A Star Search

Big Maze 549
Medium Maze 221
Tiny Maze 14
L'algorithme commence par initialiser une file de priorité avec l'état initial du problème et sa 
valeur heuristique. Il visite ensuite chaque état dans la file de priorité en enlevant l'état ayant 
le coût le plus faible, et explore ses successeurs. Pour chaque successeur, il calcule le coût 
actuel et l'ajoute à la file de priorité. L'algorithme continue jusqu'à ce qu'il atteigne un état 
final ou que la file de priorité soit vide.
La fonction renvoie le chemin le plus court de l'état initial à l'état final sous forme d'une liste 
d'actions (ou une liste vide si l'état final n'a pas été trouvé)


Conclusion :
L’algorithme de parcours en profondeur d'abord visite moins de nœud que le A* afin d’atteindre la 
nourriture, par exemple, pour le Big Maze le dfs visite 349 nœud et le A* en visite 549. On peut 
déduire que l’algorithme de parcours DFS est le plus adapté pour le jeu Pacman.
