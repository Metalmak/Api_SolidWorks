<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour~DisplayString.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| DisplayString Method (ISwColorContour) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwColorContour Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour.html) : DisplayString Method (ISwColorContour) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Value*
:   Value associated with the vertex for which to display the string

Obsolete. Superseded by [ISwColorContour1::DisplayString](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwColorContour1~DisplayString.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DisplayString( _    ByVal Value As System.Double _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwColorContour Dim Value As System.Double Dim value As System.String   value = instance.DisplayString(Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.string DisplayString(     System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ DisplayString(  &   System.double Value ) ``` | |

#### Parameters

*Value*
:   Value associated with the vertex for which to display the string

#### Return Value

String to display for the value associated with the vertex

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwColorContour::DisplayString.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwColorContour Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour.html)

[ISwColorContour Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0