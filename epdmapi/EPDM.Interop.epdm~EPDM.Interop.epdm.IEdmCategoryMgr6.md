<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmCategoryMgr6 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmCategoryMgr6 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access all of the categories that have been set up in a vault.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmCategoryMgr6 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmCategoryMgr6 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmCategoryMgr6 ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get Categories (VB.NET)](Get_Categories_Example_VBNET.htm)

[Get Categories (C#)](Get_Categories_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).

To access this interface, call IEdmVault7::CreateUtility with eType = [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_CategoryMgr.

Files in SOLIDWORKS PDM Professional can be categorized according to certain criteria such as card properties, file extensions, etc. The categories are set up using SOLIDWORKS PDM Professional’s administration tool.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCategoryMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmCategory6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategory6.html)