<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~IMultiSelectByRay.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMultiSelectByRay Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : IMultiSelectByRay Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PointIn*

*VectorIn*

*RadiusIn*

*TypeWanted*

*Append*

Obsolete. Superseded by [IModelDoc2::IMultiSelectByRay](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~IMultiSelectByRay.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IMultiSelectByRay( _    ByRef PointIn As System.Double, _    ByRef VectorIn As System.Double, _    ByVal RadiusIn As System.Double, _    ByVal TypeWanted As System.Integer, _    ByVal Append As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim PointIn As System.Double Dim VectorIn As System.Double Dim RadiusIn As System.Double Dim TypeWanted As System.Integer Dim Append As System.Boolean Dim value As System.Boolean   value = instance.IMultiSelectByRay(PointIn, VectorIn, RadiusIn, TypeWanted, Append) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IMultiSelectByRay(     ref System.double PointIn,    ref System.double VectorIn,    System.double RadiusIn,    System.int TypeWanted,    System.bool Append ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IMultiSelectByRay(  &   System.double% PointIn, &   System.double% VectorIn, &   System.double RadiusIn, &   System.int TypeWanted, &   System.bool Append ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PointIn*

*VectorIn*

*RadiusIn*

*TypeWanted*

*Append*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::IMultiSelectByRay.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)