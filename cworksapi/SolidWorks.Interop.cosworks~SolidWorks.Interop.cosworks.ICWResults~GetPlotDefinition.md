<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDefinition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPlotDefinition Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetPlotDefinition Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SPlotName*
:   Name of plot

*NPlotType*
:   Type of plot as defined in [swsPlotResultTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotResultTypes_e.html)

*NComponentName*
:   Name of plotted component

*BNodal*
:   True if plot is nodal, false if elemental

*BDeformed*
:   True if deformed, false if not

*DScaleFactor*
:   Scale factor for deformation

Gets the definition of the specified plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPlotDefinition( _    ByVal SPlotName As System.String, _    ByRef NPlotType As System.Integer, _    ByRef NComponentName As System.String, _    ByRef BNodal As System.Boolean, _    ByRef BDeformed As System.Boolean, _    ByRef DScaleFactor As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim SPlotName As System.String Dim NPlotType As System.Integer Dim NComponentName As System.String Dim BNodal As System.Boolean Dim BDeformed As System.Boolean Dim DScaleFactor As System.Double Dim value As System.Integer   value = instance.GetPlotDefinition(SPlotName, NPlotType, NComponentName, BNodal, BDeformed, DScaleFactor) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetPlotDefinition(     System.string SPlotName,    out System.int NPlotType,    out System.string NComponentName,    out System.bool BNodal,    out System.bool BDeformed,    out System.double DScaleFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetPlotDefinition(  &   System.String^ SPlotName, &   [Out] System.int NPlotType, &   [Out] System.String^ NComponentName, &   [Out] System.bool BNodal, &   [Out] System.bool BDeformed, &   [Out] System.double DScaleFactor ) ``` | |

#### Parameters

*SPlotName*
:   Name of plot

*NPlotType*
:   Type of plot as defined in [swsPlotResultTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPlotResultTypes_e.html)

*NComponentName*
:   Name of plotted component

*BNodal*
:   True if plot is nodal, false if elemental

*BDeformed*
:   True if deformed, false if not

*DScaleFactor*
:   Scale factor for deformation

#### Return Value

Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetPlotDefinition.

# ![](dotnetimages/collapse.gif)Example

[Create Body From Deformed Shape (VBA)](Create_Body_From_Deformed_Shape_Example_VB.htm)

[Create Body From Deformed Shape (VB.NET)](Create_Body_From_Deformed_Shape_Example_VBNET.htm)

[Create Body From Deformed Shape (C#)](Create_Body_From_Deformed_Shape_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlot.html)

[ICWResults::GetPlotColorOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotColorOptions.html)

[ICWResults::GetPlotCount Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotCount.html)

[ICWResults::GetPlotDisplayOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotDisplayOptions.html)

[ICWResults::GetPlotNames Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotNames.html)

[ICWResults::GetPlotPositionFormatOptions Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotPositionFormatOptions.html)

[ICWResults::GetPlotSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettings.html)

[ICWResults::GetPlotSettingsOptionForHiddenAndExcludedBody Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetPlotSettingsOptionForHiddenAndExcludedBody.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0