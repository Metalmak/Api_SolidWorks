<!-- source: obsoleteapi/Mate/Mate.htm -->

# Mate Object

This object and its methods and properties
are obsolete and have been superseded by Mate2.

|  |  |  |
| --- | --- | --- |
| ![](../AssemblyDoc.gif) | | |

|  | ![image\branch1.gif](../image/branch1.gif)![](../Mate_h.gif) | |
|  |  | ![image\branch1.gif](../image/branch1.gif)![image\MateEntity.gif](../image/MateEntity.gif) |

Allows access to various assembly mate parameters.

To get the Mate object, you must first get it as a Feature object and
then use Feature::GetSpecificFeature2 or QueryInterface to return the
Mate interface.

The Mate object is actually a subfeature beneath a MateGroup feature.
To access the Mate subfeature by traversing the FeatureManager design
tree, you can call Feature::GetFirstSubFeature and Feature::GetNextSubFeature
when the current feature type is MateGroup.

Use the Accessors
link to obtain a list of functions that return this object.