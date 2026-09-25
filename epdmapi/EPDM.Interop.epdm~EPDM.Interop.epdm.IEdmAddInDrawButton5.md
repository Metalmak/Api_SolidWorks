<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmAddInDrawButton5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmAddInDrawButton5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to dynamically draw an add-in toolbar button.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmAddInDrawButton5 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmAddInDrawButton5 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmAddInDrawButton5 ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IUnknown. See [Using and Implementing IUnknown (COM)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms693423%28v%3Dvs.85%29.aspx).

To dynamically draw a toolbar button:

1. Create a class that implements both [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) and IEdmAddInDrawButton5.- Implement [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html), calling [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html) with lEdmMenuFlags setting the [EdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html).EdmMenu\_OwnerDrawToolbarButton flag.- Implement [IEdmAddInDrawButton5::DrawToolbarButton](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5~DrawToolbarButton.html) to draw a toolbar button when called by SOLIDWORKS PDM Professional.

To draw a fixed toolbar button:

1. Call [IEdmCmdMgr5::AddToolbarImage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddToolbarImage.html).- Call IEdmCmdMgr5::AddCmd, passing in the toolbar button image ID used in IEdmCmdMgr5::AddToolbarImage.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInDrawButton5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)