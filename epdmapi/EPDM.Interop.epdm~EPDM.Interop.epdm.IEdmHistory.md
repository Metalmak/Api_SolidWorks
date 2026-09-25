<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmHistory Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmHistory Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access the history listing of files or folders.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmHistory ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmHistory ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmHistory ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get Histories of Files (VB.NET)](Get_Histories_of_Files_Example_VBNET.htm)

[Get Histories of Files (C#)](Get_Histories_of_Files_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmHistory2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory2.html).

To access this interface, call [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html) with eType set to [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_History.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistory Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)