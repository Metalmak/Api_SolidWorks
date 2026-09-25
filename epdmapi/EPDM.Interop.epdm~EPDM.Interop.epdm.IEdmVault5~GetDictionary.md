<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetDictionary.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetDictionary Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : GetDictionary Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsName*
:   Name of dictionary to get or create

*bCreateIfNew*
:   True to create the dictionary if it does not exist, false to not

Gets or creates the specified dictionary.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetDictionary( _    ByVal bsName As System.String, _    ByVal bCreateIfNew As System.Boolean _ ) As IEdmDictionary5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmDictionary5 GetDictionary(     System.string bsName,    System.bool bCreateIfNew ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmDictionary5^ GetDictionary(  &   System.String^ bsName, &   System.bool bCreateIfNew ) ``` | |

#### Parameters

*bsName*
:   Name of dictionary to get or create

*bCreateIfNew*
:   True to create the dictionary if it does not exist, false to not

#### Return Value

[IEdmDictionary5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html); Null if bCreateIfNew is false and the dictionary with bsName does not exist

# ![](dotnetimages/collapse.gif)Example

[Change Card Variables Add-in (VB.NET)](Change_Card_Variables_Addin_Example_VBNET.htm)

[Change Card Variables Add-in (C#)](Change_Card_Variables_Addin_Example_CSharp.htm)

[Create and Delete Dictionaries (C#)](Create_and_Delete_Dictionaries_Example_CSharp.htm)

[Create and Delete Dictionaries (VB.NET)](Create_and_Delete_Dictionaries_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

A dictionary in SOLIDWORKS PDM Professional is a way of storing arbitrary data in the SOLIDWORKS PDM Professional database. The data is organized into key-value pairs. The values are always strings. The keys can be either integers or strings.

**NOTE:** If you intend to store file- or folder-specific data and want the data to be deleted or copied whenever the file or folder is deleted or copied, consider using card variables instead of dictionaries. Card variables stored using [IEdmEnumeratorVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) do not require corresponding controls in the file or folder data card.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The dictionary with the specified name does not exist, and bCreateIfNew is false.* E\_EDM\_NOT\_LOGGED\_IN: You must call [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2