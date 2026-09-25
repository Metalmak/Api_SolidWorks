<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform~ISetData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetData Method (IMathTransform) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMathTransform Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html) : ISetData Method (IMathTransform) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XAxisObjIn*
:   X rotation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*YAxisObjIn*
:   Y rotation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*ZAxisObjIn*
:   Z rotation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*TransformObjIn*
:   Translation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*ScaleValIn*
:   Scale component of the transform

Sets the math vectors and data that describe the transformation matrix.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ISetData( _    ByVal XAxisObjIn As MathVector, _    ByVal YAxisObjIn As MathVector, _    ByVal ZAxisObjIn As MathVector, _    ByVal TransformObjIn As MathVector, _    ByVal ScaleValIn As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMathTransform Dim XAxisObjIn As MathVector Dim YAxisObjIn As MathVector Dim ZAxisObjIn As MathVector Dim TransformObjIn As MathVector Dim ScaleValIn As System.Double   instance.ISetData(XAxisObjIn, YAxisObjIn, ZAxisObjIn, TransformObjIn, ScaleValIn) ``` | |

| C# |  |
| --- | --- |
| ``` void ISetData(     MathVector XAxisObjIn,    MathVector YAxisObjIn,    MathVector ZAxisObjIn,    MathVector TransformObjIn,    System.double ScaleValIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ISetData(  &   MathVector^ XAxisObjIn, &   MathVector^ YAxisObjIn, &   MathVector^ ZAxisObjIn, &   MathVector^ TransformObjIn, &   System.double ScaleValIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XAxisObjIn*
:   X rotation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*YAxisObjIn*
:   Y rotation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*ZAxisObjIn*
:   Z rotation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*TransformObjIn*
:   Translation [math vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html) object of the transform

*ScaleValIn*
:   Scale component of the transform

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MathTransform::ISetData.

# ![](dotnetimages/collapse.gif)See Also

####

[IMathTransform Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html)

[IMathTransform Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform_members.html)

[IMathTransform::SetData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform~SetData.html)

[IMathTransform::GetData2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform~GetData2.html)

[IMathTransform::IGetData2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform~IGetData2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0