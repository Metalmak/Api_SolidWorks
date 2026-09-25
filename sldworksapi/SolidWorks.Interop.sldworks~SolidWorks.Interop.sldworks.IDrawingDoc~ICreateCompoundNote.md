<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateCompoundNote.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateCompoundNote Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateCompoundNote Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Height*
:   Note height in meters

*X*
:   x location of note in meters

*Y*
:   y location of note in meters

*Z*
:   z location of note in meters

Obsolete for documents created in SOLIDWORKS 2016 and later. Creates and returns a compound note.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateCompoundNote( _    ByVal Height As System.Double, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) As Note ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Height As System.Double Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As Note   value = instance.ICreateCompoundNote(Height, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` Note ICreateCompoundNote(     System.double Height,    System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Note^ ICreateCompoundNote(  &   System.double Height, &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Height*
:   Note height in meters

*X*
:   x location of note in meters

*Y*
:   y location of note in meters

*Z*
:   z location of note in meters

#### Return Value

Pointer to the newly created compound [note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateCompoundNote.

# ![](dotnetimages/collapse.gif)Remarks

A compound note is a note that can contain multiple text strings and sketch geometry.

Compound notes are equivalent to a user-defined symbol. After creating a compound note, you can use the other compound note methods to add text and sketch geometry to the object.

This object appears to the end-user as though it were one item. If the user selects the compound note and drags it, all of the entities and text move together.

Because a compound note can have multiple pieces of text, many of the compound note methods require that you specify the index value of the text. For example, the first piece of text added to the compound note using [INote::AddText](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~AddText.html) has index number 1, the second text added has index number 2, and so on.

SOLIDWORKS adds the note to the view of the current selection, so you must make a selection before you call this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::CreateCompoundNote Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateCompoundNote.html)