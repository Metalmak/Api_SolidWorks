<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~ModifyHyperLinkAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| ModifyHyperLinkAt Method (ISwDMDocument) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument.html) : ModifyHyperLinkAt Method (ISwDMDocument) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*at*
:   0-based index at which to set the embedded hyperlink

*newlink*
:   New embedded hyperlink

Sets the embedded hyperlink at the specified index for this document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ModifyHyperLinkAt( _    ByVal at As System.Integer, _    ByVal newlink As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument Dim at As System.Integer Dim newlink As System.String   instance.ModifyHyperLinkAt(at, newlink) ``` | |

| C# |  |
| --- | --- |
| ``` void ModifyHyperLinkAt(     System.int at,    System.string newlink ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ModifyHyperLinkAt(  &   System.int at, &   System.String^ newlink ) ``` | |

#### Parameters

*at*
:   0-based index at which to set the embedded hyperlink

*newlink*
:   New embedded hyperlink

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument::ModifyHyperLinkAt.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ISwDMDocument::GetHyperLinksCount](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument~GetHyperLinksCount.html) to get the number of embedded hyperlinks for this document.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument.html)

[ISwDMDocument Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument_members.html)

[ISwDMDocument::GetHyperLinkAt Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~GetHyperLinkAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2004 FCS