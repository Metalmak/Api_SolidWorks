<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileArc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddProfileArc Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IAddProfileArc Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Center*
:   **Array of 3 doubles (x,y,z)**

*Axis*
:   **Array of 3 doubles (x,y,z)**

*Radius*
:   Arc radius

*StartPoint*
:   **Array of 3 doubles (x,y,z)**

*EndPoint*
:   **Array of 3 doubles (x,y,z)**

Creates an arc profile curve and returns a pointer to that curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddProfileArc( _    ByVal Center As System.Object, _    ByVal Axis As System.Object, _    ByVal Radius As System.Double, _    ByVal StartPoint As System.Object, _    ByVal EndPoint As System.Object _ ) As Curve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Center As System.Object Dim Axis As System.Object Dim Radius As System.Double Dim StartPoint As System.Object Dim EndPoint As System.Object Dim value As Curve   value = instance.IAddProfileArc(Center, Axis, Radius, StartPoint, EndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` Curve IAddProfileArc(     System.object Center,    System.object Axis,    System.double Radius,    System.object StartPoint,    System.object EndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Curve^ IAddProfileArc(  &   System.Object^ Center, &   System.Object^ Axis, &   System.double Radius, &   System.Object^ StartPoint, &   System.Object^ EndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Center*
:   **Array of 3 doubles (x,y,z)**

*Axis*
:   **Array of 3 doubles (x,y,z)**

*Radius*
:   Arc radius

*StartPoint*
:   **Array of 3 doubles (x,y,z)**

*EndPoint*
:   **Array of 3 doubles (x,y,z)**

#### Return Value

[ICurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IAddProfileArc.

# ![](dotnetimages/collapse.gif)Example

[Create Imported Surface Body from Sketch (C#)](Create_Imported_Surface_Body_from_Sketch_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method always creates a full circle.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::AddProfileArc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddProfileArc.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0