<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~AddFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFolder Method (IEdmClearLocalCache) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmClearLocalCache Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache.html) : AddFolder Method (IEdmClearLocalCache) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oFolderIDorPath*
:   ID or path of the folder to clear from the cache

*bRecursive*
:   True to clear subfolders, false to not

Adds the specified folder to the batch of files and folders to clear from the local cache.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFolder( _    ByVal oFolderIDorPath As System.Object, _    Optional ByVal bRecursive As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFolder(     System.object oFolderIDorPath,    System.bool bRecursive ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFolder(  &   System.Object^ oFolderIDorPath, &   System.bool bRecursive ) ``` | |

#### Parameters

*oFolderIDorPath*
:   ID or path of the folder to clear from the cache

*bRecursive*
:   True to clear subfolders, false to not

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you must call [IEdmClearLocalCache::CommitClear](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~CommitClear.html) to actually clear the folder from the cache.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmClearLocalCache Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache.html)

[IEdmClearLocalCache Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008