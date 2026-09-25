<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSpotWeldConnectorEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsSpotWeldConnectorEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsSpotWeldConnectorEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Spot weld connector editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsSpotWeldConnectorEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsSpotWeldConnectorEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsSpotWeldConnectorEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsSpotWeldConnectorEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsSpotWeldConnectorEndEditErrorBodyExcludedFromAnalysis** | 18 = Selected entity is on a body excluded from analysis |
| **swsSpotWeldConnectorEndEditErrorEntityAlreadyExists** | 2 = Entity already exists |
| **swsSpotWeldConnectorEndEditErrorFaceIsEmpty** | 3 = Either the first face or second face is empty |
| **swsSpotWeldConnectorEndEditErrorGapTooBig** | 7 = Current gap between the spot-weld faces is greater than the recommended gap of 3 mm |
| **swsSpotWeldConnectorEndEditErrorHasBeamBody** | 11 = Connector has a beam body |
| **swsSpotWeldConnectorEndEditErrorHasMassElement** | 12 = Connector has mass element |
| **swsSpotWeldConnectorEndEditErrorIndexTooBig** | 14 = Index > number of entities |
| **swsSpotWeldConnectorEndEditErrorInvalidPoints** | 17 = Points are invalid |
| **swsSpotWeldConnectorEndEditErrorNoEntityAtIndex** | 15 = No entity at the specified index |
| **swsSpotWeldConnectorEndEditErrorNullEntity** | 1 = Entity is null |
| **swsSpotWeldConnectorEndEditErrorPlanesShouldTouch** | 6 = Planes should be touching each other |
| **swsSpotWeldConnectorEndEditErrorPositiveStudDiameter** | 9 = Specify a positive value for stud diameter |
| **swsSpotWeldConnectorEndEditErrorSelectDatumPoints** | 8 = Select datum points for spot weld |
| **swsSpotWeldConnectorEndEditErrorSelectFace** | 16 = Select a face |
| **swsSpotWeldConnectorEndEditErrorSelectParallelFaces** | 5 = Select parallel faces |
| **swsSpotWeldConnectorEndEditErrorSpotWeldDiameter** | 13 = Spot-weld diameter should be < 12.5 mm |
| **swsSpotWeldConnectorEndEditErrorStudDiameter** | 10 = Specify a stud diameter < 12.5 mm |
| **swsSpotWeldConnectorEndEditErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)