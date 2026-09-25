<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmFolder7 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmFolder7 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access the contents of a file system folder in the vault.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmFolder7     Inherits IEdmFolder5, IEdmFolder6, IEdmObject5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmFolder7 : IEdmFolder5, IEdmFolder6, IEdmObject5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmFolder7 : public IEdmFolder5, IEdmFolder6, IEdmObject5  ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* extends [IEdmFolder6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html) by adding the ability to destroy deleted items in this folder.* is extended by [IEdmFolder8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8.html) by adding the ability to add or copy a file, which already exists in the vault, to a different folder in the vault.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)