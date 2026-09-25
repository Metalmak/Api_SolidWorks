<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~RotateAboutPoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RotateAboutPoint Method (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : RotateAboutPoint Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XAngle*
:   Rotation about the screen X axis

*YAngle*
:   Rotation about the screen Y axis

*Ptx*
:   Center of rotation

*Pty*
:   Center of rotation

*Ptz*
:   Center of rotation

Rotates the model view about the specified point by the specified angles in the directions of the screen X and Y axes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub RotateAboutPoint( _    ByVal XAngle As System.Double, _    ByVal YAngle As System.Double, _    ByVal Ptx As System.Double, _    ByVal Pty As System.Double, _    ByVal Ptz As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim XAngle As System.Double Dim YAngle As System.Double Dim Ptx As System.Double Dim Pty As System.Double Dim Ptz As System.Double   instance.RotateAboutPoint(XAngle, YAngle, Ptx, Pty, Ptz) ``` | |

| C# |  |
| --- | --- |
| ``` void RotateAboutPoint(     System.double XAngle,    System.double YAngle,    System.double Ptx,    System.double Pty,    System.double Ptz ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RotateAboutPoint(  &   System.double XAngle, &   System.double YAngle, &   System.double Ptx, &   System.double Pty, &   System.double Ptz ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XAngle*
:   Rotation about the screen X axis

*YAngle*
:   Rotation about the screen Y axis

*Ptx*
:   Center of rotation

*Pty*
:   Center of rotation

*Ptz*
:   Center of rotation

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::RotateAboutPoint.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

[IModelView::RotateAboutAxis Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~RotateAboutAxis.html)

[IModelView::RotateAboutCenter Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~RotateAboutCenter.html)

[IModelView::RotateAboutPoint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~RotateAboutPoint.html)