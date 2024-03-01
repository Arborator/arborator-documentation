## Bienvenue dans la documentation d'ArboratorGrew

Ceci est la documentation officielle pour **[ArboratorGrew](https://arboratorgrew.elizia.net/#/)**

Un outil d'annotation **collaborative** pour le développement de **treebank**. 

Vous trouverez ci-dessous un bref résumé des principales fonctionnalités d'Arborator et des cas d'utilisation. Pour plus de détails et de tutoriels, utilisez la barre de navigation à gauche. 

Jetons un coup d'œil à la documentation.


## Caractéristiques principales

Arborator-Grew combine les fonctionnalités de deux outils préexistants : `Arborator` et `Grew`. 

**[Arborator](https://arborator.ilpga.fr/)** est un outil d'annotation des arbres de dépendences en ligne, graphique et collaboratif, largement utilisé.

**[Grew](https://grew.fr/)** est un outil d'interrogation et de réécriture de graphes spécialisé dans les structures nécessaires au NLP, c'est-à-dire les arbres et les graphes de dépendance syntaxiques et sémantiques. Grew a également une version en ligne, **[Grew-match](http://match.grew.fr/)**, où tous les treebanks de **[UD Universal Dependencies](https://universaldependencies.org/)** et **[SUD Surface Syntactic Universal Dependencies](https://surfacesyntacticud.github.io/)** peuvent être consultés.

> **[ArboratorGrew](https://arboratorgrew.elizia.net/#/)** est prêt à traiter des données des deux schémas d'annotation
**[Universal Dependencies (UD)](https://universaldependencies.org/)** ou
**[Surface Syntactic Universal Dependencies (SUD)](https://surfacesyntacticud.github.io/)**.
Il peut également facilement être adapté à d'autres shémas.

## Cas d'utilisation principal Scénarios
ArboratorGrew peut être utilisé pour une variété de scénarios. Dans la section ci-dessous, nous décrivons comment les utilisateurs se servent d'ArboratorGrew dans leur  travail d'annotation.

#### Maintenir un treebank existant

Github est l'outil le plus courant pour stocker des treebanks. Si vous avez déjà un treebank existant, ArboratorGrew vous permet de la synchroniser directement avec votre projet. Voici comment entretenir un treebank existant:

- L'utilisateur importe des échantillons depuis github en utilisant la fonctionnalité de synchronisation.
- Les arbres sont importés en tant qu'arbres **validated**.
- L'utilisateur peut annoter l'arbre **"validated"** directement, ou utiliser son arbre comme brouillon et le sauvegarder plus tard en tant qu'arbre **"validated"**.
- Le nombre de modifications est suivi une fois l'annotation terminée, l'utilisateur peut faire un commit de ses modifications.

Si plusieurs annotateurs travaillent sur le même dépôt github, ils doivent suivre les règles mentionnées dans la section github.


#### Commencer à documenter une nouvelle langue

Un grand nombre de langues à ressources limitées ont été documentées à l'aide d'ArboratorGrew dans le cadre du projet **[SUD](https://surfacesyntacticud.github.io/)**. Le processus est décrit ci-dessous :

- L'utilisateur commence généralement par des fichiers audio, qui seront annotés à l'aide d'un outil d'annotation audio tel que **[ELAN](https://archive.mpi.nl/tla/elan)**. 
- L'utilisateur transforme le fichier généré en fichier Conll à l'aide de scripts ; cette étape n'est pas prise en charge par ArboratorGrew.
- L'utilisateur importe le fichier Conll dans ArboratorGrew sous son propre nom ou en utilisant l'arbre **"validated"**.
- L'utilisateur peut annoter ses arbres et peut les exporter et les télécharger vers le dépôt Github. Nous l'encourageons fortement à utiliser la synchronisation Github une fois qu'il a terminé.


#### Annotation collaborative

Dans les cas précédents, nous supposons qu'une seule personne travaille sur le projet d'annotation. Dans cette section, nous décrivons le cas où l'annotation du projet est gérée par plusieurs annotateurs. Ce scénario peut s'appliquer au démarrage de l'annotation d'une nouvelle langue ou à la maintenance d'une langue existante.

- Les administrateurs doivent spécifier le rôle de chaque collaborateur.
- Les annotateurs utilisent les tags pour indiquer leur progression dans l'annotation.
- Le validateur filtre les arbres pour valider ceux qui ont la balise **"Done"**.
- Le validateur choisit l'arbre validé parmi les arbres des utilisateurs ou commence à partir du dernier arbre, effectue ses modifications et l'enregistre en tant qu'arbre **"validated"**.

#### Utiliser le parser (l'analyseur syntaxique)

ArboratorGrew offre la possibilité de commencer le processus d'annotation par une pré-annotation en utilisant le parser. 

- L'utilisateur importe un fichier Conll non annoté dans son projet.
- L'utilisateur dispose d'une liste de modèles pré-entraînés regroupés par langue. Si la langue de du treebank existe, l'utilisateur peut utiliser directement le parser de cette langue, sinon il peut utiliser l'analyseur d'une langue proche de la langue du treebank.
- L'analyseur génère des arbres avec le préfixe **"parser"**.
- L'annotateur peut commencer l'annotation à partir des arbres du parser.








