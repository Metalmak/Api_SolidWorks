<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~MoveDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MoveDocument Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : MoveDocument Method (ISldWorks) |

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
| ``` Function MoveDocument( _    ByVal SourceDoc As System.String, _    ByVal DestDoc As System.String, _    ByVal FromChildren As System.Object, _    ByVal ToChildren As System.Object, _    ByVal Option As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim SourceDoc As System.String Dim DestDoc As System.String Dim FromChildren As System.Object Dim ToChildren As System.Object Dim Option As System.Integer Dim value As System.Integer   value = instance.MoveDocument(SourceDoc, DestDoc, FromChildren, ToChildren, Option) ``` | |

| C# |  |
| --- | --- |
| ``` System.int MoveDocument(     System.string SourceDoc,    System.string DestDoc,    System.object FromChildren,    System.object ToChildren,    System.int Option ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int MoveDocument(  &   System.String^ SourceDoc, &   System.String^ DestDoc, &   System.Object^ FromChildren, &   System.Object^ ToChildren, &   System.int Option ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SourceDoc*
:   Full path and filename of the document to move

*DestDoc*
:   Full path and filename of the new document to which to move the document specified for SourceDoc

*FromChildren*
:   Array of strings containing the full path and filenames of the child documents dependent on the document specified for SourceDoc

*ToChildren*
:   Array of strings containing the new full path and filenames for the child documents to which to move the documents specified for FromChildren

*Option*
:   Move options as defined by swMoveCopyOptions\_e

#### Return Value

Success or error code as defined by swMoveCopyError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::MoveDocument.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::IMoveDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IMoveDocument.html)

[ISldWorks::ICopyDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ICopyDocument.html)

[ISldWorks::CopyDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CopyDocument.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0