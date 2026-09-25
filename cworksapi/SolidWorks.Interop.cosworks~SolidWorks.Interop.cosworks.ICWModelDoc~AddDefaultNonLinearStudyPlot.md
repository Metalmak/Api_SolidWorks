<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~AddDefaultNonLinearStudyPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddDefaultNonLinearStudyPlot Method (ICWModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : AddDefaultNonLinearStudyPlot Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NResultType*
:   Default nonlinear study result plot types as defined in [swsNonlinearStudyResultTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonlinearStudyResultTypes_e.html)

*NResultComponent*
:   | If NResultType is ... | Then NResultComponent is... |
    | --- | --- |
    | 0 = Nodal stress or 1 = Elemental stress | Stress component to plot as defined by [swsStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStressComponent_e.html) |
    | 2 = Displacement | Displacement component to plot as defined by [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html) |
    | 3 = Nodal strain or 4 = Elemental strain | Strain component to plot as defined by [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html) |

Specifies a default nonlinear study result plot for the active document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDefaultNonLinearStudyPlot( _    ByVal NResultType As System.Integer, _    ByVal NResultComponent As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NResultType As System.Integer Dim NResultComponent As System.Integer Dim value As System.Integer   value = instance.AddDefaultNonLinearStudyPlot(NResultType, NResultComponent) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddDefaultNonLinearStudyPlot(     System.int NResultType,    System.int NResultComponent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddDefaultNonLinearStudyPlot(  &   System.int NResultType, &   System.int NResultComponent ) ``` | |

#### Parameters

*NResultType*
:   Default nonlinear study result plot types as defined in [swsNonlinearStudyResultTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonlinearStudyResultTypes_e.html)

*NResultComponent*
:   | If NResultType is ... | Then NResultComponent is... |
    | --- | --- |
    | 0 = Nodal stress or 1 = Elemental stress | Stress component to plot as defined by [swsStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStressComponent_e.html) |
    | 2 = Displacement | Displacement component to plot as defined by [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html) |
    | 3 = Nodal strain or 4 = Elemental strain | Strain component to plot as defined by [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html) |

#### Return Value

Error code as defined by [swsAddDefaultNonLinearStudyPlotResultError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAddDefaultNonLinearStudyPlotResultError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::AddDefaultNonLinearStudyPlot.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::DeleteAllDefaultNonLinearStudyPlots Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteAllDefaultNonLinearStudyPlots.html)

[ICWModelDoc::DeleteDefaultNonLinearStudyPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteDefaultNonLinearStudyPlot.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0