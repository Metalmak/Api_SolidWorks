<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swBOMConfigurationCreationErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swBOMConfigurationCreationErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swBOMConfigurationCreationErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

BOM table configuration creation errors.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swBOMConfigurationCreationErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swBOMConfigurationCreationErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swBOMConfigurationCreationErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swBOMConfigurationCreationErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swBOMTableCreation\_AlreadyExists** | -3 = BOM table already exists for this drawing view |
| **swBOMTableCreation\_ExcelDisabled** | -4 = BOM table cannot be created because Microsoft Excel is disabled on this system |
| **swBOMTableCreation\_Failed** | -5 = BOM table creation failed because the specified template is not valid |
| **swBOMTableCreation\_MustBeDrawingView** | -2 = BOM tables can only be added to a drawing view |
| **swBOMTableCreation\_NoModelForView** | -6 = No model available for drawing view |
| **swBOMTableCreation\_Okay** | 0 = Table was successfully created |
| **swBOMTableCreation\_UnspecifiedError** | -1 = Table could not be created for unknown reasons |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)