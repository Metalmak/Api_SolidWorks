<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetHyperlinkText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetHyperlinkText Method (INote) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html) : GetHyperlinkText Method (INote) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the hyperlink in a note.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetHyperlinkText() As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As INote Dim value As System.String   value = instance.GetHyperlinkText() ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetHyperlinkText() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetHyperlinkText(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Hyperlink text

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Note::GetHyperlinkText.

# ![](dotnetimages/collapse.gif)Example

[Remove Hyperlink From Note in Drawing (VBA)](Remove_Hyperlink_from_Note_in_Drawing_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can create an embedded hyperlink on a note by using [INote::SetHyperlinkText](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~SetHyperlinkText.html) or by using the hyperlink button on the note creation dialog.

This command first looks for an embedded hyperlink on the note and returns the text used to take the user to that document, which can be on the internet (a URL address is returned) or on your local network or hard drive (a pathname is returned). If the pathname was specified as a relative pathname, then the full pathname is returned.

If an embedded hyperlink does not exist, the note's text is searched for a hyperlink explicitly entered as part of the note text. This could be a URL address (a text string beginning with http://) or a file address (a text string beginning with file://).

If no hyperlink is found, either embedded or explicitly entered within the note text, an empty string is returned.

# ![](dotnetimages/collapse.gif)See Also

####

[INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)

[INote Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote_members.html)

[INote::SetHyperlinkText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~SetHyperlinkText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 98Plus, datecode 1998319