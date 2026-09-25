<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~IAddDisplayText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddDisplayText Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : IAddDisplayText Method (IDisplayDimension) |

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
:   Location of the text; pointer to an array of 3 doubles

*Format*
:   Pointer to [ITextFormat](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITextFormat.html) object

*Attachment*
:   Justification of the text as defined in swTextJustification\_e

*WidthFactor*
:   Horizontal scale factor of the text

Overrides the display text for this display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddDisplayText( _    ByVal Text As System.String, _    ByRef Position As System.Double, _    ByVal Format As TextFormat, _    ByVal Attachment As System.Integer, _    ByVal WidthFactor As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim Text As System.String Dim Position As System.Double Dim Format As TextFormat Dim Attachment As System.Integer Dim WidthFactor As System.Double Dim value As System.Boolean   value = instance.IAddDisplayText(Text, Position, Format, Attachment, WidthFactor) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IAddDisplayText(     System.string Text,    ref System.double Position,    TextFormat Format,    System.int Attachment,    System.double WidthFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IAddDisplayText(  &   System.String^ Text, &   System.double% Position, &   TextFormat^ Format, &   System.int Attachment, &   System.double WidthFactor ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Text*
:   Text to display

*Position*
:   Location of the text; pointer to an array of 3 doubles

*Format*
:   Pointer to [ITextFormat](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITextFormat.html) object

*Attachment*
:   Justification of the text as defined in swTextJustification\_e

*WidthFactor*
:   Horizontal scale factor of the text

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::IAddDisplayText.

# ![](dotnetimages/collapse.gif)Remarks

The new graphics displayed by this method are temporary. When the user changes the dimension, this display dimension reverts back to the SOLIDWORKS standard.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::AddDisplayText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~AddDisplayText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0