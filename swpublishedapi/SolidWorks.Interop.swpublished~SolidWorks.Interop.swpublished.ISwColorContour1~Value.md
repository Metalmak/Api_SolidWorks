<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1~Value.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| Value Method (ISwColorContour1) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwColorContour1 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1.html) : Value Method (ISwColorContour1) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*face*
:   Face to color

*vertex\_x*
:   X coordinate of vertex to color

*vertex\_y*
:   Y coordinate of vertex to color

*vertex\_z*
:   Z coordinate of vertex to color

*normal\_x*
:   :   X coordinate of normal to color

*normal\_y*
:   Y coordinate of normal to color

*normal\_z*
:   Z coordinate of normal to color

*Value*
:   :   Function of the specified face or coordinates of the model (see **Remarks**)

Gets the value that is associated with the specified location on the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Value( _    ByVal face As System.Object, _    ByVal vertex_x As System.Single, _    ByVal vertex_y As System.Single, _    ByVal vertex_z As System.Single, _    ByVal normal_x As System.Single, _    ByVal normal_y As System.Single, _    ByVal normal_z As System.Single, _    ByRef Value As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwColorContour1 Dim face As System.Object Dim vertex_x As System.Single Dim vertex_y As System.Single Dim vertex_z As System.Single Dim normal_x As System.Single Dim normal_y As System.Single Dim normal_z As System.Single Dim Value As System.Double Dim value As System.Integer   value = instance.Value(face, vertex_x, vertex_y, vertex_z, normal_x, normal_y, normal_z, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Value(     System.object face,    System.float vertex_x,    System.float vertex_y,    System.float vertex_z,    System.float normal_x,    System.float normal_y,    System.float normal_z,    out System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Value(  &   System.Object^ face, &   System.float vertex_x, &   System.float vertex_y, &   System.float vertex_z, &   System.float normal_x, &   System.float normal_y, &   System.float normal_z, &   [Out] System.double Value ) ``` | |

#### Parameters

*face*
:   Face to color

*vertex\_x*
:   X coordinate of vertex to color

*vertex\_y*
:   Y coordinate of vertex to color

*vertex\_z*
:   Z coordinate of vertex to color

*normal\_x*
:   :   X coordinate of normal to color

*normal\_y*
:   Y coordinate of normal to color

*normal\_z*
:   Z coordinate of normal to color

*Value*
:   :   Function of the specified face or coordinates of the model (see **Remarks**)

#### Return Value

Not used

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwColorContour1::Value.

# ![](dotnetimages/collapse.gif)Example

[Custom Colorize a Model Example (C#)](Custom_Colorize_a_Model_Example_CSharp.htm)

[Custom Colorize a Model Example (VB.NET)](Custom_Colorize_a_Model_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

When you implement this method, you need to populate the Value output parameter. Value can be a function of the specified coordinates or the properties of the face. By default Value is the input parameter for [ISwColorContour1::Color](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwColorContour1~Color.html) and [ISwColorContour1::DisplayString](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwColorContour1~DisplayString.html).

In VB.NET implementations, you need to change the name of the Value output parameter to avoid a compiler error. When you change the name, use the same name for the input parameters of your ISwColorContour1::Color and ISwColorContour1::DisplayString implementations.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwColorContour1 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1.html)

[ISwColorContour1 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 SP05, Revision Number 18.5 and SOLIDWORKS 2011 SP01, Revision Number 19.1