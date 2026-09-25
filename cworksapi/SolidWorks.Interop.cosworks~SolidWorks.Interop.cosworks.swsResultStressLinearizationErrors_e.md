<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultStressLinearizationErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsResultStressLinearizationErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsResultStressLinearizationErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Linearized stress errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsResultStressLinearizationErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsResultStressLinearizationErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsResultStressLinearizationErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsResultStressLinearizationErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsStressLinearization\_AllElementsNotFoundForIntermediatePoints** | 8 = No elements were found near any of the intermediate points |
| **swsStressLinearization\_DatabaseNotAvailable** | 4 = Mesh or study results are not available |
| **swsStressLinearization\_ElementalValuesNotSupported** | 10 = Plotting with elemental values is not supported |
| **swsStressLinearization\_ElementsFromDifferentComponents** | 7 = Elements at the end points are from different bodies |
| **swsStressLinearization\_ElementsNotFoundForEndPoints** | 6 = No elements were found near the specified end points |
| **swsStressLinearization\_IncorrectNumberOfIntermediatePoints** | 5 = Number of intermediate points must be greater than 0 and less than 100 |
| **swsStressLinearization\_InvalidNumberOfPointsSelected** | 13 = Number of points must be 2 |
| **swsStressLinearization\_InvalidReferencePlane** | 3 = Only SWDATUMPLANES are supported |
| **swsStressLinearization\_InvalidResultComponent** | 12 = Invalid result component |
| **swsStressLinearization\_MeshTypeNotSupported** | 2 = Only solid meshes are supported |
| **swsStressLinearization\_SpecifiedPointsNotOnSectionPlane** | 9 = The specified points are not on the section plane |
| **swsStressLinearization\_StudyNotSupported** | 1 = Only pressure vessel studies are supported |
| **swsStressLinearization\_Success** | 0 |
| **swsStressLinearization\_VectorPlotNotSupported** | 11 = Vector plots are not supported |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)