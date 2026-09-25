<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1~Color.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| Color Method (ISwColorContour1) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwColorContour1 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1.html) : Color Method (ISwColorContour1) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Value*
:   Value that is associated with a location on the model (see **Remarks**)

Gets the color for the specified location on the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Color( _    ByVal Value As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwColorContour1 Dim Value As System.Double Dim value As System.Integer   value = instance.Color(Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Color(     System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Color(  &   System.double Value ) ``` | |

#### Parameters

*Value*
:   Value that is associated with a location on the model (see **Remarks**)

#### Return Value

COLORREF value corresponding to the specified Value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwColorContour1::Color.

# ![](dotnetimages/collapse.gif)Example

[Custom Colorize a Model Example (C#)](Custom_Colorize_a_Model_Example_CSharp.htm)

[Custom Colorize a Model Example (VB.NET)](Custom_Colorize_a_Model_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

When you implement this method, you can return different colors for different locations of the model.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwColorContour1 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1.html)

[ISwColorContour1 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1_members.html)

[ISwColorContour1::Value Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1~Value.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 SP05, Revision Number 18.5 and SOLIDWORKS 2011 SP01, Revision Number 19.1