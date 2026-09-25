<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~GetHyperLinkAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetHyperLinkAt Method (ISwDMDocument) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument.html) : GetHyperLinkAt Method (ISwDMDocument) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*at*
:   0-based index at which to get the embedded hyperlinks

Gets the embedded hyperlinks at the specified index for this document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetHyperLinkAt( _    ByVal at As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument Dim at As System.Integer Dim value As System.String   value = instance.GetHyperLinkAt(at) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetHyperLinkAt(     System.int at ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetHyperLinkAt(  &   System.int at ) ``` | |

#### Parameters

*at*
:   0-based index at which to get the embedded hyperlinks

#### Return Value

Hyperlinks

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument::GetHyperLinkAt.

# ![](dotnetimages/collapse.gif)Example

[Get Hyperlinks (C#)](Get_Hyperlinks_Example_CSharp.htm)

[Get Hyperlinks (VB.NET)](Get_Hyperlinks_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ISwDMDocument::GetHyperLinksCount](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument~GetHyperLinksCount.html) to get the number of embedded hyperlinks associated with this document.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument.html)

[ISwDMDocument Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument_members.html)

[ISwDMDocument::ModifyHyperLinkAt Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~ModifyHyperLinkAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2004 FCS