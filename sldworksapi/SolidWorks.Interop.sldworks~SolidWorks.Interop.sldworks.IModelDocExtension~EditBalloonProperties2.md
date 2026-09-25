<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~EditBalloonProperties2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditBalloonProperties2 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : EditBalloonProperties2 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Style*
:   Style of balloon as defined in swBalloonStyle\_e

*Size*
:   Balloon size as defined in swBalloonFit\_e

*UpperTextStyle*
:   Balloon text style as defined in swBalloonTextContent\_e

*UpperText*
:   Text for the balloon; valid only if UpperTextStyle is one of the following:

    * swBalloonTextContent\_e.swBalloonTextCustom* swBalloonTextContent\_e.swBalloonTextCustomProperties* swBalloonTextContent\_e.swBalloonTextCutListProperties

*LowerTextStyle*
:   Lower text style as defined in swBalloonTextContent\_e; valid only if Style is swBalloonStyle\_e.swBS\_SplitCirc

*LowerText*
:   Text for the lower text in the balloon; valid only if Style is swBalloonStyle\_e.swBS\_SplitCirc and LowerTextStyle is one of the following:

    * swBalloonTextContent\_e.swBalloonTextCustom* swBalloonTextContent\_e.swBalloonTextCustomProperties* swBalloonTextContent\_e.swBalloonTextCutListProperties

*CustomSize*
:   User-defined size of the balloon; valid only if Size is swBalloonFit\_e.swBF\_UserDef

*ShowQuantity*
:   True to show quantity, false to not

*QuantityPlacement*
:   Placement of quantity value as defined in swBalloonQuantityPlacement\_e; valid only if ShowQuantity is true

*QuantityDenotationText*
:   Denotation text for quantity; valid only if ShowQuantity is true

*QuantityDistance*
:   Distance between the balloon and the quantity; valid only if ShowQuantity is true

Edits the selected balloon's properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EditBalloonProperties2( _    ByVal Style As System.Integer, _    ByVal Size As System.Integer, _    ByVal UpperTextStyle As System.Integer, _    ByVal UpperText As System.String, _    ByVal LowerTextStyle As System.Integer, _    ByVal LowerText As System.String, _    ByVal CustomSize As System.Double, _    ByVal ShowQuantity As System.Boolean, _    ByVal QuantityPlacement As System.Short, _    ByVal QuantityDenotationText As System.String, _    ByVal QuantityDistance As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Style As System.Integer Dim Size As System.Integer Dim UpperTextStyle As System.Integer Dim UpperText As System.String Dim LowerTextStyle As System.Integer Dim LowerText As System.String Dim CustomSize As System.Double Dim ShowQuantity As System.Boolean Dim QuantityPlacement As System.Short Dim QuantityDenotationText As System.String Dim QuantityDistance As System.Double Dim value As System.Object   value = instance.EditBalloonProperties2(Style, Size, UpperTextStyle, UpperText, LowerTextStyle, LowerText, CustomSize, ShowQuantity, QuantityPlacement, QuantityDenotationText, QuantityDistance) ``` | |

| C# |  |
| --- | --- |
| ``` System.object EditBalloonProperties2(     System.int Style,    System.int Size,    System.int UpperTextStyle,    System.string UpperText,    System.int LowerTextStyle,    System.string LowerText,    System.double CustomSize,    System.bool ShowQuantity,    System.short QuantityPlacement,    System.string QuantityDenotationText,    System.double QuantityDistance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ EditBalloonProperties2(  &   System.int Style, &   System.int Size, &   System.int UpperTextStyle, &   System.String^ UpperText, &   System.int LowerTextStyle, &   System.String^ LowerText, &   System.double CustomSize, &   System.bool ShowQuantity, &   System.short QuantityPlacement, &   System.String^ QuantityDenotationText, &   System.double QuantityDistance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*
:   Style of balloon as defined in swBalloonStyle\_e

*Size*
:   Balloon size as defined in swBalloonFit\_e

*UpperTextStyle*
:   Balloon text style as defined in swBalloonTextContent\_e

*UpperText*
:   Text for the balloon; valid only if UpperTextStyle is one of the following:

    * swBalloonTextContent\_e.swBalloonTextCustom* swBalloonTextContent\_e.swBalloonTextCustomProperties* swBalloonTextContent\_e.swBalloonTextCutListProperties

*LowerTextStyle*
:   Lower text style as defined in swBalloonTextContent\_e; valid only if Style is swBalloonStyle\_e.swBS\_SplitCirc

*LowerText*
:   Text for the lower text in the balloon; valid only if Style is swBalloonStyle\_e.swBS\_SplitCirc and LowerTextStyle is one of the following:

    * swBalloonTextContent\_e.swBalloonTextCustom* swBalloonTextContent\_e.swBalloonTextCustomProperties* swBalloonTextContent\_e.swBalloonTextCutListProperties

*CustomSize*
:   User-defined size of the balloon; valid only if Size is swBalloonFit\_e.swBF\_UserDef

*ShowQuantity*
:   True to show quantity, false to not

*QuantityPlacement*
:   Placement of quantity value as defined in swBalloonQuantityPlacement\_e; valid only if ShowQuantity is true

*QuantityDenotationText*
:   Denotation text for quantity; valid only if ShowQuantity is true

*QuantityDistance*
:   Distance between the balloon and the quantity; valid only if ShowQuantity is true

#### Return Value

[Note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::EditBalloonProperties2.

# ![](dotnetimages/collapse.gif)Example

[Edit Balloon (VBA)](Edit_Balloon_Example_VB.htm)

[Edit Balloon (VB.NET)](Edit_Balloon_Example_VBNET.htm)

[Edit Balloon (C#)](Edit_Balloon_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, select the balloon annotation whose properties you want to edit.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[INote::SetBalloon Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~SetBalloon.html)

[INote::SetBomBalloonText Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~SetBomBalloonText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0