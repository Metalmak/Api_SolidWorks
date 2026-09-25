<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~CommitClear.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CommitClear Method (IEdmClearLocalCache) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmClearLocalCache Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache.html) : CommitClear Method (IEdmClearLocalCache) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to provide progress feedback to the user

Clears the files and folders specified by [IEdmClearLocalCache::AddFilebyPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~AddFileByPath.html) and [IEdmClearLocalCache::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~AddFolder.html) from the local cache.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CommitClear( _    Optional ByVal poCallback As EdmCallback _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CommitClear(     EdmCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CommitClear(  &   EdmCallback^ poCallback ) ``` | |

#### Parameters

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to provide progress feedback to the user

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmClearLocalCache Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache.html)

[IEdmClearLocalCache Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008