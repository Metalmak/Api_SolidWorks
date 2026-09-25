<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateText2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateText2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateText2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TextString*
:   User input text

*TextX*
:   X text location in meters (see **Remarks**)

*TextY*
:   Y text location in meters (see Remarks)

*TextZ*
:   Z text location in meters (see Remarks)

*TextHeight*
:   Text height in meters

*TextAngle*
:   Text angle for rotated text in radians

Creates a [note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html) containing the specified text at a given location.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateText2( _    ByVal TextString As System.String, _    ByVal TextX As System.Double, _    ByVal TextY As System.Double, _    ByVal TextZ As System.Double, _    ByVal TextHeight As System.Double, _    ByVal TextAngle As System.Double _ ) As Note ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim TextString As System.String Dim TextX As System.Double Dim TextY As System.Double Dim TextZ As System.Double Dim TextHeight As System.Double Dim TextAngle As System.Double Dim value As Note   value = instance.ICreateText2(TextString, TextX, TextY, TextZ, TextHeight, TextAngle) ``` | |

| C# |  |
| --- | --- |
| ``` Note ICreateText2(     System.string TextString,    System.double TextX,    System.double TextY,    System.double TextZ,    System.double TextHeight,    System.double TextAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Note^ ICreateText2(  &   System.String^ TextString, &   System.double TextX, &   System.double TextY, &   System.double TextZ, &   System.double TextHeight, &   System.double TextAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TextString*
:   User input text

*TextX*
:   X text location in meters (see **Remarks**)

*TextY*
:   Y text location in meters (see Remarks)

*TextZ*
:   Z text location in meters (see Remarks)

*TextHeight*
:   Text height in meters

*TextAngle*
:   Text angle for rotated text in radians

#### Return Value

Pointer to the [note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateText2.

# ![](dotnetimages/collapse.gif)Remarks

The location specifies the position of the upper-left corner of the box containing the text with respect to the lower-left corner of the drawing.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::CreateText2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateText2.html)