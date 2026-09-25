<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactSetEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsContactSetEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsContactSetEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Contact set editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsContactSetEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsContactSetEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsContactSetEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsContactSetEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsContactSetEndEditErrorBondTouchingFacesInDropTestStudies** | 15 = In drop test studies, you can only bond touching faces |
| **swsContactSetEndEditErrorContactSetsMustBeUnique** | 13 = For thermal resistance, contact sets must be unique; use the split-line features to split common faces; you may need to redefine existing contact sets |
| **swsContactSetEndEditErrorEntityAlreadySpecified** | 2 = At least one entity is specified more than once |
| **swsContactSetEndEditErrorIncorrectCoefficientFriction** | 10 = Coefficient of friction must be >= 0 and <= 1.0 |
| **swsContactSetEndEditErrorInvalidContactSetType** | 3 = Invalid contact set type |
| **swsContactSetEndEditErrorInvalidOption** | 4 = Invalid option |
| **swsContactSetEndEditErrorNodeToNodeContactAndSourceTargetFaces** | 14 = Node to node contact requires that source and target faces touch |
| **swsContactSetEndEditErrorNoEntityAtIndex** | 1 = No entity is passed at index |
| **swsContactSetEndEditErrorOnlyFacesAllowedForTarget** | 7 = Only faces are allowed for target |
| **swsContactSetEndEditErrorShrinkFitAndnterferingSourceTargetBodies** | 16 = Shrink fit requires that source and target bodies interfere |
| **swsContactSetEndEditErrorSpecifyFacesEdgesOrVerticesForSource** | 5 = Specify faces, edges, or vertices for source |
| **swsContactSetEndEditErrorSpecifyOneTargetPlaneForVirtualWall** | 6 = Specify only one target plane for virtual wall |
| **swsContactSetEndEditErrorStiffnessCannotBeNegative** | 8 = Stiffness cannot be negative |
| **swsContactSetEndEditErrorStiffnessMustBePositive** | 9 = Specify a positive value for at least one of the stiffness parameters |
| **swsContactSetEndEditErrorSuccessful** | 0 = Successful |
| **swsContactSetEndEditErrorThermalResistanceMustBePositive** | 12 = Thermal resistance must have a positive value |
| **swsContactSetEndEditErrorVerticesAndEdgesForBondingAndSurfaceContacts** | 11 = Vertices and edges are allowed as source entities only for bonding and surface contact conditions |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)