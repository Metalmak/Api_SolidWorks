<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteDefaultNonLinearStudyPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DeleteDefaultNonLinearStudyPlot Method (ICWModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : DeleteDefaultNonLinearStudyPlot Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NResultType*
:   Type of nonlinear study result plot to delete as defined in [swsNonlinearStudyResultTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonlinearStudyResultTypes_e.html)

*NResultComponent*
:   | If NResultType is ... | Then NResultComponent is... |
    | --- | --- |
    | 0 = Nodal stress or 1 = Elemental stress | Stress component to plot as defined by [swsStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStressComponent_e.html) |
    | 2 = Displacement | Displacement component to plot as defined by [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html) |
    | 3 = Nodal strain or 4 = Elemental strain | Strain component to plot as defined by [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html) |

Deletes the specified default nonlinear study plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteDefaultNonLinearStudyPlot( _    ByVal NResultType As System.Integer, _    ByVal NResultComponent As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NResultType As System.Integer Dim NResultComponent As System.Integer Dim value As System.Integer   value = instance.DeleteDefaultNonLinearStudyPlot(NResultType, NResultComponent) ``` | |

| C# |  |
| --- | --- |
| ``` System.int DeleteDefaultNonLinearStudyPlot(     System.int NResultType,    System.int NResultComponent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int DeleteDefaultNonLinearStudyPlot(  &   System.int NResultType, &   System.int NResultComponent ) ``` | |

#### Parameters

*NResultType*
:   Type of nonlinear study result plot to delete as defined in [swsNonlinearStudyResultTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNonlinearStudyResultTypes_e.html)

*NResultComponent*
:   | If NResultType is ... | Then NResultComponent is... |
    | --- | --- |
    | 0 = Nodal stress or 1 = Elemental stress | Stress component to plot as defined by [swsStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStressComponent_e.html) |
    | 2 = Displacement | Displacement component to plot as defined by [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html) |
    | 3 = Nodal strain or 4 = Elemental strain | Strain component to plot as defined by [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html) |

#### Return Value

Error code as defined in [swsResultPlotDelete\_ErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotDelete_ErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::DeleteDefaultNonLinearStudyPlot.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::AddDefaultNonLinearStudyPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~AddDefaultNonLinearStudyPlot.html)

[ICWModelDoc::DeleteAllDefaultNonLinearStudyPlots Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteAllDefaultNonLinearStudyPlots.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0