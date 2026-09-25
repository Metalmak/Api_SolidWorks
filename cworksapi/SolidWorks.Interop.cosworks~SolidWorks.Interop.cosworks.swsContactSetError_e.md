<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactSetError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsContactSetError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsContactSetError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Contact set errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsContactSetError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsContactSetError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsContactSetError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsContactSetError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsContactSetErrorBondedContactForTouchingFaces** | 10 = Bonded contact for drop test studies is only allowed for touching faces |
| **swsContactSetErrorCannotCreateContactPair** | 12 = Contact pair cannot be created for this study type |
| **swsContactSetErrorFaceForSourceAndTarget** | 7 = At least one face is specified for both source and target |
| **swsContactSetErrorInvalidArray** | 1 = Invalid array |
| **swsContactSetErrorInvalidType** | 3 = Invalid contact set type |
| **swsContactSetErrorNoEntities** | 2 = No entities specified (empty array) |
| **swsContactSetErrorSelectOneTargetPlane** | 5 = Specify faces, edges, or vertices for source |
| **swsContactSetErrorSelectOnlyFaces** | 6 = Only faces can be selected for target |
| **swsContactSetErrorShrinkFitNeedsIntereference** | 11 = Shrink fit requires that source and target bodies interfere |
| **swsContactSetErrorSourceTargetFacesMustTouch** | 9 = Node to node contact requires that source and target faces touch |
| **swsContactSetErrorSpecifyFacesEdgesOrVertices** | 4 = Specify faces, edges, or vertices for source |
| **swsContactSetErrorSuccess** | 0 = Successful |
| **swsContactSetErrorVerticesEdgesForBondingSurfaceContacts** | 8 = Vertices and edges are allowed in source entities only for bonding  and surface contact conditions |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)