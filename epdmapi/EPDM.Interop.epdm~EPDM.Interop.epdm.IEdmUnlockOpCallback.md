<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmUnlockOpCallback Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmUnlockOpCallback Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access information and gain control of [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) operations.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmUnlockOpCallback ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmUnlockOpCallback ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmUnlockOpCallback ``` | |

# ![](dotnetimages/collapse.gif)Example

[Access Check-in Flags in Check out Dialog (C#)](Access_Check-in_Flags_in_Check_in_Dialog_Example_CSharp.htm)

[Access Check-in Flags in Check out Dialog (VB.NET)](Access_Check-in_Flags_in_Check_in_Dialog_Example_VBNET.htm)

[Prevent Admin from Checking In File (C#)](Prevent_Admin_from_Checking_In_File_Example_CSharp.htm)

[Prevent Admin from Checking In File (VB.NET)](Prevent_Admin_from_Checking_In_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IUnknown. See [Using and Implementing IUnknown (COM)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms693423%28v%3Dvs.85%29.aspx).

To use this callback interface:

1. Create a new class.- Implement all of the methods of this interface in the new class.- Call [IEdmBatchUnlock::CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~CreateTree.html) or [IEdmBatchUnlock::UnlockFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~UnlockFiles.html), setting poCallback to a pointer to the new class.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUnlockOpCallback Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)