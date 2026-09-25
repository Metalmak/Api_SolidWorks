<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~SetUnits.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetUnits Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : SetUnits Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UType*

*FractBase*

*FractDenom*

*SigDigits*

*RoundToFraction*

Obsolete. Superseded by [IModelDoc2::SetUnits](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SetUnits.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetUnits( _    ByVal UType As System.Short, _    ByVal FractBase As System.Short, _    ByVal FractDenom As System.Short, _    ByVal SigDigits As System.Short, _    ByVal RoundToFraction As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim UType As System.Short Dim FractBase As System.Short Dim FractDenom As System.Short Dim SigDigits As System.Short Dim RoundToFraction As System.Boolean   instance.SetUnits(UType, FractBase, FractDenom, SigDigits, RoundToFraction) ``` | |

| C# |  |
| --- | --- |
| ``` void SetUnits(     System.short UType,    System.short FractBase,    System.short FractDenom,    System.short SigDigits,    System.bool RoundToFraction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetUnits(  &   System.short UType, &   System.short FractBase, &   System.short FractDenom, &   System.short SigDigits, &   System.bool RoundToFraction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UType*

*FractBase*

*FractDenom*

*SigDigits*

*RoundToFraction*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::SetUnits.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)