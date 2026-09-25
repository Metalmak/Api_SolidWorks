<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration2~AddSelection2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddSelection2 Method (IEdmBatchItemGeneration2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchItemGeneration2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration2.html) : AddSelection2 Method (IEdmBatchItemGeneration2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault in which to create the new item

*poVariables*
:   Optional array of [EdmVarVal](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal.html) structures; variables to write to the item

*bsItemName*
:   Name of new item; if left blank, the serial number generator assigns the name

*lDestFolderID*
:   ID of the folder in which to place the new item; if left blank, the new item is placed in the item root folder

*lSrcFileID*
:   ID of the file from which to create the item; if 0 or blank, no link is created

*lSrcFileProjID*
:   ID of the parent folder of lSrcFileID; only valid if lSrcFileID is not 0 or blank

*bsSrcFileConfig*
:   Name of the configuration in the source file to which to link the new item

*lEdmRefFlags*
:   Combination of [EdmRefFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefFlags.html) bits

Adds information to the batch to generate a new item either from a file or stand-alone without a source file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddSelection2( _    ByVal poVault As EdmVault5, _    ByVal poVariables() As EdmVarVal, _    Optional ByVal bsItemName As System.String, _    Optional ByVal lDestFolderID As System.Integer, _    Optional ByVal lSrcFileID As System.Integer, _    Optional ByVal lSrcFileProjID As System.Integer, _    Optional ByVal bsSrcFileConfig As System.String, _    Optional ByVal lEdmRefFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddSelection2(     EdmVault5 poVault,    EdmVarVal[] poVariables,    System.string bsItemName,    System.int lDestFolderID,    System.int lSrcFileID,    System.int lSrcFileProjID,    System.string bsSrcFileConfig,    System.int lEdmRefFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddSelection2(  &   EdmVault5^ poVault, &   array<EdmVarVal>^ poVariables, &   System.String^ bsItemName, &   System.int lDestFolderID, &   System.int lSrcFileID, &   System.int lSrcFileProjID, &   System.String^ bsSrcFileConfig, &   System.int lEdmRefFlags ) ``` | |

#### Parameters

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault in which to create the new item

*poVariables*
:   Optional array of [EdmVarVal](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal.html) structures; variables to write to the item

*bsItemName*
:   Name of new item; if left blank, the serial number generator assigns the name

*lDestFolderID*
:   ID of the folder in which to place the new item; if left blank, the new item is placed in the item root folder

*lSrcFileID*
:   ID of the file from which to create the item; if 0 or blank, no link is created

*lSrcFileProjID*
:   ID of the parent folder of lSrcFileID; only valid if lSrcFileID is not 0 or blank

*bsSrcFileConfig*
:   Name of the configuration in the source file to which to link the new item

*lEdmRefFlags*
:   Combination of [EdmRefFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefFlags.html) bits

# ![](dotnetimages/collapse.gif)Example

[Add Items (C#)](Add_Items_Example_CSharp.htm)

[Add Items (VB.NET)](Add_Items_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmBatchItemGeneration::AddSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~AddSelection.html) by adding the ability to create stand-alone items without a source file.

To create a stand-alone item, you must call this method specifying poVault at a minimum. You can optionally specify poVariables and bsItemName to create a stand-alone item. The other parameters are only used to create new items from files.

After calling this method, call [IEdmBatchItemGeneration::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~CreateTree.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchItemGeneration2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration2.html)

[IEdmBatchItemGeneration2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010