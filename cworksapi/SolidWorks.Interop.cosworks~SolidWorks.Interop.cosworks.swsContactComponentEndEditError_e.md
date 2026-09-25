<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactComponentEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsContactComponentEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsContactComponentEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Contact component editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsContactComponentEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsContactComponentEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsContactComponentEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsContactComponentEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsContactComponentEndEditErrorBodiesNotTouchingBodies** | 8 = Specified bodies for bonding or node to node contact condition are not touching other bodies |
| **swsContactComponentEndEditErrorCannotSpecifyFreeContact** | 7 = Free contact may not be specified for components that interfere with other components |
| **swsContactComponentEndEditErrorContactComponentCannotBeCreated** | 1 = Contact component cannot be created for this study type |
| **swsContactComponentEndEditErrorIncorrectCoefficientOfFriction** | 4 = Coefficient of friction must be greater than or equal to 0 and less than or equal to 1.0 |
| **swsContactComponentEndEditErrorInvalidContactType** | 2 = Invalid contact type |
| **swsContactComponentEndEditErrorSelectComponentOrBody** | 3 = Select one component or one body |
| **swsContactComponentEndEditErrorSelectSolidBodyOrComponent** | 5 = Select only one solid body or component |
| **swsContactComponentEndEditErrorSuccessful** | 0 = Successful |
| **swsContactComponentEndEditErrorTooManyBodiesOrComponents** | 6 = At least one body or component is specified more than once |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)