<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform~IGetData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetData Method (IMathTransform) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMathTransform Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html) : IGetData Method (IMathTransform) |

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

Obsolete. See [IMathTransform::IGetData2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform~IGetData2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetData( _    ByRef XAxisObjOut As MathVector, _    ByRef YAxisObjOut As MathVector, _    ByRef ZAxisObjOut As MathVector, _    ByRef TransformObjOut As MathVector, _    ByRef ScaleOut As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMathTransform Dim XAxisObjOut As MathVector Dim YAxisObjOut As MathVector Dim ZAxisObjOut As MathVector Dim TransformObjOut As MathVector Dim ScaleOut As System.Double   instance.IGetData(XAxisObjOut, YAxisObjOut, ZAxisObjOut, TransformObjOut, ScaleOut) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetData(     out MathVector XAxisObjOut,    out MathVector YAxisObjOut,    out MathVector ZAxisObjOut,    out MathVector TransformObjOut,    out System.double ScaleOut ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetData(  &   [Out] MathVector^ XAxisObjOut, &   [Out] MathVector^ YAxisObjOut, &   [Out] MathVector^ ZAxisObjOut, &   [Out] MathVector^ TransformObjOut, &   [Out] System.double ScaleOut ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XAxisObjOut*

*YAxisObjOut*

*ZAxisObjOut*

*TransformObjOut*

*ScaleOut*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MathTransform::IGetData.

# ![](dotnetimages/collapse.gif)See Also

####

[IMathTransform Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html)

[IMathTransform Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform_members.html)