## Blind annotation mode

Blind annotation is a widely used in research, where the annotators independently label trees without access to the annotations made by other annotators. This practice can minimize bias and ensure the objectivity. Additionally, the concept of the blind annotation can be used for teaching syntactic annotation for the students. 

This concept is already implemented in ArboratorGrew through the Blind Annotation mode. To activate this feature, administrator can configure it during project creation or within the project settings window.

## Blind annotation levels

In ArboratorGrew, the blind annotation mode offers multiple levels of configuration, allowing the admins to adjust the degree of blind annotation for each sample. These levels are explained below for better understanding:

| Blind annotation level     |property  |
| ------------------- |--------------------------------------------------------------------------  |
| `1:validated_visible`| <div style="width:100%,">When Editing, the annotators can see the validated tree, the differences are highlighted in red and they can access to the statistics</div>|
| `2:local_feedback`|<div style="width:100%,">Here, the validated tree is not visible, but differences are still highlighted and statistics are available.</div> |
|`3:global_feedback`|The annotators can only access to the statics statistics|
|`4:no_feedback`|<div style="width:100%,">Nothing is provided only the validator who can see the trees and access to the statistics</div>|


## Tree types in the blind annotation mode

Within this mode, we have three distinct types of trees: the base tree, the user tree, and the validated tree.

**Base Tree**: The base tree serves as the starting point for the annotator's work. It provides the initial structure upon which the annotation process begins.

**User Tree**: This refers to the tree created and modified by the annotator during the annotation process. It represents the annotator's input and efforts.

**Validated Tree**: The validated tree signifies the version of the tree that has been approved by a validator.

Users have the  access to the same annotation options as previously mentioned. However, due to the limited visibility of trees for annotators, certain tree types may not be accessible to them.

For all the features where tree types need to be selected, the validator has access to all trees, including the most recent trees, validated trees, and pending trees.However, the annotator has access only to their own trees.





