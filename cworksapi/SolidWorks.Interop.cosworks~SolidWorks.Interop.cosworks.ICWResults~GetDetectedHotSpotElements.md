<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDetectedHotSpotElements.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetDetectedHotSpotElements Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetDetectedHotSpotElements Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RetVal*
:   Array of stress hot spot elements

Gets the stress hot spot elements.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDetectedHotSpotElements( _    ByRef RetVal As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim RetVal As System.Object Dim value As System.Integer   value = instance.GetDetectedHotSpotElements(RetVal) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetDetectedHotSpotElements(     out System.object RetVal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetDetectedHotSpotElements(  &   [Out] System.Object^ RetVal ) ``` | |

#### Parameters

*RetVal*
:   Array of stress hot spot elements

#### Return Value

1 if successful, 0 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetDetectedHotSpotElements.

# ![](dotnetimages/collapse.gif)Example

See the [ICWStaticStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call [ICWResults::RunStressHotSpotDiagnostics](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~RunStressHotSpotDiagnostics.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::CreateStressHotSpotPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateStressHotSpotPlot.html)

[ICWResults::GetDetectedHotSpotNodes Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDetectedHotSpotNodes.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0