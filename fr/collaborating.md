## Collaboration dans les projets

L'annotation collaborative est l'une des fonctionnalités puissantes d'Arborator-Grew. Elle permet à plusieurs utilisateurs de partager l'accès au projet afin de travailler ensemble.

Lorsque vous créez un projet, vous en êtes le **propriétaire**. Dans ce cas, vous avez un contrôle total sur le treebank. Vous pouvez gérer sa configuration, inviter des collaborateurs et consulter les arbres des autres utilisateurs.

?> De plus, nous pouvons distinguer les rôles suivants :

- **L'administrateur** dispose des mêmes options que le **propriétaire**, à l'exception de la synchronisation GitHub et de la gel du projet. **L'administrateur** peut :
  - Modifier les paramètres du projet.
  - Assigner de nouveaux membres au projet.
  - Télécharger de nouveaux échantillons et utiliser le tokenizer.
  - Ajouter des nouvelles phrases en utilisant le tokenizer
  - Changer la segmentation des phrases
  - Modifier les phrases d'un échantillon (comme diviser ou fusionner des jetons...)
  - Utiliser le parseur.
  - Consulter les arbres des autres utilisateurs dans le mode d'annotation à l'aveugle.
  - Supprimer des échantillons ou des arbres d'utilisateurs.

- **Le validateur** endosse le rôle du linguiste en corrigeant le treebank et en choisissant l'arbre validé parmi les arbres des annotateurs.

- **L'annotateur** Chaque échantillon a une liste d'**annotateurs**. Les **annotateurs** peuvent parcourir et modifier le treebank (la modification signifie qu'un arbre modifié est enregistré sous leur nom).

- **L'invité** Ce rôle n'est disponible que pour les projets privés, où vous pouvez choisir quels invités peuvent seulement voir le treebank.

## Invitation de Collaborateurs

Vous pouvez inviter des collaborateurs directement à votre projet en accédant aux paramètres du projet. Vous pouvez rechercher l'utilisateur dans la liste des utilisateurs, définir le rôle et cliquer sur le bouton "partager".

<div style="text-align:center">
      <img src="assets/images/add-user.png" alt="drawing" width="900"/>
</div>
