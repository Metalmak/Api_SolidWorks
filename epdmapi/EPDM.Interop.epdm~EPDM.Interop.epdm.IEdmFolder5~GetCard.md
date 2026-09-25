<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetCard.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCard Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : GetCard Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsExtension*
:   Extension of file for which to get a data card; for example, "DWG" or "DOC" or "." to get the data card for this folder

Gets the interface to a data card of a file of the specified file type or the interface to the data card of this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetCard( _    ByVal bsExtension As System.String _ ) As IEdmCard5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmCard5 GetCard(     System.string bsExtension ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmCard5^ GetCard(  &   System.String^ bsExtension ) ``` | |

#### Parameters

*bsExtension*
:   Extension of file for which to get a data card; for example, "DWG" or "DOC" or "." to get the data card for this folder

#### Return Value

[IEdmCard5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html)

# ![](dotnetimages/collapse.gif)Example

[Find Data Cards with Description Variable (C#)](Find_Data_Cards_with_Description_Variable_Example_CSharp.htm)

[Find Data Cards with Description Variable (VB.NET)](Find_Data_Cards_with_Description_Variable_Example_VBNET.htm)

[Get Card Control Information (VB.NET)](Get_Card_Control_Info_Example_VBNET.htm)

[Get Card Control Information (C#)](Get_Card_Control_Info_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you only need the card ID, it is faster to call [IEdmfolder5::GetCardID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetCardID.html) than to call this method.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmCard5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_NAME: There is no data card matching the specified extension.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2