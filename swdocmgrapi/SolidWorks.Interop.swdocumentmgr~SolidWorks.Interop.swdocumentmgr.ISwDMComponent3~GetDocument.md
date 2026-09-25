<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent3~GetDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetDocument Method (ISwDMComponent3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMComponent3 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent3.html) : GetDocument Method (ISwDMComponent3) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*allowReadOnly*
:   True to open the document as read-only, false as read-write

*result*
:   Error as defined by [SwDmDocumentOpenError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmDocumentOpenError.html)

Obsolete. Superseded by [ISwDMComponent4::GetDocument2](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMComponent4~GetDocument2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDocument( _    ByVal allowReadOnly As System.Boolean, _    ByRef result As SwDmDocumentOpenError _ ) As SwDMDocument ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMComponent3 Dim allowReadOnly As System.Boolean Dim result As SwDmDocumentOpenError Dim value As SwDMDocument   value = instance.GetDocument(allowReadOnly, result) ``` | |

| C# |  |
| --- | --- |
| ``` SwDMDocument GetDocument(     System.bool allowReadOnly,    out SwDmDocumentOpenError result ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SwDMDocument^ GetDocument(  &   System.bool allowReadOnly, &   [Out] SwDmDocumentOpenError result ) ``` | |

#### Parameters

*allowReadOnly*
:   True to open the document as read-only, false as read-write

*result*
:   Error as defined by [SwDmDocumentOpenError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmDocumentOpenError.html)

#### Return Value

Pointer to the [ISwDMDocument](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMComponent3::GetDocument.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMComponent3 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent3.html)

[ISwDMComponent3 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2008 FCS