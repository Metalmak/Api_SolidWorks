<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Print2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| Print2 Method (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : Print2 Method (IEModelViewControl) |

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
:   True to print shaded, false to print not shaded

*DraftQuality*
:   True to print draft quality, false to print regular quality

*Color*
:   True to print color, false to print black and white

*ScaleToFit*
:   Scale the eDrawings file as defined in [EMVPrintType](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVPrintType.html) (see Remarks)

Obsolete. Superseded by [IEModelViewControl::Print3](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Print3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Print2( _    ByVal ShowDialog As System.Boolean, _    ByVal FileName As System.String, _    ByVal Shaded As System.Boolean, _    ByVal DraftQuality As System.Boolean, _    ByVal Color As System.Boolean, _    ByVal ScaleToFit As EMVPrintType _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim ShowDialog As System.Boolean Dim FileName As System.String Dim Shaded As System.Boolean Dim DraftQuality As System.Boolean Dim Color As System.Boolean Dim ScaleToFit As EMVPrintType   instance.Print2(ShowDialog, FileName, Shaded, DraftQuality, Color, ScaleToFit) ``` | |

| C# |  |
| --- | --- |
| ``` void Print2(     System.bool ShowDialog,    System.string FileName,    System.bool Shaded,    System.bool DraftQuality,    System.bool Color,    EMVPrintType ScaleToFit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Print2(  &   System.bool ShowDialog, &   System.String^ FileName, &   System.bool Shaded, &   System.bool DraftQuality, &   System.bool Color, &   EMVPrintType ScaleToFit ) ``` | |

#### Parameters

*ShowDialog*
:   True to show the Print dialog, false to not

*FileName*
:   Document name to show in the printer queue for this eDrawings file (see Remarks)

*Shaded*
:   True to print shaded, false to print not shaded

*DraftQuality*
:   True to print draft quality, false to print regular quality

*Color*
:   True to print color, false to print black and white

*ScaleToFit*
:   Scale the eDrawings file as defined in [EMVPrintType](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVPrintType.html) (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::Print2.

# ![](dotnetimages/collapse.gif)Remarks

Set [IEModelViewControl::SetPageSetupOptions](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~SetPageSetupOptions.html) before calling this method.

You can use the FileName argument to describe the eDrawings file so that it is easily recognizable in the printer queue. This argument is optional.

The ScaleToFit argument must be set to eWYSIWYG for parts and assemblies; the other two options are only appropriate for drawings.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[\_IEModelViewControlEvents\_OnFailedPrintingDocumentEventHandler Delegate](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler.html)

[\_IEModelViewControlEvents\_OnFinishedPrintingDocumentEventHandler Delegate](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedPrintingDocumentEventHandler.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0