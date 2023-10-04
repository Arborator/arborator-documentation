## Treebank Graphic Annotation
Pour commencer l'annotation du treebank, vous avez deux options :

- Importer un fichier `CoNLL` en tant qu'entrée.
- Introduire du texte en tant qu'entrée et utiliser les différentes options du tokenizer.
<div style="text-align:center">
      <img src="assets/images/upload-sample.png" alt="drawing" width="900"/>
</div>
Arborator traduit les données CoNLL en arbres graphiques. Voici comment fonctionne l'interface de l'annotation graphique:

?> Pour établir une relation de dépendance entre deux jetons, il vous suffit de faire glisser la flèche du token vers l'autre.

?> Pour créer une dépendance racine, vous devez faire glisser la flèche du token vers le haut.

?> Pour modifier les caractéristiques du token, cliquez dessus et vous pouvez choisir et définir différentes caractéristiques telles que les `Caractéristiques Universelles`, les `Caractéristiques Diverses` et les `Lemmes`.

?> Pour attribuer une catégorie au token, cliquez sur le trait souligné et sélectionnez la catégorie appropriée.

?> Pour supprimer une annotation, le bouton violet de suppression vous permettra de supprimer les différentes parties d'annotation mentionnées ci-dessus.

<div style="text-align:center">
      <video autoplay loop width="900">
            <source src="assets/videos/1-Annotation.webm" type=video/webm>
      </video>
</div>


## Annotation Functionnalities

Il y a une barre d'outils située en haut à gauche de la zone de la vue de l'arbre. À partir de là, l'utilisateur peut effectuer les actions suivantes :

<div style="text-align:center">
      <img src="assets/images/edit-treebank.png" alt="drawing" width="400"/>
</div>

- Chaque fois qu'une modification est apportée à l'arbre (par exemple, une nouvelle annotation ou une relation ajoutée), un disque jaune apparaîtra pour indiquer qu'il y a des modifications à **enregistrer**. Cliquez sur le bouton **Enregistrer** pour **sauvegarder** les modifications.

- Vous avez la possibilité d'ajouter des **tags** à vos arbres en utilisant la **fonction des tags**. Ces tags servent d'outil d'organisation précieux, simplifiant votre processus d'annotation. De plus, ils facilitent la collaboration efficace au sein de votre équipe en vous permettant de communiquer sur votre avancement. Il existe des tags prédéfinies disponibles, et vous avez également la possibilité de créer vos propres tags.

<div style="text-align:center">
      <img src="assets/images/tags.png" alt="drawing" width="400"/>
</div>

- Vous pouvez activer le mode de différence pour mettre en évidence les différences d'annotation entre les annotateurs dans la structure de l'arbre. Cette fonctionnalité peut également être activée directement en faisant un clic droit sur l'utilisateur pour lequel vous recherchez des différences.

- Vous avez également la possibilité d'obtenir un fichier `PNG`, `SVG` et `CONLL` de l'arbre.

#### Tokens editing options

- Vous avez la possibilité de manipuler les tokens au sein d'une phrase en les fusionnant, en les divisant ou en insérant un token à un emplacement particulier. Pour ce faire, il vous suffit de sélectionner le token que vous souhaitez modifier dans la phrase affichée dans la vue de l'arbre, et vous obtiendrez un menu avec ces options disponibles.

<div style="text-align:center">
      <img src="assets/images/edit-tokens.png" alt="drawing" width="200"/>
</div>
