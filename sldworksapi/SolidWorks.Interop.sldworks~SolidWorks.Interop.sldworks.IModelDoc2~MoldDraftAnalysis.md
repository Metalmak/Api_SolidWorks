<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~MoldDraftAnalysis.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MoldDraftAnalysis Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : MoldDraftAnalysis Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*
:   Reference draft angle

*Options*
:   Analysis options as defined in swDraftAnalysisOptions\_e

*Colors*
:   Array of 4 colors (positive draft, negative draft, no draft, straddled faces)

*Shows*
:   Show each draft type as defined in swDraftAnalysisShow\_e

Performs a mold draft analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub MoldDraftAnalysis( _    ByVal Angle As System.Double, _    ByVal Options As System.Integer, _    ByVal Colors As System.Object, _    ByVal Shows As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Angle As System.Double Dim Options As System.Integer Dim Colors As System.Object Dim Shows As System.Integer   instance.MoldDraftAnalysis(Angle, Options, Colors, Shows) ``` | |

| C# |  |
| --- | --- |
| ``` void MoldDraftAnalysis(     System.double Angle,    System.int Options,    System.object Colors,    System.int Shows ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void MoldDraftAnalysis(  &   System.double Angle, &   System.int Options, &   System.Object^ Colors, &   System.int Shows ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*
:   Reference draft angle

*Options*
:   Analysis options as defined in swDraftAnalysisOptions\_e

*Colors*
:   Array of 4 colors (positive draft, negative draft, no draft, straddled faces)

*Shows*
:   Show each draft type as defined in swDraftAnalysisShow\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::MoldDraftAnalysis.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0