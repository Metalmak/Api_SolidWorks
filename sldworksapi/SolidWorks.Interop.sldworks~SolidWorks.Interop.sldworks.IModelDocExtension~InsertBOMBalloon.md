<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertBOMBalloon.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBOMBalloon Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertBOMBalloon Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Style*
:   Balloon style as defined in swBalloonStyle\_e

*Size*
:   Balloon size as defined in swBalloonFit\_e

*UpperTextStyle*
:   Style for the upper text of the balloon as defined in swBalloonTextContent\_e (see **Remarks**)

*UpperText*
:   Upper text of the balloon

*LowerTextStyle*
:   Style for the lower text of the balloon as defined in swBalloonTextContent\_e; valid for balloons only and Style must be set to swBS\_SplitCirc (see **Remarks**)

*LowerText*
:   Lower text of the balloon; valid for balloons only and Style must be set to swBS\_SplitCirc

*CustomSize*
:   :   User-defined size of the balloon; Size must be set to swBF\_UserDef

*ShowQuantity*
:   :   True to show quantity, false to not

*QuantityPlacement*
:   Placement of quantity value:

    * 0 = Left* 1 = Right* 2 = Top* 3 = Bottom

*QuantityDenotationText*
:   Denotation text for quantity

Obsolete. Superseded by [IModelDocExtension::InsertBomBalloon2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~InsertBomBalloon2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBOMBalloon( _    ByVal Style As System.Integer, _    ByVal Size As System.Integer, _    ByVal UpperTextStyle As System.Integer, _    ByVal UpperText As System.String, _    ByVal LowerTextStyle As System.Integer, _    ByVal LowerText As System.String, _    ByVal CustomSize As System.Double, _    ByVal ShowQuantity As System.Boolean, _    ByVal QuantityPlacement As System.Short, _    ByVal QuantityDenotationText As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Style As System.Integer Dim Size As System.Integer Dim UpperTextStyle As System.Integer Dim UpperText As System.String Dim LowerTextStyle As System.Integer Dim LowerText As System.String Dim CustomSize As System.Double Dim ShowQuantity As System.Boolean Dim QuantityPlacement As System.Short Dim QuantityDenotationText As System.String Dim value As System.Object   value = instance.InsertBOMBalloon(Style, Size, UpperTextStyle, UpperText, LowerTextStyle, LowerText, CustomSize, ShowQuantity, QuantityPlacement, QuantityDenotationText) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertBOMBalloon(     System.int Style,    System.int Size,    System.int UpperTextStyle,    System.string UpperText,    System.int LowerTextStyle,    System.string LowerText,    System.double CustomSize,    System.bool ShowQuantity,    System.short QuantityPlacement,    System.string QuantityDenotationText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertBOMBalloon(  &   System.int Style, &   System.int Size, &   System.int UpperTextStyle, &   System.String^ UpperText, &   System.int LowerTextStyle, &   System.String^ LowerText, &   System.double CustomSize, &   System.bool ShowQuantity, &   System.short QuantityPlacement, &   System.String^ QuantityDenotationText ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*
:   Balloon style as defined in swBalloonStyle\_e

*Size*
:   Balloon size as defined in swBalloonFit\_e

*UpperTextStyle*
:   Style for the upper text of the balloon as defined in swBalloonTextContent\_e (see **Remarks**)

*UpperText*
:   Upper text of the balloon

*LowerTextStyle*
:   Style for the lower text of the balloon as defined in swBalloonTextContent\_e; valid for balloons only and Style must be set to swBS\_SplitCirc (see **Remarks**)

*LowerText*
:   Lower text of the balloon; valid for balloons only and Style must be set to swBS\_SplitCirc

*CustomSize*
:   :   User-defined size of the balloon; Size must be set to swBF\_UserDef

*ShowQuantity*
:   :   True to show quantity, false to not

*QuantityPlacement*
:   Placement of quantity value:

    * 0 = Left* 1 = Right* 2 = Top* 3 = Bottom

*QuantityDenotationText*
:   Denotation text for quantity

#### Return Value

[Note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertBOMBalloon.

# ![](dotnetimages/collapse.gif)Remarks

See [INote::PropertyLinkedText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~PropertyLinkedText.html) for examples of link strings usable with swBalloonTextContent\_e.swBalloonTextCustomProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IDrawingDoc::AutoBalloon3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AutoBalloon3.html)

[INote::GetBomBalloonText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetBomBalloonText.html)

[INote::GetBomBalloonTextStyle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetBomBalloonTextStyle.html)

[INote::SetBomBalloonText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~SetBomBalloonText.html)

[INote::IsBomBalloon Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~IsBomBalloon.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision number 18.0