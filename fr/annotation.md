## Treebank Graphic Annotation
Pour commencer l'annotation du treebank, vous avez deux options :

- Importer un fichier `CoNLL` en tant qu'entrée.
- Introduire du texte en tant qu'entrée et utiliser les différentes options du tokenizer.
Il y a trois options pour le tokenizer : **tokenizer texte brut** pour les deux langues français et anglais, **tokenizer horizontal** où chaque phrase est sur une ligne séparée et **tokenizer vertical** où chaque token est sur une ligne séparée avec une ligne vide indiquant la fin de la phrase.
- Le tokenizer est utile pour ajouter de nouvelles phrases aux échantillons.
- Vous pouvez aussi choisir le nom d'utilisateur qui sera associé à vos arbres importés.
- Pour les langues RTL, l'utilisateur doit cocher l'option RTL.

<div style="text-align:center">
      <figure>
            <img src="assets/images/upload-sample.png" alt="drawing" width="900"/>
            <figcaption>Import Conll file</figcaption>
      </figure>
</div>
<div style="text-align:center">
      <figure>
            <img src="assets/images/tokenizer.png" alt="drawing" width="900"/>
            <figcaption>Tokenizer options</figcaption>
      </figure>
</div>
Arborator traduit les données CoNLL en arbres graphiques. Voici comment fonctionne l'interface de l'annotation graphique:

?> Pour établir une relation de dépendance entre deux jetons, il vous suffit de faire glisser la flèche du token vers l'autre.

?> Pour créer une dépendance racine, vous devez faire glisser la flèche du token vers le haut.

?> Pour modifier les caractéristiques du token, cliquez dessus et vous pouvez choisir et définir différentes caractéristiques telles que les `Caractéristiques Universelles`, les `Caractéristiques Diverses` et les `Lemmes`.

?> Pour attribuer une catégorie au token, cliquez sur le trait souligné et sélectionnez la catégorie appropriée.

?> Pour supprimer une annotation, le bouton violet de suppression vous permettra de supprimer les différentes parties d'annotation mentionnées ci-dessus.



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


#### La segmentation des phrases

Les annotateurs sont généralement confrontés au problème de la segmentation des phrases au cours du processus d'annotation. Ils veulent soit diviser une phrase en deux autres phrases, soit fusionner deux phrases pour en former une seule, ce qui peut être fait à l'aide de la fonction de segmentation des phrases. Les captures d'écran suivantes illustrent ces deux options.

<div style="text-align:center">
      <figure>
            <img src="assets/images/split-sent.png" alt="drawing" width="1000"/>
            <figurecaption>Sentence divison</figurecaption>
      </figure>
</div>
</br>
<div style="text-align:center">
      <figure>
            <img src="assets/images/merge-sent.png" alt="drawing" width="1000"/>
            <figurecaption>Sentences merge</figurecaption>
      </figure>
</div>

#### Edition des tokens

- Vous avez la possibilité de manipuler les tokens au sein d'une phrase en les fusionnant, en les divisant ou en insérant un token à un emplacement particulier. Pour ce faire, il vous suffit de cliquer sur le token que vous souhaitez modifier dans la vue de l'arbre, et vous obtiendrez un menu avec ces options disponibles.

<div style="text-align:center">
      <img src="assets/images/edit-tokens.png" alt="drawing" width="400"/>
</div>

- Vous pouvez aussi avoir cette fonctionnalité à partir de la vue du tableau. Pour afficher la liste des options il suffit de cliquer avec le bouton droit de la souris sur la ligne du token concerné.

<div style="text-align:center">
      <img src="assets/images/edit-tokens-2.png" width="900"/>
</div>

#### Le mode diff

ArboratorGrew vous aide à comparer efficacement deux annotations en utilisant le mode diff. Pour activer le mode diff, cliquez avec le bouton droit de la souris sur l'icône de l'utilisateur que vous souhaitez utiliser comme référence pour la comparaison. L'icône de l'utilisateur se transforme en chapeau de graduation et les changements sont mis en évidence en rouge dans l'arbre ouvert.
<div style="text-align:center">
      <img src="assets/images/diff-mode.png" alt="drawing" width="1200"/>
</div>
