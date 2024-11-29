# Épreuve finale - Automne 2022

## Directives Générales

Utilisez le répertoire **Depart** comme gabarit pour faire l'examen et répondre de votre
mieux aux questions suivantes. Une fois terminé ou si vous êtes bloqué, vous pouvez vous
référez à la version fonctionnelle du répertoire **Final**.

En partant du projet de base, vous allez créer une petite application qui va permettre de lancer un nombre de fois un type de dé aléatoirement. On va choisir entre 7 types de dés : d4, d6, d8, d10, d12, d20 et d100. Le nombre qui suit la lettre "d" indique le nombre de face du dé, donc pour un d8 par exemple on obtiendra des résultats de 1 à 8. On va ensuite pouvoir choisir le nombre de jets du dé sélectionné, un nombre de 1 à 10, à l'aide du "input" de type "range". Finalement en cliquant sur le bouton "Lancer", la génération aléatoire des jets va se faire et le résultat va s'afficher à l'écran.

Dans le fichier script.js il y a déjà une fonction **nombreAleatoire** qui prend en paramètre un nombre minimum et maximum. Cette fonction va générer un nombre aléatoire entre les deux paramètres qu'on lui passe et retournera ce nombre sous forme d'un entier.

## Question #1

Utilisez le fichier **VecnaBold.ttf** présent dans le répertoire **assets/font** dans votre page comme police par défaut pour tout le texte ainsi que pour le bouton **Lancer**.

Modifiez la balise **\<h1>** portant le id "titre" de la façon suivante : 

- Modifiez la couleur du tiret pour la variable **--couleur-bouton**.
- Modifiez la lettre "o" de roule par l'image **d0.png**. Ajustez la taille de l'image pour qu'elle soit "environ" de la même taille que le texte.

Exemple du résultat attendu

![exfinal_gr1_01](G:\Mon disque\cegep\2022-2023\cours\Design Web 420-1E6-VI\Examens\Epreuve finale\ressources\exfinal_01.png)

## Question #2

Utilisez css grid pour créer la disposition suivante. Les images sont toutes comprises dans la section avec le id **selection-des**: 

- Sur la première ligne on retrouve le d4 et le d6.
- Sur la deuxième ligne on retrouve le d8, le d20 et le d10.
- Sur la troisième ligne on retrouve le d12 et le d100.
- Les dimensions de chaque cellule de la grille doivent être de 1fr.
- La largeur et la hauteur de chaque image de dé doit être de 80 pixels.

Exemple du résultat attendu

![exfinal_05](G:\Mon disque\cegep\2022-2023\cours\Design Web 420-1E6-VI\Examens\Epreuve finale\ressources\exfinal_05.png)

## Question #3

À l'aide d'une requête media query, faites en sorte que lorsque la résolution de l'écran est sous 600 pixels, la disposition des dés change pour la suivante : 

![exfinal_02](G:\Mon disque\cegep\2022-2023\cours\Design Web 420-1E6-VI\Examens\Epreuve finale\ressources\exfinal_02.png)

## Question #4

Quand on survol un des dés, appliquez le même style que lors de sa sélection. Regardez les règles css utilisées pour la sélection et reproduisez les. La transition doit se faire pendant <u>150 millisecondes</u>.

![exfinal_03](G:\Mon disque\cegep\2022-2023\cours\Design Web 420-1E6-VI\Examens\Epreuve finale\ressources\exfinal_03.png)



## Question #5

Implémentez les jets de dés aléatoires quand on clique sur le bouton **Lancer**

- Le nombre de jets est déterminé par la valeur du input avec le id **choix-nombre-jet**
- Le type de dé à lancer est celui qui est sélectionné lors du clique sur le bouton.
- Le résultat sera inscrit dans un élément div qui sera créé par code. Il y a déjà une fonction **creerElementResultat** qui prend en paramètre un nombre qui représente le résultat et qui retourne un élément html à ajouter ensuite dans la section avec la classe **resultats**. On a déjà vu comment créer et ajouter un élément html à une page, en utilisant la fonction il ne vous restera qu'à l'ajouter.

![exfinal_04](G:\Mon disque\cegep\2022-2023\cours\Design Web 420-1E6-VI\Examens\Epreuve finale\ressources\exfinal_04.png)

## Question #6

- Quand on clique sur un des dés, changez le texte de l'élément avec la classe **texte-type-de** pour le type de dé sélectionné. (d4, d6, d8, etc...)
- Quand on modifie la valeur du input avec le id **choix-nombre-jet**, modifiez le texte de l'élément avec la classe **texte-nombre-jet** pour le nombre sélectionné. (1x, 2x, 3x, etc...). Vous pouvez utiliser l'événement "input".

Exemple du résultat attendu

![exfinal_06](G:\Mon disque\cegep\2022-2023\cours\Design Web 420-1E6-VI\Examens\Epreuve finale\ressources\exfinal_06.png)



## Grille de correction

| ÉlÉments                                                     |   Points |
| ------------------------------------------------------------ | -------: |
|                                                              |          |
| **Question #1**                                              |  **/10** |
| La police d'écriture de la page et du bouton a été modifiée comme demandé. |        5 |
| La couleur du caractère "-" du titre a été modifiée par la variable **--couleur-bouton**. |        3 |
| La marge du haut a été supprimée.                            |        2 |
|                                                              |          |
| **Question #2**                                              |  **/30** |
| Les images de dés sont disposés sur trois ligne selon ce qui est requis avec CSS Grid |       20 |
| La dimension de chaque cellule est de 1fr                    |        5 |
| Les images ont une dimension en largeur et en hauteur de 80 pixels |        5 |
|                                                              |          |
| **Question #3**                                              |  **/10** |
| Quand la résolution de l'écran est moins de 600 pixels, la disposition des images de dés change selon ce qui est demandé à l'aide d'une requète media query. |       10 |
|                                                              |          |
| **Question #4**                                              |  **/10** |
| La même animation css que lors de la sélection est déclenchée sur les images de dés lors de leur survol. |       10 |
|                                                              |          |
| **Question #5**                                              |  **/30** |
| Un nombre aléatoire est généré selon le type de dé choisi    |       10 |
| Un nombre aléatoire est généré un nombre de fois égale à la valeur indiquée dans le input **choix-nombre-jet** |       10 |
| Les résultats sont ajoutés un à un dans la section **resultats** |       10 |
|                                                              |          |
| **Question #6**                                              |  **/10** |
| Le texte du type de dé est modifié quand on clique sur un des images de dé. |        5 |
| Le texte du nombre de jets à faire est modifié quand on change la valeur du input **choix-nombre-jet** |        5 |
|                                                              |          |
| **Total**                                                    | **/100** |

  

  





