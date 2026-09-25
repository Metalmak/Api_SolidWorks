<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~AddDefaultStaticStudyPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddDefaultStaticStudyPlot Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : AddDefaultStaticStudyPlot Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NResultType*
:   Type of static study result to plot as defined by [swsDefaultStaticResultTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDefaultStaticResultTypes_e.html)

*NResultComponent*
:   | If NResultType is swsDefaultStaticResultTypes\_e... | Then NResultComponent is... |
    | --- | --- |
    | swsStaticResultDisplacement | Displacement to plot as defined by [swsStaticResultDisplacementComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultDisplacementComponentTypes_e.html) |
    | swsStaticResultElementalStrain | Elemental strain to plot as defined by [swsStaticResultElementalStrainComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultElementalStrainComponentTypes_e.html) |
    | swsStaticResultElementalStress | Elemental stress to plot as defined by [swsStaticResultElementalStressComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultElementalStressComponentTypes_e.html) |
    | swsStaticResultNodalStrain | Nodal strain to plot as defined by [swsStaticResultNodalStrainComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultNodalStrainComponentTypes_e.html) |
    | swsStaticResultNodalStress | Nodal stress to plot as defined by [swsStaticResultNodalStressComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultNodalStressComponentTypes_e.html) |
    | swsStaticResultBoltPinCheck | Not valid |
    | swsStaticResultFactorOfSafety | Not valid |

Specifies a default static study result plot for the active document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDefaultStaticStudyPlot( _    ByVal NResultType As System.Integer, _    ByVal NResultComponent As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NResultType As System.Integer Dim NResultComponent As System.Integer Dim value As System.Integer   value = instance.AddDefaultStaticStudyPlot(NResultType, NResultComponent) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddDefaultStaticStudyPlot(     System.int NResultType,    System.int NResultComponent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddDefaultStaticStudyPlot(  &   System.int NResultType, &   System.int NResultComponent ) ``` | |

#### Parameters

*NResultType*
:   Type of static study result to plot as defined by [swsDefaultStaticResultTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDefaultStaticResultTypes_e.html)

*NResultComponent*
:   | If NResultType is swsDefaultStaticResultTypes\_e... | Then NResultComponent is... |
    | --- | --- |
    | swsStaticResultDisplacement | Displacement to plot as defined by [swsStaticResultDisplacementComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultDisplacementComponentTypes_e.html) |
    | swsStaticResultElementalStrain | Elemental strain to plot as defined by [swsStaticResultElementalStrainComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultElementalStrainComponentTypes_e.html) |
    | swsStaticResultElementalStress | Elemental stress to plot as defined by [swsStaticResultElementalStressComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultElementalStressComponentTypes_e.html) |
    | swsStaticResultNodalStrain | Nodal strain to plot as defined by [swsStaticResultNodalStrainComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultNodalStrainComponentTypes_e.html) |
    | swsStaticResultNodalStress | Nodal stress to plot as defined by [swsStaticResultNodalStressComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStaticResultNodalStressComponentTypes_e.html) |
    | swsStaticResultBoltPinCheck | Not valid |
    | swsStaticResultFactorOfSafety | Not valid |

#### Return Value

Error code as defined by [swsAddDefaultStaticStudyPlotResultError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAddDefaultStaticStudyPlotResultError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::AddDefaultStaticStudyPlot.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::DeleteAllDefaultStaticStudyPlots Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteAllDefaultStaticStudyPlots.html)

[ICWModelDoc::DeleteDefaultStaticStudyPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteDefaultStaticStudyPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0