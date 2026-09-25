<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetCardID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCardID Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : GetCardID Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsExtension*
:   Extension of file for which to get a data card ID; for example, "DWG" or "DOC" or "." to get the ID of the data card for this folder

Gets the ID of the data card of a file with the specified extension or the ID of the data card of this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetCardID( _    ByVal bsExtension As System.String _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCardID(     System.string bsExtension ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCardID(  &   System.String^ bsExtension ) ``` | |

#### Parameters

*bsExtension*
:   Extension of file for which to get a data card ID; for example, "DWG" or "DOC" or "." to get the ID of the data card for this folder

#### Return Value

ID of the data card; 0 if not found

# ![](dotnetimages/collapse.gif)Example

[Get Card Control Information (VB.NET)](Get_Card_Control_Info_Example_VBNET.htm)

[Get Card Control Information (C#)](Update_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you need to access the entire card, call [IEdmFolder5::GetCard](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetCard.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The card is not found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2