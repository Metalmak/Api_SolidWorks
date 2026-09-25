<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IMoveDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMoveDocument Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : IMoveDocument Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SourceDoc*
:   Full path and filename of the document to move

*DestDoc*
:   Full path and filename of the new document to which to move the document specified for SourceDoc

*ChildCount*
:   Number of child documents for SourceDoc

*FromChildren*
:   Array of strings containing the full path and filenames of the child documents dependent on the document specified for SourceDoc

*ToChildren*
:   Array of strings containing the new full path and filenames for the child documents to which to move the documents specified for FromChildren

*Option*
:   Move options as defined by swMoveCopyOptions\_e

Moves a document and optionally updates references to it.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IMoveDocument( _    ByVal SourceDoc As System.String, _    ByVal DestDoc As System.String, _    ByVal ChildCount As System.Integer, _    ByRef FromChildren As System.String, _    ByRef ToChildren As System.String, _    ByVal Option As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim SourceDoc As System.String Dim DestDoc As System.String Dim ChildCount As System.Integer Dim FromChildren As System.String Dim ToChildren As System.String Dim Option As System.Integer Dim value As System.Integer   value = instance.IMoveDocument(SourceDoc, DestDoc, ChildCount, FromChildren, ToChildren, Option) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IMoveDocument(     System.string SourceDoc,    System.string DestDoc,    System.int ChildCount,    ref System.string FromChildren,    ref System.string ToChildren,    System.int Option ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IMoveDocument(  &   System.String^ SourceDoc, &   System.String^ DestDoc, &   System.int ChildCount, &   System.String^% FromChildren, &   System.String^% ToChildren, &   System.int Option ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SourceDoc*
:   Full path and filename of the document to move

*DestDoc*
:   Full path and filename of the new document to which to move the document specified for SourceDoc

*ChildCount*
:   Number of child documents for SourceDoc

*FromChildren*
:   Array of strings containing the full path and filenames of the child documents dependent on the document specified for SourceDoc

*ToChildren*
:   Array of strings containing the new full path and filenames for the child documents to which to move the documents specified for FromChildren

*Option*
:   Move options as defined by swMoveCopyOptions\_e

#### Return Value

Success or error code as defined by swMoveCopyError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::IMoveDocument.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::MoveDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~MoveDocument.html)

[ISldWorks::ICopyDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ICopyDocument.html)

[ISldWorks::CopyDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CopyDocument.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0