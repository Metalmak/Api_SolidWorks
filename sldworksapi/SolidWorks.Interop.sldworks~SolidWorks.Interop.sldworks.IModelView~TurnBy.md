<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~TurnBy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| TurnBy Method (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : TurnBy Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XAngle*
:   Angle by which to rotate the camera about its x axis

*YAngle*
:   Angle by which to rotate the camera about its y axis

Rotates the camera by the specified angles about the camera's x and y axes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub TurnBy( _    ByVal XAngle As System.Double, _    ByVal YAngle As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim XAngle As System.Double Dim YAngle As System.Double   instance.TurnBy(XAngle, YAngle) ``` | |

| C# |  |
| --- | --- |
| ``` void TurnBy(     System.double XAngle,    System.double YAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void TurnBy(  &   System.double XAngle, &   System.double YAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XAngle*
:   Angle by which to rotate the camera about its x axis

*YAngle*
:   Angle by which to rotate the camera about its y axis

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::TurnBy.

# ![](dotnetimages/collapse.gif)Remarks

The model view must have an active camera.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

[IModelView::Camera Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~Camera.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0