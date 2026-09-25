<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~AddCommands.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddCommands Method (ICommandTabBox) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html) : AddCommands Method (ICommandTabBox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandIDs*
:   Array of command IDs for the buttons (see **Remarks**)

*TextDisplayStyles*
:   Array of the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

Adds buttons to this CommandManager tab box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCommands( _    ByVal CommandIDs As System.Object, _    ByVal TextDisplayStyles As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICommandTabBox Dim CommandIDs As System.Object Dim TextDisplayStyles As System.Object Dim value As System.Boolean   value = instance.AddCommands(CommandIDs, TextDisplayStyles) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddCommands(     System.object CommandIDs,    System.object TextDisplayStyles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddCommands(  &   System.Object^ CommandIDs, &   System.Object^ TextDisplayStyles ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandIDs*
:   Array of command IDs for the buttons (see **Remarks**)

*TextDisplayStyles*
:   Array of the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

#### Return Value

True if the buttons are added to the CommandManager tab box, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CommandTabBox::AddCommands.

# ![](dotnetimages/collapse.gif)Example

[Create CommandManager Tab and Tab Boxes (VB.NET)](Create_CommandManager_Tab_and_Tab_Boxes_Example_VB.NET.htm)

[Create CommandManager Tab and Tab Boxes (C#)](Create_CommandManager_Tab_and_Tab_Boxes_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can add both CommandGroup and FlyoutGroup items to CommandManager. Populate CommandIDs by calling [IFlyoutGroup::CmdID](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFlyoutGroup~CmdID.html) for FlyoutGroups and [ICommandGroup::CommandID](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~CommandID.html) or [ICommandGroup::ToolbarId](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~ToolbarId.html) after calling [ICommandGroup::Activate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~Activate.html) for CommandGroups.

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html)

[ICommandTabBox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox_members.html)

[ICommandTabBox::IAddCommands Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~IAddCommands.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0