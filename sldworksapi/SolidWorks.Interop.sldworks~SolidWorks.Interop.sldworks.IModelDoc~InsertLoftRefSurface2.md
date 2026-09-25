<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertLoftRefSurface2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertLoftRefSurface2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertLoftRefSurface2 Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Closed*

*KeepTangency*

*ForceNonRational*

*TessToleranceFactor*

*StartMatchingType*

*EndMatchingType*

Obsolete. Superseded by [IModelDoc2::InsertLoftRefSurface2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertLoftRefSurface2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertLoftRefSurface2( _    ByVal Closed As System.Boolean, _    ByVal KeepTangency As System.Boolean, _    ByVal ForceNonRational As System.Boolean, _    ByVal TessToleranceFactor As System.Double, _    ByVal StartMatchingType As System.Short, _    ByVal EndMatchingType As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Closed As System.Boolean Dim KeepTangency As System.Boolean Dim ForceNonRational As System.Boolean Dim TessToleranceFactor As System.Double Dim StartMatchingType As System.Short Dim EndMatchingType As System.Short   instance.InsertLoftRefSurface2(Closed, KeepTangency, ForceNonRational, TessToleranceFactor, StartMatchingType, EndMatchingType) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertLoftRefSurface2(     System.bool Closed,    System.bool KeepTangency,    System.bool ForceNonRational,    System.double TessToleranceFactor,    System.short StartMatchingType,    System.short EndMatchingType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertLoftRefSurface2(  &   System.bool Closed, &   System.bool KeepTangency, &   System.bool ForceNonRational, &   System.double TessToleranceFactor, &   System.short StartMatchingType, &   System.short EndMatchingType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Closed*

*KeepTangency*

*ForceNonRational*

*TessToleranceFactor*

*StartMatchingType*

*EndMatchingType*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertLoftRefSurface2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)