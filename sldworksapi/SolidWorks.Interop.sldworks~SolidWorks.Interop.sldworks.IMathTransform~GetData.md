<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform~GetData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetData Method (IMathTransform) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMathTransform Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html) : GetData Method (IMathTransform) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XAxisObjOut*

*YAxisObjOut*

*ZAxisObjOut*

*TransformObjOut*

*ScaleOut*

Obsolete. See [IMathTransform::GetData2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform~GetData2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetData( _    ByRef XAxisObjOut As System.Object, _    ByRef YAxisObjOut As System.Object, _    ByRef ZAxisObjOut As System.Object, _    ByRef TransformObjOut As System.Object, _    ByRef ScaleOut As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMathTransform Dim XAxisObjOut As System.Object Dim YAxisObjOut As System.Object Dim ZAxisObjOut As System.Object Dim TransformObjOut As System.Object Dim ScaleOut As System.Double   instance.GetData(XAxisObjOut, YAxisObjOut, ZAxisObjOut, TransformObjOut, ScaleOut) ``` | |

| C# |  |
| --- | --- |
| ``` void GetData(     out System.object XAxisObjOut,    out System.object YAxisObjOut,    out System.object ZAxisObjOut,    out System.object TransformObjOut,    out System.double ScaleOut ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetData(  &   [Out] System.Object^ XAxisObjOut, &   [Out] System.Object^ YAxisObjOut, &   [Out] System.Object^ ZAxisObjOut, &   [Out] System.Object^ TransformObjOut, &   [Out] System.double ScaleOut ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XAxisObjOut*

*YAxisObjOut*

*ZAxisObjOut*

*TransformObjOut*

*ScaleOut*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MathTransform::GetData.

# ![](dotnetimages/collapse.gif)See Also

####

[IMathTransform Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html)

[IMathTransform Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform_members.html)