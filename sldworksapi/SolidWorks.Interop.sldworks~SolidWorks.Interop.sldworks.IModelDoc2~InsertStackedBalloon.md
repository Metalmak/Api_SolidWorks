<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertStackedBalloon.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertStackedBalloon Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertStackedBalloon Method (IModelDoc2) |

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
:   Text style for the upper text of the balloon as defined in swBalloonTextContent\_e

*UpperText*
:   Text in the balloon

*LowerTextStyle*
:   Text style for the lower text of the balloon as defined in swBalloonTextContent\_e

*LowerText*
:   Text in the lower part of the balloon when Style = swBS\_SplitCirc

Obsolete. Superseded by [IModelDocExtension::InsertStackedBalloon](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~InsertStackedBalloon.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertStackedBalloon( _    ByVal Style As System.Integer, _    ByVal Size As System.Integer, _    ByVal UpperTextStyle As System.Integer, _    ByVal UpperText As System.String, _    ByVal LowerTextStyle As System.Integer, _    ByVal LowerText As System.String _ ) As Note ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Style As System.Integer Dim Size As System.Integer Dim UpperTextStyle As System.Integer Dim UpperText As System.String Dim LowerTextStyle As System.Integer Dim LowerText As System.String Dim value As Note   value = instance.InsertStackedBalloon(Style, Size, UpperTextStyle, UpperText, LowerTextStyle, LowerText) ``` | |

| C# |  |
| --- | --- |
| ``` Note InsertStackedBalloon(     System.int Style,    System.int Size,    System.int UpperTextStyle,    System.string UpperText,    System.int LowerTextStyle,    System.string LowerText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Note^ InsertStackedBalloon(  &   System.int Style, &   System.int Size, &   System.int UpperTextStyle, &   System.String^ UpperText, &   System.int LowerTextStyle, &   System.String^ LowerText ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*
:   Balloon style as defined in swBalloonStyle\_e

*Size*
:   Balloon size as defined in swBalloonFit\_e

*UpperTextStyle*
:   Text style for the upper text of the balloon as defined in swBalloonTextContent\_e

*UpperText*
:   Text in the balloon

*LowerTextStyle*
:   Text style for the lower text of the balloon as defined in swBalloonTextContent\_e

*LowerText*
:   Text in the lower part of the balloon when Style = swBS\_SplitCirc

#### Return Value

Newly created [note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertStackedBalloon.

# ![](dotnetimages/collapse.gif)Remarks

This method adds a single balloon note attached to the pre-selected entity. The note is located near the pre-selection.

This method returns a Note object, which you can then use to access the note; for example, setting the font of the note text or setting the position of the Note. You can stack notes on the Note object returned by this method.

Use [INote::GetBalloonStack](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~GetBalloonStack.html) with this note to get the [IBalloonStack](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBalloonStack.html) object. You can control various properties of the stack, such as the direction and size. You can also use the BalloonStack to stack more balloons on this first balloon.

If the balloon style is split circle, both the lower- and upper-text arguments are used. If the balloon style is anything other than split circle, the upper-text arguments are used and the lower-text arguments are ignored.

If the text style is item number or quantity, the note text is determined through the pres-selected entity to which this note is attached and the corresponding text argument is ignored. If the pre-selection is just a location on the drawing, not an entity, then the text style should be custom and you must specify the text to use.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[INote::IsStackedBalloon Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~IsStackedBalloon.html)

[INote::IsStackedBalloonMaster Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~IsStackedBalloonMaster.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0