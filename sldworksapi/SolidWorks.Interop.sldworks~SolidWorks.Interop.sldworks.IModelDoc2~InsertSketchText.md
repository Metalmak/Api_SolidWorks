<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSketchText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSketchText Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertSketchText Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Ptx*
:   X coordinate of starting point of text block

*Pty*
:   Y coordinate of starting point of text block

*Ptz*
:   Z coordinate of starting point of text block

*Text*
:   Text to insert (see **Remarks**)

*Alignment*
:   * 0 = Left

      * 1 = Center

        * 2 = Right

          * 3 = Fully justified

    (see **Remarks**)

*FlipDirection*
:   1 to flip text vertically about the selected entity, 0 to not (see **Remarks**)

*HorizontalMirror*
:   1 to flip text horizontally, 0 to not

*WidthFactor*
:   6 <= Percentage by which to evenly widen each character in the text block < = 1667

*SpaceBetweenChars*
:   1 <= Percentage of space between each character in the text block <= 10000; valid only if Alignment != 3

Inserts sketch text.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSketchText( _    ByVal Ptx As System.Double, _    ByVal Pty As System.Double, _    ByVal Ptz As System.Double, _    ByVal Text As System.String, _    ByVal Alignment As System.Integer, _    ByVal FlipDirection As System.Integer, _    ByVal HorizontalMirror As System.Integer, _    ByVal WidthFactor As System.Integer, _    ByVal SpaceBetweenChars As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Ptx As System.Double Dim Pty As System.Double Dim Ptz As System.Double Dim Text As System.String Dim Alignment As System.Integer Dim FlipDirection As System.Integer Dim HorizontalMirror As System.Integer Dim WidthFactor As System.Integer Dim SpaceBetweenChars As System.Integer Dim value As System.Object   value = instance.InsertSketchText(Ptx, Pty, Ptz, Text, Alignment, FlipDirection, HorizontalMirror, WidthFactor, SpaceBetweenChars) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertSketchText(     System.double Ptx,    System.double Pty,    System.double Ptz,    System.string Text,    System.int Alignment,    System.int FlipDirection,    System.int HorizontalMirror,    System.int WidthFactor,    System.int SpaceBetweenChars ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertSketchText(  &   System.double Ptx, &   System.double Pty, &   System.double Ptz, &   System.String^ Text, &   System.int Alignment, &   System.int FlipDirection, &   System.int HorizontalMirror, &   System.int WidthFactor, &   System.int SpaceBetweenChars ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Ptx*
:   X coordinate of starting point of text block

*Pty*
:   Y coordinate of starting point of text block

*Ptz*
:   Z coordinate of starting point of text block

*Text*
:   Text to insert (see **Remarks**)

*Alignment*
:   * 0 = Left

      * 1 = Center

        * 2 = Right

          * 3 = Fully justified

    (see **Remarks**)

*FlipDirection*
:   1 to flip text vertically about the selected entity, 0 to not (see **Remarks**)

*HorizontalMirror*
:   1 to flip text horizontally, 0 to not

*WidthFactor*
:   6 <= Percentage by which to evenly widen each character in the text block < = 1667

*SpaceBetweenChars*
:   1 <= Percentage of space between each character in the text block <= 10000; valid only if Alignment != 3

#### Return Value

[Sketch text](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchText.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertSketchText.

# ![](dotnetimages/collapse.gif)Example

[Insert Text At Angle (VBA)](Insert_Text_at_Angle_Example_VB.htm)

[Align Text With Line (VBA)](Align_Text_with_Line_Eample_VB.htm)

[Insert Sketch Text and Hole (VBA)](Insert_Sketch_Text_and_Hole_Example_VB.htm)

[Insert Sketch Text and Hole (VB.NET)](Insert_Sketch_Text_and_Hole_Example_VBNET.htm)

[Insert Sketch Text and Hole (C#)](Insert_Sketch_Text_and_Hole_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Alignment and FlipDirection are valid only when a curve, edge, or sketch segment is selected. Text appears along the selected entity. If an entity is not selected, Text appears horizontally starting at the origin. [Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) the curve, edge, or sketch segment with Mark = 1.

See the SOL**IDWORKS user-interface help > Sketching > Sketch Entities > Sketch Text > SketchText PropertyManager** topic for more information about this functionality.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::DissolveSketchText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~DissolveSketchText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0