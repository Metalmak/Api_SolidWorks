<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~RotateAboutAxis.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RotateAboutAxis Method (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : RotateAboutAxis Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*
:   Angle of rotation

*Ptx*
:   Center of rotation

*Pty*
:   Center of rotation

*Ptz*
:   Center of rotation

*AxisVecX*
:   Direction of axis of rotation

*AxisVecY*
:   Direction of axis of rotation

*AxisVecZ*
:   Direction of axis of rotation

Rotates the model view about a point, by an angle in the specified direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub RotateAboutAxis( _    ByVal Angle As System.Double, _    ByVal Ptx As System.Double, _    ByVal Pty As System.Double, _    ByVal Ptz As System.Double, _    ByVal AxisVecX As System.Double, _    ByVal AxisVecY As System.Double, _    ByVal AxisVecZ As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim Angle As System.Double Dim Ptx As System.Double Dim Pty As System.Double Dim Ptz As System.Double Dim AxisVecX As System.Double Dim AxisVecY As System.Double Dim AxisVecZ As System.Double   instance.RotateAboutAxis(Angle, Ptx, Pty, Ptz, AxisVecX, AxisVecY, AxisVecZ) ``` | |

| C# |  |
| --- | --- |
| ``` void RotateAboutAxis(     System.double Angle,    System.double Ptx,    System.double Pty,    System.double Ptz,    System.double AxisVecX,    System.double AxisVecY,    System.double AxisVecZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RotateAboutAxis(  &   System.double Angle, &   System.double Ptx, &   System.double Pty, &   System.double Ptz, &   System.double AxisVecX, &   System.double AxisVecY, &   System.double AxisVecZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*
:   Angle of rotation

*Ptx*
:   Center of rotation

*Pty*
:   Center of rotation

*Ptz*
:   Center of rotation

*AxisVecX*
:   Direction of axis of rotation

*AxisVecY*
:   Direction of axis of rotation

*AxisVecZ*
:   Direction of axis of rotation

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::RotateAboutAxis.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

[IModelView::RotateAboutCenter Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~RotateAboutCenter.html)

[IModelView::RotateAboutPoint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~RotateAboutPoint.html)

[IModelView::StartDynamics Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~StartDynamics.html)