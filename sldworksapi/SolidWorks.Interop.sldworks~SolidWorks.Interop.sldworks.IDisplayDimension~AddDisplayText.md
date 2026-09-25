<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~AddDisplayText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddDisplayText Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : AddDisplayText Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Text*
:   Text to display

*Position*
:   Location of the text; array of 3 doubles

*Format*
:   Object for the text format

*Attachment*
:   Justification of the text as defined in swTextJustification\_e

*WidthFactor*
:   Horizontal scale factor of the text

Overrides the display text.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDisplayText( _    ByVal Text As System.String, _    ByVal Position As System.Object, _    ByVal Format As System.Object, _    ByVal Attachment As System.Integer, _    ByVal WidthFactor As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim Text As System.String Dim Position As System.Object Dim Format As System.Object Dim Attachment As System.Integer Dim WidthFactor As System.Double Dim value As System.Boolean   value = instance.AddDisplayText(Text, Position, Format, Attachment, WidthFactor) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddDisplayText(     System.string Text,    System.object Position,    System.object Format,    System.int Attachment,    System.double WidthFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddDisplayText(  &   System.String^ Text, &   System.Object^ Position, &   System.Object^ Format, &   System.int Attachment, &   System.double WidthFactor ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Text*
:   Text to display

*Position*
:   Location of the text; array of 3 doubles

*Format*
:   Object for the text format

*Attachment*
:   Justification of the text as defined in swTextJustification\_e

*WidthFactor*
:   Horizontal scale factor of the text

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::AddDisplayText.

# ![](dotnetimages/collapse.gif)Example

[Replace Dimension with Text (VBA)](Replace_Dimension_with_Text_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The new graphics displayed by this method are temporary. When the user changes the dimension, this display dimension reverts back to the SOLIDWORKS standard.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::IAddDisplayText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~IAddDisplayText.html)

[IDisplayDimension::HorizontalJustification Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~HorizontalJustification.html)

[IDisplayDimension::VerticalJustification Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~VerticalJustification.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0