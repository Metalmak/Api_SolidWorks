<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker~GetInferencePoints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| GetInferencePoints Method (ISwAddinBroker) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwAddinBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker.html) : GetInferencePoints Method (ISwAddinBroker) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pDoc*
:   SOLIDWORKS document

*SelPosX*
:   x coordinate in screen space

*SelPosY*
:   y coordinate in screen space

*Tolerance*
:   Distance within model space that inference points can exist

*Option*
:   Options as defined in swPointInferenceBrokerOption\_e

*InferPoints*
:   Array of doubles; each inference point returns its x,y,z coordinates

Gets one or more inference points from an add-in.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetInferencePoints( _    ByVal pDoc As System.Object, _    ByVal SelPosX As System.Integer, _    ByVal SelPosY As System.Integer, _    ByVal Tolerance As System.Double, _    ByVal Option As System.Integer, _    ByRef InferPoints As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwAddinBroker Dim pDoc As System.Object Dim SelPosX As System.Integer Dim SelPosY As System.Integer Dim Tolerance As System.Double Dim Option As System.Integer Dim InferPoints As System.Object   instance.GetInferencePoints(pDoc, SelPosX, SelPosY, Tolerance, Option, InferPoints) ``` | |

| C# |  |
| --- | --- |
| ``` void GetInferencePoints(     System.object pDoc,    System.int SelPosX,    System.int SelPosY,    System.double Tolerance,    System.int Option,    out System.object InferPoints ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetInferencePoints(  &   System.Object^ pDoc, &   System.int SelPosX, &   System.int SelPosY, &   System.double Tolerance, &   System.int Option, &   [Out] System.Object^ InferPoints ) ``` | |

#### Parameters

*pDoc*
:   SOLIDWORKS document

*SelPosX*
:   x coordinate in screen space

*SelPosY*
:   y coordinate in screen space

*Tolerance*
:   Distance within model space that inference points can exist

*Option*
:   Options as defined in swPointInferenceBrokerOption\_e

*InferPoints*
:   Array of doubles; each inference point returns its x,y,z coordinates

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwAddinBroker::GetInferencePoints.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwAddinBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker.html)

[ISwAddinBroker Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0