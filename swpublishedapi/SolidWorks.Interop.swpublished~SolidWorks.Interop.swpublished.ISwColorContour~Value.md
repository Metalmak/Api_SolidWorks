<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour~Value.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| Value Method (ISwColorContour) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwColorContour Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour.html) : Value Method (ISwColorContour) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*face*
:   Face on the model

*vertexCoords*
:   Array of vertex coordinates (x, y, z) to which to color

*normalCoords*
:   Array of normal coordinates (x, y, z) to which to color

*Value*
:   Value defined by the add-in to display

Obsolete. Superseded by [ISwColorContour1::Value](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwColorContour1~Value.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Value( _    ByVal face As System.Object, _    ByRef vertexCoords As System.Single, _    ByRef normalCoords As System.Single, _    ByRef Value As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwColorContour Dim face As System.Object Dim vertexCoords As System.Single Dim normalCoords As System.Single Dim Value As System.Double Dim value As System.Integer   value = instance.Value(face, vertexCoords, normalCoords, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Value(     System.object face,    ref System.float vertexCoords,    ref System.float normalCoords,    out System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Value(  &   System.Object^ face, &   System.float% vertexCoords, &   System.float% normalCoords, &   [Out] System.double Value ) ``` | |

#### Parameters

*face*
:   Face on the model

*vertexCoords*
:   Array of vertex coordinates (x, y, z) to which to color

*normalCoords*
:   Array of normal coordinates (x, y, z) to which to color

*Value*
:   Value defined by the add-in to display

#### Return Value

COLORREF value that represents value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwColorContour::Value.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwColorContour Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour.html)

[ISwColorContour Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0