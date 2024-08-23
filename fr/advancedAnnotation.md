## Tree types

Dans ArboratorGrew, les arbres sont organisés en différentes catégories, notamment :

- **"Vos Arbres"** : Les arbres sur lesquels vous avez travaillé.
- **"Les Arbres les Plus Récents"** : Le dernier arbre annoté de toutes les phrases.
- **"Vos Arbres Récents Remplis avec les Arbres les Plus Récents"** : Une combinaison de vos arbres récents et des arbres les plus récents ajoutés.
- **"Tous les Arbres"** : Une collection inclusive de tous les arbres disponibles.
- **"Arbres Validés"** : Les arbres qui ont été examinés et approuvés par un validateur.
- **"Arbres en Attente"** : Les arbres associés à des phrases qui n'ont pas d'arbres validés.

Ces types d'arbres seront utilisés dans les fonctionnalités suivantes.
## Grew search

ArboratorGrew offre un ensemble exceptionnel de fonctionnalités, notamment son puissant système de recherche de pattern. Avec **[Grew](https://grew.fr/)**, ArboratorGrew vous permet de rechercher en utilisant divers critères, notamment la recherche par `POS`, la recherche par `Form`, la recherche par `Lemme`, la recherche par `Relation de Dépendance`, et la recherche par `Relation et Étiquettes`, le tout adapté au type spécifique d'arbre que vous avez sélectionné.

<div style="text-align:center">
      <img src="assets/images/grew-search.png" alt="drawing" width="900"/>
</div>

?> Les nœuds qui correspondent au pattern sont ensuite mis en évidence dans les arbres de la page de résultats.

</br>

<div style="text-align:center">
      <img src="assets/images/Grew-result.png" alt="drawing" width="1200"/>
</div>


?> Pour détecter les erreurs, il est possible de filtrer ces résultats en fonction de motifs négatifs (des motifs qui ne doivent pas apparaître dans le graphe). Une fois que l'arbre défectueux a été trouvé, il peut alors être directement édité et enregistré.

?> Les requêtes de recherche et les règles de réécriture sont stockées pour permettre aux utilisateurs d'y accéder ultérieurement. Cette fonctionnalité est très utile pour les annotateurs, car elle leur permet de suivre les modifications apportées aux projets à l'aide des règles de réécriture Grew. Ils peuvent gérer cet historique en sélectionnant des requêtes et des règles favorites ou en effaçant tout l'historique.

<div style="text-align:center; border: 0.5px solid #808080;">
      <img src="assets/images/grew-history.png" alt="drawing" width="1200"/>
</div>

## Grew Rewrite

Avec ArboratorGrew, vous avez la possibilité de modifier et de réécrire vos arbres en utilisant les règles de réécriture Grew (voir **[Grew Rules](https://grew.fr/doc/rule/)**).

<div style="text-align:center; border: 0.5px solid #808080;">
      <img src="assets/images/grew-rewriting-rule.png" alt="drawing" width="1200"/>
</div>

Les nœuds qui correspondent à la règle spécifiée seront mis en évidence sur la page des résultats. Pour sauvegarder ces résultats, vous pouvez choisir de sélectionner des résultats individuels ou opter pour l'ensemble des résultats, puis cliquer sur le bouton 'Appliquer les Règles'.



## Relation tables

ArboratorGrew offre également la possibilité de regrouper le treebank en fonction d'une ou de plusieurs caractéristiques. Ces caractéristiques peuvent être utilisées pour construire un tableau de relations qui fournit un résumé complet de toutes les dépendances au sein d'un projet, en mettant l'accent sur la relation de dépendance.

<div style="text-align:center; border: 0.5px solid #808080;">
      <img src="assets/images/relation-table.png" alt="drawing" width="1200"/>
</div> 

!> C'est un excellent moyen de rechercher des structures rares et des erreurs potentielles au sein d'un treebank. L'utilisateur peut accéder directement aux arbres qui correspondent au pattern négatif et les mettre à jour. Cela facilite grandement la détection et la correction d'erreurs dans le treebank.

## Lexicon 

Le lexique est l'une des options avancées disponibles dans **[Arborator-Grew](https://arboratorgrew.elizia.net/#)**. L'utilisateur sélectionne deux listes de caractéristiques :
- $L_1 = [f_1, …, f_m]$ comme caractéristiques principales.
- $L_2 = [g_1, …, g_m]$ comme caractéristiques auxiliaires.

<div style="text-align:center; border: 0.5px solid #808080;">
      <img src="assets/images/select-lexicon-features.png" alt="drawing" width="1200"/>
</div>

La table de sortie correspond aux valeurs possibles de toutes les caractéristiques, de telle manière que pour toutes les combinaisons de valeurs pour $f_i$, il existe plus d'une combinaison de valeurs pour $g_i$. L'idée est de n'afficher que les valeurs de $f$ qui sont ambiguës par rapport aux valeurs de $g$.

#### Exemple 

Pour  $L_1 = [$`Form`, `Lemma`, `Upos`$]$ et $L_2 = [$`Gender `, `Number`$]$ 

<div style="text-align:center">
      <img src="assets/images/lexicon-exemple.png" alt="drawing" width="900"/>
</div>

Cela affichera les entrées où il y a plus d'un couple de valeurs pour `Genre` et `Nombre` avec la même combinaison (`Form`, `Lemme`, `Upos`).


<div style="text-align:center; border: 0.5px solid #808080;">
      <img src="assets/images/lexicon-ambiguous.png" alt="drawing" width="900"/>
</div>
 
Ensuite, l'utilisateur peut les corriger directement en utilisant l'option de règle de réécriture Grew.
<br/><br/>
<div style="text-align:center; border: 0.5px solid #808080;">
      <img src="assets/images/modify-lexicon.png" alt="drawing" width="900"/>
</div> 


?> La deuxième liste $L_2$ est facultative. Si elle n'est pas fournie, toutes les entrées du lexique sont affichées.