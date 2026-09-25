<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility~ICreateTransformRotateAxis.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateTransformRotateAxis Method (IMathUtility) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMathUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility.html) : ICreateTransformRotateAxis Method (IMathUtility) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PointObjIn*
:   Center [point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html) of the axis of the transform

*VectorObjIn*
:   Axis [vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) of the transform

*Angle*
:   Angle of rotation about the X axis vector

Creates a new math transform matrix that represents the rotation by an angle about a vector positioned at a point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateTransformRotateAxis( _    ByVal PointObjIn As MathPoint, _    ByVal VectorObjIn As MathVector, _    ByVal Angle As System.Double _ ) As MathTransform ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMathUtility Dim PointObjIn As MathPoint Dim VectorObjIn As MathVector Dim Angle As System.Double Dim value As MathTransform   value = instance.ICreateTransformRotateAxis(PointObjIn, VectorObjIn, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` MathTransform ICreateTransformRotateAxis(     MathPoint PointObjIn,    MathVector VectorObjIn,    System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` MathTransform^ ICreateTransformRotateAxis(  &   MathPoint^ PointObjIn, &   MathVector^ VectorObjIn, &   System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PointObjIn*
:   Center [point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html) of the axis of the transform

*VectorObjIn*
:   Axis [vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) of the transform

*Angle*
:   Angle of rotation about the X axis vector

#### Return Value

Newly created [math transform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html) or NULL if the operation fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MathUtility::ICreateTransformRotateAxis.

# ![](dotnetimages/collapse.gif)See Also

####

[IMathUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility.html)

[IMathUtility Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility_members.html)

[IMathUtility::CreateTransformRotateAxis Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility~CreateTransformRotateAxis.html)

[IMathUtility::ComposeTransform Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility~ComposeTransform.html)

[IMathUtility::CreateTransform Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility~CreateTransform.html)

[IMathUtility::ICreateTransform Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathUtility~ICreateTransform.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0