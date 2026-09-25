<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateRevolutionSurfaceDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateRevolutionSurfaceDLL Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : ICreateRevolutionSurfaceDLL Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ProfileCurve*
:   Pointer to a profile [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) object

*AxisPoint*
:   Array of 3 doubles (x,y,z)

*AxisDirection*
:   Array of 3 doubles (x,y,z)

*ProfileEndPtParams*
:   Array of 2 doubles (uStart,uEnd)

Creates a surface of revolution for this body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateRevolutionSurfaceDLL( _    ByVal ProfileCurve As Curve, _    ByRef AxisPoint As System.Double, _    ByRef AxisDirection As System.Double, _    ByRef ProfileEndPtParams As System.Double _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim ProfileCurve As Curve Dim AxisPoint As System.Double Dim AxisDirection As System.Double Dim ProfileEndPtParams As System.Double Dim value As Surface   value = instance.ICreateRevolutionSurfaceDLL(ProfileCurve, AxisPoint, AxisDirection, ProfileEndPtParams) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreateRevolutionSurfaceDLL(     Curve ProfileCurve,    ref System.double AxisPoint,    ref System.double AxisDirection,    ref System.double ProfileEndPtParams ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreateRevolutionSurfaceDLL(  &   Curve^ ProfileCurve, &   System.double% AxisPoint, &   System.double% AxisDirection, &   System.double% ProfileEndPtParams ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ProfileCurve*
:   Pointer to a profile [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html) object

*AxisPoint*
:   Array of 3 doubles (x,y,z)

*AxisDirection*
:   Array of 3 doubles (x,y,z)

*ProfileEndPtParams*
:   Array of 2 doubles (uStart,uEnd)

#### Return Value

Pointer to a new [surface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html) of revolution

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::ICreateRevolutionSurfaceDLL.

# ![](dotnetimages/collapse.gif)Remarks

Any existing object created by this method is destroyed if you call this method again.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0