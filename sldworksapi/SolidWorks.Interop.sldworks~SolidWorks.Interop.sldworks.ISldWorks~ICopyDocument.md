<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ICopyDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICopyDocument Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ICopyDocument Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SourceDoc*
:   Full path and filename of the document to copy

*DestDoc*
:   Full path and filename of the document to which to copy SourceDoc

*ChildCount*
:   Number of child documents for SourceDoc

*FromChildren*
:   Array containing the full path and filenames of the child documents dependent on the document specified for SourceDoc

*ToChildren*
:   Array of strings containing the new full path and filenames of the child documents to which to copy the child documents specified for FromChildren

*Option*
:   Copy options as defined by swMoveCopyOptions\_e

Copies a document and optionally updates references to it.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICopyDocument( _    ByVal SourceDoc As System.String, _    ByVal DestDoc As System.String, _    ByVal ChildCount As System.Integer, _    ByRef FromChildren As System.String, _    ByRef ToChildren As System.String, _    ByVal Option As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim SourceDoc As System.String Dim DestDoc As System.String Dim ChildCount As System.Integer Dim FromChildren As System.String Dim ToChildren As System.String Dim Option As System.Integer Dim value As System.Integer   value = instance.ICopyDocument(SourceDoc, DestDoc, ChildCount, FromChildren, ToChildren, Option) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ICopyDocument(     System.string SourceDoc,    System.string DestDoc,    System.int ChildCount,    ref System.string FromChildren,    ref System.string ToChildren,    System.int Option ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ICopyDocument(  &   System.String^ SourceDoc, &   System.String^ DestDoc, &   System.int ChildCount, &   System.String^% FromChildren, &   System.String^% ToChildren, &   System.int Option ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SourceDoc*
:   Full path and filename of the document to copy

*DestDoc*
:   Full path and filename of the document to which to copy SourceDoc

*ChildCount*
:   Number of child documents for SourceDoc

*FromChildren*
:   Array containing the full path and filenames of the child documents dependent on the document specified for SourceDoc

*ToChildren*
:   Array of strings containing the new full path and filenames of the child documents to which to copy the child documents specified for FromChildren

*Option*
:   Copy options as defined by swMoveCopyOptions\_e

#### Return Value

Success or error code as defined by swMoveCopyError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ICopyDocument.

# ![](dotnetimages/collapse.gif)Example

[Copy Document (C++)](Copy_Document_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

There can be no documents open when using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::MoveDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~MoveDocument.html)

[IModelDocExtension::SaveAs Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SaveAs.html)

[ISldWorks::CopyDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CopyDocument.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0