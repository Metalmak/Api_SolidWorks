<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~SetHyperlinkText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetHyperlinkText Method (INote) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html) : SetHyperlinkText Method (INote) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Text*
:   Text for hyperlink

Sets the hyperlink in a note.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetHyperlinkText( _    ByVal Text As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As INote Dim Text As System.String Dim value As System.Boolean   value = instance.SetHyperlinkText(Text) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetHyperlinkText(     System.string Text ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetHyperlinkText(  &   System.String^ Text ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Text*
:   Text for hyperlink

#### Return Value

True if the hyperlink is successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Note::SetHyperlinkText.

# ![](dotnetimages/collapse.gif)Remarks

You can retrieve the hyperlink text using [INote::GetHyperlinkText](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~GetHyperlinkText.html).

The input text can be a URL address or the name of a document on the local network or on your local system. You must specify the full address for a URL address, starting with the http://. You can specify a file name on your local network or system either as a full pathname or pathname relative to the current document, for example, D:\parts\drawing1.slddrw, or drawing1.slddrw.

To remove the hyperlink from a note, use this method and specify non-hyperlinked text.

# ![](dotnetimages/collapse.gif)See Also

####

[INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)

[INote Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote_members.html)

[INote::GetHyperlinkText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetHyperlinkText.html)