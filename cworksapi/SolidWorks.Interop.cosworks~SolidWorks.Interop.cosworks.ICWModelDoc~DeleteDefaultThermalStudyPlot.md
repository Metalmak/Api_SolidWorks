<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteDefaultThermalStudyPlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DeleteDefaultThermalStudyPlot Method (ICWModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : DeleteDefaultThermalStudyPlot Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NResultComponent*
:   Type of thermal study result plot to delete as defined by [swsThermalResultComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsThermalResultComponentTypes_e.html)

*BTransient*
:   True if transient, false if steady state (see **Remarks**)

Deletes the specified default thermal study plot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteDefaultThermalStudyPlot( _    ByVal NResultComponent As System.Integer, _    ByVal BTransient As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NResultComponent As System.Integer Dim BTransient As System.Boolean Dim value As System.Integer   value = instance.DeleteDefaultThermalStudyPlot(NResultComponent, BTransient) ``` | |

| C# |  |
| --- | --- |
| ``` System.int DeleteDefaultThermalStudyPlot(     System.int NResultComponent,    System.bool BTransient ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int DeleteDefaultThermalStudyPlot(  &   System.int NResultComponent, &   System.bool BTransient ) ``` | |

#### Parameters

*NResultComponent*
:   Type of thermal study result plot to delete as defined by [swsThermalResultComponentTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsThermalResultComponentTypes_e.html)

*BTransient*
:   True if transient, false if steady state (see **Remarks**)

#### Return Value

Error code as defined in [swsResultPlotDelete\_ErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotDelete_ErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::DeleteDefaultThermalStudyPlot.

# ![](dotnetimages/collapse.gif)Remarks

If BTransient is true, this plot is for a transient thermal study in which an initial temperature profile is defined for the thermal load.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::AddDefaultThermalStudyPlot Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~AddDefaultThermalStudyPlot.html)

[ICWModelDoc::DeleteAllDefaultThermalStudyPlots Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~DeleteAllDefaultThermalStudyPlots.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0