<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteDefaultDropTestStudyPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DeleteDefaultDropTestStudyPlot Method (ICWModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : DeleteDefaultDropTestStudyPlot Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NResultType*
:   Type of drop test study result plot to delete as defined by [swsDropTestStudyResultType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDropTestStudyResultType_e.html)

*NResultComponent*
:   | If NResultType is swsDropTestStudyResultType\_e... | Then NResultComponent is... |
    | --- | --- |
    | swsDropTestResultDisplacement | Displacement component to plot as defined by [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html) |
    | swsDropTestResultElementalStrain | Strain component to plot as defined by [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html) |
    | swsDropTestResultElementalStress or swsDropTestResultNodalStress | Stress component to plot as defined by [swsStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStressComponent_e.html) |

Deletes the specified default drop test study plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteDefaultDropTestStudyPlot( _    ByVal NResultType As System.Integer, _    ByVal NResultComponent As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NResultType As System.Integer Dim NResultComponent As System.Integer Dim value As System.Integer   value = instance.DeleteDefaultDropTestStudyPlot(NResultType, NResultComponent) ``` | |

| C# |  |
| --- | --- |
| ``` System.int DeleteDefaultDropTestStudyPlot(     System.int NResultType,    System.int NResultComponent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int DeleteDefaultDropTestStudyPlot(  &   System.int NResultType, &   System.int NResultComponent ) ``` | |

#### Parameters

*NResultType*
:   Type of drop test study result plot to delete as defined by [swsDropTestStudyResultType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDropTestStudyResultType_e.html)

*NResultComponent*
:   | If NResultType is swsDropTestStudyResultType\_e... | Then NResultComponent is... |
    | --- | --- |
    | swsDropTestResultDisplacement | Displacement component to plot as defined by [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html) |
    | swsDropTestResultElementalStrain | Strain component to plot as defined by [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html) |
    | swsDropTestResultElementalStress or swsDropTestResultNodalStress | Stress component to plot as defined by [swsStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStressComponent_e.html) |

#### Return Value

Error code as defined in [swsResultPlotDelete\_ErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotDelete_ErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::DeleteDefaultDropTestStudyPlot.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::AddDefaultDropTestStudyPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~AddDefaultDropTestStudyPlot.html)

[ICWModelDoc::DeleteAllDefaultDropTestStudyPlots Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteAllDefaultDropTestStudyPlots.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0