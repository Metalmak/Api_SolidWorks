<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBomMgr2 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBomMgr2 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access the Bill of Materials (BOM) layouts installed in a vault.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBomMgr2     Inherits IEdmBomMgr  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBomMgr2 : IEdmBomMgr  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBomMgr2 : public IEdmBomMgr  ``` | |

# ![](dotnetimages/collapse.gif)Example

[Access Bill of Materials (VB.NET)](Access_Bill_of_Materials_Example_VBNET.htm)

[Access Bill of Materials (C#)](Access_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface:

   - Extends [IEdmBomMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr.html) by providing:

+ support for Web 2 applications,+ the ability to determine whether a specified user can see a specified BOM layout, and+ a new layout structure, [EdmBomLayout2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2.html), that includes BOM type information.

   - Is extended by [IEdmBomMgr3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html).

To view a vault's BOM layouts in the SOLIDWORKS PDM Professional Administration tool, log in to a vault and expand **Bills of Materials**.

To access this interface, call IEdmVault7::CreateUtility with eType = [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_BomMgr.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomMgr2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)