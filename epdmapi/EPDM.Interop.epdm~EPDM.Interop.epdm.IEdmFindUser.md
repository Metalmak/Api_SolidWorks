<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmFindUser Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmFindUser Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to search for users in the vault.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmFindUser ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmFindUser ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmFindUser ``` | |

# ![](dotnetimages/collapse.gif)Example

[Find Users (VB.NET)](Find_Users_Example_VBNET.htm)

[Find Users (C#)](Find_Users_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).

To access this interface, call [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html) with eType set to [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_FindUser.

SOLIDWORKS PDM Professional uses this interface internally when you have linked a card button to the **Find User** command.

This interface provides for both silent and interactive searches of users. Interactive searches display the same user interface that SOLIDWORKS PDM Professional displays when searching the vault for users.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFindUser Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)