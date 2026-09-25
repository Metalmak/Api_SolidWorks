<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MakeOffset.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MakeOffset Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : MakeOffset Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Distance*
:   Distance by which to offset the selected surface body

*Direction*
:   True to offset the selected surface body in the opposite direction, false to offset
    the surface body along the normal

Creates a new temporary body by offsetting the selected surface body by the specified distance and in the specified direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MakeOffset( _    ByVal Distance As System.Double, _    ByVal Direction As System.Boolean _ ) As Body2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Distance As System.Double Dim Direction As System.Boolean Dim value As Body2   value = instance.MakeOffset(Distance, Direction) ``` | |

| C# |  |
| --- | --- |
| ``` Body2 MakeOffset(     System.double Distance,    System.bool Direction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Body2^ MakeOffset(  &   System.double Distance, &   System.bool Direction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Distance*
:   Distance by which to offset the selected surface body

*Direction*
:   True to offset the selected surface body in the opposite direction, false to offset
    the surface body along the normal

#### Return Value

Pointer to the newly created [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::MakeOffset.

# ![](dotnetimages/collapse.gif)Example

[Create Temporary Bodies by Offsetting Surface Body (C#)](Create_Temporary_Bodies_by_Offsetting_Surface_Body_Example_CSharp.htm)

[Create Temporary Bodies by Offsetting Surface Body (VB.NET)](Create_Temporary_Bodies_by_Offsetting_Surface_Body_Example_VBNET.htm)

[Create Temporary Bodies By Offsetting a Surface Body (VBA)](Create_Temporary_Bodies_by_Offsetting_Surface_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only supports surface bodies.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14