<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileArcDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddProfileArcDLL Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IAddProfileArcDLL Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*
:   Pointer to an array of 3 doubles (x,y,z)

*Axis*
:   Pointer to an array of 3 doubles (x,y,z)

*Radius*
:   Radius of the arc

*StartPoint*
:   Pointer to an array of 3 doubles (x,y,z)

*EndPoint*
:   Pointer to an array of 3 doubles (x,y,z)

Adds a profile arc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddProfileArcDLL( _    ByRef Center As System.Double, _    ByRef Axis As System.Double, _    ByVal Radius As System.Double, _    ByRef StartPoint As System.Double, _    ByRef EndPoint As System.Double _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Center As System.Double Dim Axis As System.Double Dim Radius As System.Double Dim StartPoint As System.Double Dim EndPoint As System.Double Dim value As Curve   value = instance.IAddProfileArcDLL(Center, Axis, Radius, StartPoint, EndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` Curve IAddProfileArcDLL(     ref System.double Center,    ref System.double Axis,    System.double Radius,    ref System.double StartPoint,    ref System.double EndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ IAddProfileArcDLL(  &   System.double% Center, &   System.double% Axis, &   System.double Radius, &   System.double% StartPoint, &   System.double% EndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*
:   Pointer to an array of 3 doubles (x,y,z)

*Axis*
:   Pointer to an array of 3 doubles (x,y,z)

*Radius*
:   Radius of the arc

*StartPoint*
:   Pointer to an array of 3 doubles (x,y,z)

*EndPoint*
:   Pointer to an array of 3 doubles (x,y,z)

#### Return Value

Pointer to the arc profile [curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IAddProfileArcDLL.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision 10.0