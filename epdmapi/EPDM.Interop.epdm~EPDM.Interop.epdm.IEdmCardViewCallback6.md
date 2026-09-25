<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmCardViewCallback6 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmCardViewCallback6 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Handles customized loading and saving of data in a card view.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmCardViewCallback6 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmCardViewCallback6 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmCardViewCallback6 ``` | |

# ![](dotnetimages/collapse.gif)Example

[Create Custom Card View (VB.NET)](Create_Custom_Card_View_Example_VBNET.htm)

[Create Custom Card View (C#)](Create_Custom_Card_View_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IUnknown. See [Using and Implementing IUnknown (COM)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms693423%28v%3Dvs.85%29.aspx).

This callback interface allows you to customize how data is loaded and saved in a simple card view that is created using [IEdmVault10::CreateCardViewEx2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault10~CreateCardViewEx2.html). To use this callback interface:

1. Create a new class.- Implement all of the methods of IEdmCardViewCallback6 in the new class.- Call IEdmVault10::CreateCardViewEx2, setting poCallback to a pointer to the new class.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardViewCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)