<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~Translation3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Translation3 Property (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : Translation3 Property (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the model view translation vector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Translation3 As MathVector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim value As MathVector   instance.Translation3 = value   value = instance.Translation3 ``` | |

| C# |  |
| --- | --- |
| ``` MathVector Translation3 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property MathVector^ Translation3 {    MathVector^ get();    void set ( &   MathVector^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

[Model view translation vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::Translation3.

# ![](dotnetimages/collapse.gif)Remarks

When modifying a model view transform, you must use [IModelView::Orientation3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~Orientation3.html) and IModelView::Translation3. For example:

...

Dim xyzOrigin As SldWorks.MathPoint

dPoint(0) = 0#: dPoint(1) = 0#: dPoint(2) = 0#

Set xyzOrigin = swMathUtil.CreatePoint((dPoint))

Set swVectorZ = swVectorZ.Scale(-1)

Set swMathTrans = swMathUtil.ComposeTransform(swVectorX, swVectorY, swVectorZ, xyzOrigin.ConvertToVector, 1#)

Set swMathTrans = swMathTrans.Inverse

Set swModelView = swModel.ActiveView

Set swViewTrans = swModelView.Orientation3

swModelView.Orientation3 = swMathTrans

Dim u As Double

u = swModelView.Scale2

Set swMathPoint = swVectorT.ConvertToPoint

Set swMathPoint = swMathPoint.Scale(-1 \* u)

Set swMathPoint = swMathPoint.MultiplyTransform(swMathTrans)

swModelView.Translation3 = swMathPoint.ConvertToVector

...

Also, check the vectors by looking at the triad in the model view.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP2, Revision Number 10.2