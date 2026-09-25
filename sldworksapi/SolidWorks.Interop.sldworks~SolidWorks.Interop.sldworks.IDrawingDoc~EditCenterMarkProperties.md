<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~EditCenterMarkProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditCenterMarkProperties Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : EditCenterMarkProperties Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*
:   New angle of the center mark

*Size*
:   New size of the center mark

*Lines*
:   True displays the center mark lines, false displays the plus sign (+) at the circle
    center

*DocSettings*
:   True uses the default settings for this document, false does not

Edits center mark properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub EditCenterMarkProperties( _    ByVal Angle As System.Double, _    ByVal Size As System.Double, _    ByVal Lines As System.Boolean, _    ByVal DocSettings As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Angle As System.Double Dim Size As System.Double Dim Lines As System.Boolean Dim DocSettings As System.Boolean   instance.EditCenterMarkProperties(Angle, Size, Lines, DocSettings) ``` | |

| C# |  |
| --- | --- |
| ``` void EditCenterMarkProperties(     System.double Angle,    System.double Size,    System.bool Lines,    System.bool DocSettings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void EditCenterMarkProperties(  &   System.double Angle, &   System.double Size, &   System.bool Lines, &   System.bool DocSettings ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*
:   New angle of the center mark

*Size*
:   New size of the center mark

*Lines*
:   True displays the center mark lines, false displays the plus sign (+) at the circle
    center

*DocSettings*
:   True uses the default settings for this document, false does not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::EditCenterMarkProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[ICenterMark Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0