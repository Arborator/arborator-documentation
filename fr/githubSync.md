## Synchronisation avec GitHub

ArboratorGrew offre une intégration transparente avec votre dépôt GitHub, un choix populaire parmi les linguistes pour la gestion des treebanks. Cette intégration vous permet de synchroniser facilement avec GitHub, garantissant que vous restez à jour avec vos annotations. De plus, cela ouvre des possibilités de collaboration en permettant à votre projet ArboratorGrew de faire partie de l'environnement collaboratif de GitHub, facilitant ainsi le travail avec des collègues travaillant directement depuis GitHub.

!> Dans le cas où plusieurs collaborateurs travaillent directement depuis GitHub, il est important de suivre les meilleures pratiques pour éviter d'éventuels problèmes. Ces pratiques recommandées seront abordées dans les sections suivantes.

## Connexion avec GitHub Social Login

La première étape pour utiliser cette fonctionnalité est de vous connecter à ArboratorGrew en utilisant votre compte GitHub afin d'accorder l'accès à vos dépôts GitHub.

## Synchroniser votre projet ArboratorGrew avec votre dépôt Github

!> Seul le propriétaire du projet peut synchroniser avec GitHub.

Après avoir connecté votre compte ArboratorGrew avec vos identifiants GitHub, vous avez la possibilité de synchroniser votre projet ArboratorGrew avec un dépôt GitHub. Veuillez noter que vous devez être le propriétaire du dépôt ou avoir un accès en lecture/écriture. Ce processus de synchronisation peut être lancé lors de la création d'un nouveau projet ArboratorGrew.

- Dans la fenêtre de création du nouveau projet, vous aurez un bouton vous demandant de synchroniser avec le dépôt GitHub.

<div style="text-align:center">
      <img src="assets/images/1-github.png" alt="drawing" width="900"/>
</div> 

- Ou lorsque vous cliquez sur l'icône GitHub sur la page du projet.

<div style="text-align:center">
      <img src="assets/images/3-github.png" alt="drawing" width="900"/>
</div> 

- Vous obtiendrez une liste de tous vos dépôts GitHub, filtrée par propriétaire.
- Sélectionnez le dépôt avec lequel vous souhaitez synchroniser et la branche que vous souhaitez importer.
- Ensuite, vous aurez deux options : travailler avec la branche que vous avez sélectionnée à l'étape précédente afin que tous les commits et pulls soient effectués dans cette branche. Ou créer une nouvelle branche nommée `arboratorgrew` qui sera utilisée uniquement pour les commits et pulls réalisés avec ArboratorGrew. Cette option permettra de préserver l'intégrité de votre base de code principale.

<div style="text-align:center">
      <img src="assets/images/2-github.png" alt="drawing" width="900"/>
</div> 

- ArboratorGrew n'importera que les fichiers conll qui se trouvent à la racine de votre dépôt GitHub. Assurez-vous que votre dépôt GitHub a une représentation aplatie.

## Flux de travail GitHub

<div style="text-align:center">
      <img src="assets/images/4-github.png" alt="drawing" width="1000"/>
</div> 

#### Pousser vers GitHub

Une fois que votre projet ArboratorGrew est synchronisé avec un dépôt GitHub spécifique et une branche, toutes les modifications que vous apportez à votre projet sont prises en compte (enregistrement d'arbres, téléchargement de nouveaux échantillons, suppression d'échantillons). Lorsque vous êtes prêt à valider ces modifications, vous cliquez sur le bouton de validation dans le menu des options GitHub.

- Il vous demandera de saisir un message de validation.
- Vous pouvez choisir de ne pousser que vos arbres, les arbres validés ou vos arbres remplis avec les plus récents.

<div style="text-align:center">
      <img src="assets/images/5-github.png" alt="drawing" width="900"/>
</div> 

#### Récupérer depuis GitHub

ArboratorGrew écoutera uniquement les modifications apportées dans la branche sélectionnée lors des étapes précédentes (arboratorgrew ou la branche synchronisée). Si vous souhaitez récupérer les modifications, cliquez sur le bouton de récupération dans le menu des options GitHub. Cela rafraîchira la synchronisation pour obtenir les nouvelles modifications apportées dans votre dépôt GitHub.

<div style="text-align:center">
      <img src="assets/images/6-github.png" alt="drawing" width="900"/>
</div> 

#### Demandes de Tirage (Pull Request)

Une fois que vous êtes prêt à fusionner vos modifications dans une autre branche, vous pouvez cliquer sur le bouton de demande de tirage (pull request). Cela vous permettra de créer une nouvelle demande de tirage.

<div style="text-align:center">
      <img src="assets/images/10-github.png" alt="drawing" width="900"/>
</div> 

#### Désynchronisation depuis GitHub

Si vous souhaitez vous déconnecter de la synchronisation GitHub, vous pouvez la supprimer en cliquant sur le bouton de suppression de la synchronisation. Les fichiers ne seront pas supprimés du dépôt GitHub ni de votre projet ArboratorGrew.

## Meilleures pratiques

Comme mentionné précédemment, il existe deux façons d'utiliser la fonctionnalité GitHub.

Le premier scénario est lorsque vous êtes le seul mainteneur dans ArboratorGrew et que vous utilisez GitHub comme un outil de stockage. Dans ce cas, vous pouvez travailler directement avec la branche par défaut sans avoir besoin d'utiliser la branche `arboratorgrew`.

Le deuxième moyen implique une collaboration avec des personnes travaillant sur le treebank directement depuis GitHub. Assurez-vous de suivre ces étapes pour éviter tout conflit potentiel :

?> Utilisez la branche `arboratorgrew` sur GitHub et restreignez l'accès à cette branche pour éviter les conflits.

!> Si vous avez des modifications non validées par des collaborateurs travaillant sur ArboratorGrew lorsque vous récupérez des modifications depuis GitHub, les modifications non validées dans ArboratorGrew seront perdues et écrasées par les modifications récupérées.

Si vous travaillez avec la branche `arboratorgrew` depuis GitHub, procédez comme suit :

1. Poussez toutes les modifications apportées depuis ArboratorGrew vers GitHub.
2. Évitez de travailler sur le treebank depuis ArboratorGrew. Pour ce faire, vous devez désactiver votre projet en utilisant la fonction de gel de projet. Cela empêchera les annotateurs du projet d'apporter de nouvelles modifications tout en effectuant les étapes suivantes.

<div style="text-align:center">
      <img src="assets/images/7-github.png" alt="drawing" width="900"/>
</div> 

3. Fusionnez les modifications faites en dehors de la branche `arboratorgrew` depuis GitHub.

?> Lors de la mise à jour de la branche `arboratorgrew`, vous pourriez avoir des conflits. Essayez de les résoudre directement depuis GitHub.

4. Récupérez les modifications depuis GitHub vers votre branche ArboratorGrew.

!> Si ArboratorGrew détecte une syntaxe invalide, vos modifications ne seront pas récupérées. Assurez-vous que les modifications faites sur GitHub sont valides.

5. À cette étape, vous pouvez débloquer votre projet ArboratorGrew.

!> Il peut arriver que vous ne puissiez pas trouver certains dépôts d'organisation dans votre liste de dépôts lors de la synchronisation. Cela se produit lorsque vous oubliez de donner accès à cette organisation lorsque vous vous connectez à ArboratorGrew avec votre compte GitHub.
Pour résoudre ce problème, vous devez :
1. Accédez aux [paramètres des applications GitHub](https://github.com/settings/applications)
2. Révoquez l'accès à l'application Arborator.
<div style="text-align:center">
      <img src="assets/images/8-github-sync.png" alt="drawing" width="900"/>
</div>  

3. Essayez de vous reconnecter à ArboratorGrew.
4. Vous serez redirigé vers une page où vous pourrez sélectionner l'organisation à laquelle vous souhaitez accorder l'accès.

<div style="text-align:center">
      <img src="assets/images/9-github-sync.png" alt="drawing" width="900"/>
</div> 

