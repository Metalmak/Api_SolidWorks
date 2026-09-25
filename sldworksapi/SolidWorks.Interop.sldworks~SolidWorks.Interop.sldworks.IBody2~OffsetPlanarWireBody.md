<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~OffsetPlanarWireBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| OffsetPlanarWireBody Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : OffsetPlanarWireBody Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Distance*
:   Distance by which to offset the planar wire body

*Normal*
:   Plane normal

*Option*
:   How to fill the gap between edges as defined in swOffsetPlanarWireBodyOptions\_e

Offsets a planar wire body in the normal plane by the specified distance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OffsetPlanarWireBody( _    ByVal Distance As System.Double, _    ByVal Normal As MathVector, _    ByVal Option As System.Integer _ ) As Body2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Distance As System.Double Dim Normal As MathVector Dim Option As System.Integer Dim value As Body2   value = instance.OffsetPlanarWireBody(Distance, Normal, Option) ``` | |

| C# |  |
| --- | --- |
| ``` Body2 OffsetPlanarWireBody(     System.double Distance,    MathVector Normal,    System.int Option ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Body2^ OffsetPlanarWireBody(  &   System.double Distance, &   MathVector^ Normal, &   System.int Option ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Distance*
:   Distance by which to offset the planar wire body

*Normal*
:   Plane normal

*Option*
:   How to fill the gap between edges as defined in swOffsetPlanarWireBodyOptions\_e

#### Return Value

Pointer to the [IBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::OffsetPlanarWireBody.

# ![](dotnetimages/collapse.gif)Remarks

The offset direction is determined by the direction of the first edge and the normal. For example, imagine that you are standing on the plane with normal pointing upwards and you are looking along the first edge, then the offset is to your right.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)