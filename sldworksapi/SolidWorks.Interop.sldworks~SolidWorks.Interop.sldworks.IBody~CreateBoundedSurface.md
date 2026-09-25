<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~CreateBoundedSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateBoundedSurface Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : CreateBoundedSurface Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UOpt*

*VOpt*

*UvParams*

Obsolete. Superseded by [IBody2::CreateBoundedSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateBoundedSurface.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateBoundedSurface( _    ByVal UOpt As System.Boolean, _    ByVal VOpt As System.Boolean, _    ByVal UvParams As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim UOpt As System.Boolean Dim VOpt As System.Boolean Dim UvParams As System.Object Dim value As System.Boolean   value = instance.CreateBoundedSurface(UOpt, VOpt, UvParams) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateBoundedSurface(     System.bool UOpt,    System.bool VOpt,    System.object UvParams ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateBoundedSurface(  &   System.bool UOpt, &   System.bool VOpt, &   System.Object^ UvParams ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UOpt*

*VOpt*

*UvParams*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::CreateBoundedSurface.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)