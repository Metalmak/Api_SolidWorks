<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmClearLocalCache Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmClearLocalCache Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Removes specified checked-in files and folders from the local file vault view cache. Only files that are not referenced by checked-out files are cleared.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmClearLocalCache ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmClearLocalCache ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmClearLocalCache ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmClearLocalCache2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache2.html) which provides the option to not remove cached Toolbox Library parts.

This interface provides the same functionality as the Clear Local Cache command that you can run from the context menu of a folder in File Explorer.

To clear the local cache:

1. Access this interface by calling IEdmVault7::CreateUtility, passing [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_ClearLocalCache as a parameter.- Call [IEdmClearLocalCache::AddFileByPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~AddFileByPath.html) or [IEdmClearLocalCache::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~AddFolder.html) one or more times, specifying the files and folders that you want to clear.- Call [IEdmClearLocalCache::CommitClear](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache~CommitClear.html) to clear the local cache.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmClearLocalCache Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)