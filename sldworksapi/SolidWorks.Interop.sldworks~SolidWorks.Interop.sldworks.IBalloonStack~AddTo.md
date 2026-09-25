<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonStack~AddTo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddTo Method (IBalloonStack) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBalloonStack Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonStack.html) : AddTo Method (IBalloonStack) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UpperTextStyle*
:   Text style for the text of the balloon as defined in swBalloonTextContent\_e

*UpperText*
:   Text in the balloon

*LowerTextStyle*
:   Text style for the text of the balloon as defined in swBalloonTextContent\_e

*LowerText*
:   Text in the lower part of the balloon (when Style = swBS\_SplitCirc)

Adds a balloon note to this balloon stack.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddTo( _    ByVal UpperTextStyle As System.Integer, _    ByVal UpperText As System.String, _    ByVal LowerTextStyle As System.Integer, _    ByVal LowerText As System.String _ ) As Note ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBalloonStack Dim UpperTextStyle As System.Integer Dim UpperText As System.String Dim LowerTextStyle As System.Integer Dim LowerText As System.String Dim value As Note   value = instance.AddTo(UpperTextStyle, UpperText, LowerTextStyle, LowerText) ``` | |

| C# |  |
| --- | --- |
| ``` Note AddTo(     System.int UpperTextStyle,    System.string UpperText,    System.int LowerTextStyle,    System.string LowerText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Note^ AddTo(  &   System.int UpperTextStyle, &   System.String^ UpperText, &   System.int LowerTextStyle, &   System.String^ LowerText ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UpperTextStyle*
:   Text style for the text of the balloon as defined in swBalloonTextContent\_e

*UpperText*
:   Text in the balloon

*LowerTextStyle*
:   Text style for the text of the balloon as defined in swBalloonTextContent\_e

*LowerText*
:   Text in the lower part of the balloon (when Style = swBS\_SplitCirc)

#### Return Value

[INote](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BalloonStack::AddTo.

# ![](dotnetimages/collapse.gif)Example

[Add Balloon to Stacked Balloon (C#)](Add_Balloon_to_Stacked_Balloon_Example_CSharp.htm)

[Add Balloon to Stacked Balloon (VB.NET)](Add_Balloon_to_Stacked_Balloon_Example_VBNET.htm)

[Add Balloon to Stacked Balloon (VBA)](Add_Balloon_to_Stacked_Balloon_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method adds a balloon note that is attached to the preselected entity to this stack. It returns an INote object, which you can then use to access the note (for example, to set the font of the note text). The balloon style and size are the same as the initial balloon in this stack.

If the balloon style is split circle, this method uses both the lower and upper text arguments. If the balloon style is anything other than split circle, this method uses the upper text arguments and ignores the lower text arguments.

If the text style is item number or quantity, SOLIDWORKS uses the note text to determine the preselected entity that this note is attached to, and ignores the corresponding text argument. If the preselection is a location on the drawing instead of an entity, you must specify the text style and text.

Use [INote::GetBalloonStack](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~GetBalloonStack.html) to get a balloon stack interface from an existing note.

# ![](dotnetimages/collapse.gif)See Also

####

[IBalloonStack Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonStack.html)

[IBalloonStack Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonStack_members.html)

[INote::MakeStackedBalloon Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~MakeStackedBalloon.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0