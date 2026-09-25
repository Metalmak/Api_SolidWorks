<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Display3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Display3 Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : Display3 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Component*
:   Part or component where the temporary body exists (see **Remarks**)

*Color*
:   COLORREF value (see **Remarks**)

*Option*
:   Selection state of temporary body as defined by swTempBodySelectOptions\_e (see **Remarks**)

Displays this temporary body in the context of the specified part or component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Display3( _    ByVal Component As System.Object, _    ByVal Color As System.Integer, _    ByVal Option As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Component As System.Object Dim Color As System.Integer Dim Option As System.Integer Dim value As System.Integer   value = instance.Display3(Component, Color, Option) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Display3(     System.object Component,    System.int Color,    System.int Option ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Display3(  &   System.Object^ Component, &   System.int Color, &   System.int Option ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Component*
:   Part or component where the temporary body exists (see **Remarks**)

*Color*
:   COLORREF value (see **Remarks**)

*Option*
:   Selection state of temporary body as defined by swTempBodySelectOptions\_e (see **Remarks**)

#### Return Value

* 0 = Success

  * 1 = Failed because this body is not a temporary body

    * 2 = Invalid component

      * 3 = Not a part instance

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::Display3.

# ![](dotnetimages/collapse.gif)Example

[Create Loft Body (VB.NET)](Create_Loft_Body_Example_VBNET.htm)

[Create Loft Body (VBA)](Create_Loft_Body_Example_VB.htm)

[Create Loft Body (C#)](Create_Loft_Body_Example_CSharp.htm)

[Display Temporary Body (C#)](Display_Temporary_Body_Example_CSharp.htm)

[Display Temporary Body (VB.NET)](Display_Temporary_Body_Example_VBNET.htm)

[Display Temporary Body (VBA)](Display_Temporary_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Is valid only for temporary bodies. To determine whether a body is temporary, use [IBody2::IsTemporaryBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsTemporaryBody.html).* Applies Color to this temporary body in the graphics area, effectively selecting it.

You can also use [IBody2::MaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MaterialPropertyValues2.html) to change the appearance of this temporary body.

Component cannot be in a subassembly.

Specifying Option with swTempBodySelectable sets the blocking state to swBlockingStates\_e.swModifyBlock. Unset the blocking state by calling [IBody2::Hide](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Hide.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15