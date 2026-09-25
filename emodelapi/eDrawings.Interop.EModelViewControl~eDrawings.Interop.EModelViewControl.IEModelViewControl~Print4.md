<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Print4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| Print4 Method (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : Print4 Method (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ShowDialog*
:   True to show the Print dialog, false to not

*FileName*
:   Document name to show in the printer queue for this eDrawings file (see Remarks)

*Shaded*
:   True to print shaded, false to not print shaded

*DraftQuality*
:   True to print draft quality, false to print regular quality

*Color*
:   True to print in grayscale on black-and-white printers, false to print black and white (lines, edges, and text are black, and shaded data is grayscale)

*printType*
:   Scale the eDrawings file as defined in [EMVPrintType](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVPrintType.html) (see Remarks)

*scale*
:   Scaling factor; this argument is valid only when printType is set to eScaled

*centerOffsetX*
:   Offset in thousands of an inch; this argument is valid only when printType is set to eScaled

*centerOffsetY*
:   Offset in thousands of an inch; this argument is valid only when printType is set to eScaled

*printAll*
:   True to print all pages, false to not

*pageFirst*
:   Page number of first page to print

*pageLast*
:   Page number of last page to print

Obsolete. Superseded by [IEModelViewControl::Print5](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Print5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Print4( _    ByVal ShowDialog As System.Boolean, _    ByVal FileName As System.String, _    ByVal Shaded As System.Boolean, _    ByVal DraftQuality As System.Boolean, _    ByVal Color As System.Boolean, _    ByVal printType As EMVPrintType, _    ByVal scale As System.Double, _    ByVal centerOffsetX As System.Integer, _    ByVal centerOffsetY As System.Integer, _    ByVal printAll As System.Boolean, _    ByVal pageFirst As System.Integer, _    ByVal pageLast As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim ShowDialog As System.Boolean Dim FileName As System.String Dim Shaded As System.Boolean Dim DraftQuality As System.Boolean Dim Color As System.Boolean Dim printType As EMVPrintType Dim scale As System.Double Dim centerOffsetX As System.Integer Dim centerOffsetY As System.Integer Dim printAll As System.Boolean Dim pageFirst As System.Integer Dim pageLast As System.Integer   instance.Print4(ShowDialog, FileName, Shaded, DraftQuality, Color, printType, scale, centerOffsetX, centerOffsetY, printAll, pageFirst, pageLast) ``` | |

| C# |  |
| --- | --- |
| ``` void Print4(     System.bool ShowDialog,    System.string FileName,    System.bool Shaded,    System.bool DraftQuality,    System.bool Color,    EMVPrintType printType,    System.double scale,    System.int centerOffsetX,    System.int centerOffsetY,    System.bool printAll,    System.int pageFirst,    System.int pageLast ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Print4(  &   System.bool ShowDialog, &   System.String^ FileName, &   System.bool Shaded, &   System.bool DraftQuality, &   System.bool Color, &   EMVPrintType printType, &   System.double scale, &   System.int centerOffsetX, &   System.int centerOffsetY, &   System.bool printAll, &   System.int pageFirst, &   System.int pageLast ) ``` | |

#### Parameters

*ShowDialog*
:   True to show the Print dialog, false to not

*FileName*
:   Document name to show in the printer queue for this eDrawings file (see Remarks)

*Shaded*
:   True to print shaded, false to not print shaded

*DraftQuality*
:   True to print draft quality, false to print regular quality

*Color*
:   True to print in grayscale on black-and-white printers, false to print black and white (lines, edges, and text are black, and shaded data is grayscale)

*printType*
:   Scale the eDrawings file as defined in [EMVPrintType](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVPrintType.html) (see Remarks)

*scale*
:   Scaling factor; this argument is valid only when printType is set to eScaled

*centerOffsetX*
:   Offset in thousands of an inch; this argument is valid only when printType is set to eScaled

*centerOffsetY*
:   Offset in thousands of an inch; this argument is valid only when printType is set to eScaled

*printAll*
:   True to print all pages, false to not

*pageFirst*
:   Page number of first page to print

*pageLast*
:   Page number of last page to print

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::Print4.

# ![](dotnetimages/collapse.gif)Remarks

Set [IEModelViewControl::SetPageSetupOptions](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~SetPageSetupOptions.html) before calling this method.

You can use the FileName argument to describe the eDrawings file so that it is easily recognizable in the printer queue.

The printType argument must be set to eWYSIWYG for parts and assemblies. eWYSIWYG is also valid for drawings as are the other [EMVPrintType](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVPrintType.html) enumerations.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings 2010 SP0