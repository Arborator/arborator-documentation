## Mode d'annotation à l'aveugle

L'annotation à l'aveugle est largement utilisée dans la recherche, où les annotateurs étiquettent indépendamment les arbres sans avoir accès aux annotations faites par d'autres annotateurs. Cette pratique permet de minimiser les biais et de garantir l'objectivité. De plus, le concept de l'annotation à l'aveugle peut être utilisé pour enseigner l'annotation syntaxique aux étudiants.

Ce concept est déjà mis en œuvre dans ArboratorGrew grâce au mode d'annotation à l'aveugle. Pour activer cette fonctionnalité, l'administrateur peut la configurer lors de la création du projet ou dans la fenêtre de paramètres du projet.

## Niveaux d'annotation à l'aveugle

Dans ArboratorGrew, le mode d'annotation à l'aveugle offre plusieurs niveaux de configuration, permettant aux administrateurs d'ajuster le degré d'annotation à l'aveugle pour chaque échantillon. Ces niveaux sont expliqués ci-dessous pour une meilleure compréhension :

| Niveau d'annotation à l'aveugle | Propriété |
| ------------------- |--------------------------------------------------------------------------  |
| `1:validated_visible`| <div style="width:100%">En mode édition, les annotateurs peuvent voir l'arbre validé, les différences sont surlignées en rouge et ils ont accès aux statistiques.</div>|
| `2:local_feedback`|<div style="width:100%">Ici, l'arbre validé n'est pas visible, mais les différences sont toujours surlignées et les statistiques sont disponibles.</div> |
|`3:global_feedback`|Les annotateurs ont uniquement accès aux statistiques.|
|`4:no_feedback`|<div style="width:100%">Rien n'est fourni, seul le validateur peut voir les arbres et accéder aux statistiques.</div>|


## Types d'arbres dans le mode d'annotation à l'aveugle

Dans ce mode, nous avons trois types distincts d'arbres : l'arbre de base, l'arbre de l'utilisateur et l'arbre validé.

**Arbre de base** : L'arbre de base sert de point de départ pour le travail de l'annotateur. Il fournit la structure initiale sur laquelle commence le processus d'annotation.

**Arbre de l'utilisateur** : Il s'agit de l'arbre créé et modifié par l'annotateur au cours du processus d'annotation. Il représente l'apport et les efforts de l'annotateur.

**Arbre validé** : L'arbre validé signifie la version de l'arbre qui a été approuvée par un validateur.

Les utilisateurs ont accès aux mêmes options d'annotation que précédemment mentionnées. Cependant, en raison de la visibilité limitée des arbres pour les annotateurs, certains types d'arbres peuvent ne pas leur être accessibles.

Pour toutes les fonctionnalités où les types d'arbres doivent être sélectionnés, le validateur a accès à tous les arbres, y compris les arbres les plus récents, les arbres validés et les arbres en attente. Cependant, l'annotateur n'a accès qu'à ses propres arbres.




