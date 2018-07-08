# Ensembles de sommes spéciaux : Meta-Testing
`Difficulté : Difficile (50%)`
`Origine : Projet Euler n°106`

Notons S(A) la somme des éléments d'un ensemble A de taille n. On dira que A est un ensemble de sommes spécial si pour tous ensembles disjoints B et C, on a les deux propriétés suivantes qui sont vérifiées :

    S(B) ≠ S(C) : c'est à dire que les sommes de sous ensembles sont toutes différentes
    Si B contient plus d'éléments que C alors S(B) > S(C)

Pour ce problème on va supposer que les ensembles contiennent n éléments formant une suite strictement croissante et qu'il vérifient déjà la deuxième règle.

De manière surprenante, parmi les 25 paires de sous-ensembles qu'on peut former à partir d'un ensemble à 4 éléments, seulement une de ces paires a besoin d'être testée pour vérifier la première règle. De la même manière, pour n=7, seule 70 des 966 paires de sous-ensembles ont besoin d'être testées.

Pour n=12, combien des 261625 paires de sous-ensembles qu'on peut obtenir ont elles besoin d'être testées pour vérifier la première règle ?

Note : Ce problème est en relation avec le problème 103 et 105.

On affichera le résultat avec `print`.

@[Ensembles de sommes spéciaux : Meta-Testing]({"stubs": ["Defis/Euler_106.py"], "command": "python3 Defis/Euler_106_Test.py"})

---

# Réseau minimal
`Difficulté : Moyen (35%)`
`Origine : Projet Euler n°107`

Le réseau non orienté suivant est composé de 7 sommets and 12 arêtes avec un poids total de 243. 

![reseau](https://projecteuler.net/project/images/p107_1.gif)

Ce réseau peut être représenté par le tableau suivant :

 | A | B | C | D | E | F | G   
 -- | -- | -- | -- | -- | -- | -- | --  
A | - | 16 | 12 | 21 | - | - | -   
B | 16 | - | -  | 17 | 20 | - | -  
C | 12 | - | - | 28 | - | 31 | -  
D | 21 | 17 | 28 | - | 18 | 19 | 23  
E | - | 20 | - | 18 | - | - | 11  
F | - | - | 31 | 19 | - | - | 27  
G | - | - | - | 23 | 11 | 27 | -  

Cependant, il est possible d'optimiser le reseau en retirant des arêtes et toujours assurer que chaque points du réseau reste connecté. Le réseau qui réussit le maximum d'économie est montré ci-dessous. Il a un poids de 93, représentant une économie de 243 − 93 = 150 par rapport au réseau d'origine.

![Matrice minimale](https://projecteuler.net/project/images/p107_2.gif)

En utilisant la matrice donnée ci-dessous,  correspondant à un réseau de 40 sommets, trouver l'économie maximum qui peut être réalisée en retirant des arêtes du réseau mais en assurant que tous les sommets restent connectés entre eux.

On affichera le résultat avec `print`.

@[Minimal network]({"stubs": ["Defis/Euler_107.py"], "command": "python3 Defis/Euler_107_Test.py"})

---