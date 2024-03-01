## Welcome to ArboratorGrew Documentation

This is the official user documentation for **[ArboratorGrew](https://arboratorgrew.elizia.net/#/)**

?> A **collaborative annotation** tool for the **treebank** developpement. 

Below is brief summary of Arborator's main features and user cases. For more details and tutorials, use the navigation bar on the left. 

Let's have a look at the documentation.


## Main Features

Arborator-Grew combines the features of two preexisting tools: `Arborator` and `Grew`. 

> **[Arborator](https://arborator.ilpga.fr/)** is a widely used collaborative graphical online dependency treebank
annotation tool. 

> **[Grew](https://grew.fr/)** is a tool for graph querying and rewriting specialized in structures needed in NLP, i.e. syntactic and semantic
dependency trees and graphs. Grew also has an online version, **[Grew-match](http://match.grew.fr/)**, where all Universal Dependencies treebanks in their classical,
deep and surface-syntactic flavors can be queried.

> **[ArboratorGrew](https://arboratorgrew.elizia.net/#/)** opens up new paths of collectively
creating, updating, maintaining, and curating syntactic treebanks.

> **[ArboratorGrew](https://arboratorgrew.elizia.net/#/)** is ready to be used with data following 
**[Universal Dependencies (UD)](https://universaldependencies.org/)** or 
**[Surface Syntactic Universal Dependencies (SUD)](https://surfacesyntacticud.github.io/)** annotation frameworks
but it can easily be configured for other annotation schemas.

## Main use case Scenarios
ArboratorGrew can be used for a variety of scenarios. In the section below, we outline how users use ArboratorGrew in their annotation workflow.

#### Maintain existing treebank

Github is the most common tool for storing treebanks. If you already have an existing treebank, ArboratorGrew allows you to synchronize it directly with your project. Here's how to maintenance an existing treebank

- The user imports samples from github using the synchronization feature.
- Trees are imported as **validated** trees.
- The user can annotate the **"validated "** tree directly, or use their tree as a draft and save it later as a **"validated "** tree.
- The number of modifications is tracked once the annotation is finished the user can commit their modifications.

If many annotators are working on the same github repository, they should follow the best practices mentioned in the github section.


#### Start documenting new language

A large number of low-resource languages have been documented using ArboratorGrew as part of the **[SUD](https://surfacesyntacticud.github.io/)** project. The process is described below:

- The user usually starts with audio files, which will be annotated using an audio annotation tool such as **[ELAN](https://archive.mpi.nl/tla/elan)**. 
- The user transforms the generated file into a Conll file using scripts; this step is not supported by ArboratorGrew.
- The user imports the Conll file into ArboratorGrew under their own name or using the **"validated "** tree.
- The user can annotate their trees and can export and upload them to the Github repository. We strongly encourage them to use Github synchronization once they've finished.


#### Collaborative annotation

In the previous cases, we assume that only one person is working in the annotation project. In this section, we describe the case where the project annotation is managed by several annotators. This scenario can be applied in case of starting the annotation of new language or maintaining an existing one.

- Admins need to specify the role of each collaborator.
- Annotators use the tags to indicate their progress in the annotation.
- Validator filter the trees to validate those with the **"Done"** tag.
- Validator chooses the validated tree bewteen users' trees or starts from the last tree, makes their changes and saves it as **"validated"** tree.

#### Use the parser

ArboratorGrew offer the possibility of starting the annotation process with a pre-annotation using the parser. 

- User imported an unannotated Conll file into their project.
- User have a list of pretrained models grouped by language. If the language of the treebank exists, user can use directly the parser for this language, otherwise they can use the parser of language that's close to the treebank language.
- The parser will generate trees with prefix parser **"parser"**.
- Annotator can start the annotation from the parsed trees
