<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTab~AddSeparator.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddSeparator Method (ICommandTab) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICommandTab Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTab.html) : AddSeparator Method (ICommandTab) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandTabBoxIn*
:   [CommandManager tab box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandTabBox.html) to which to add the separator

*CommandID*
:   Button before which to place the separator (see Remarks)

Adds a separator to this CommandManager tab.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddSeparator( _    ByVal CommandTabBoxIn As CommandTabBox, _    ByVal CommandID As System.Integer _ ) As CommandTabBox ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICommandTab Dim CommandTabBoxIn As CommandTabBox Dim CommandID As System.Integer Dim value As CommandTabBox   value = instance.AddSeparator(CommandTabBoxIn, CommandID) ``` | |

| C# |  |
| --- | --- |
| ``` CommandTabBox AddSeparator(     CommandTabBox CommandTabBoxIn,    System.int CommandID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CommandTabBox^ AddSeparator(  &   CommandTabBox^ CommandTabBoxIn, &   System.int CommandID ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandTabBoxIn*
:   [CommandManager tab box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandTabBox.html) to which to add the separator

*CommandID*
:   Button before which to place the separator (see Remarks)

#### Return Value

New [CommandManager tab box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandTabBox.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CommandTab::AddSeparator.

# ![](dotnetimages/collapse.gif)Example

[Create CommandManager Tab and Tab Boxes (VB.NET)](Create_CommandManager_Tab_and_Tab_Boxes_Example_VB.NET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The specified CommandManager tab is split into two. The left side is the original CommandManager tab box, and the right side is the new CommandManager tab box. The first button on the new CommandManager tab box is the button specified by CommandID.

If the CommandManager tab box has multiple commands with the same CommandID, then a separator is added before the first matching CommandID.

You can get the CommandID using [ICommandGroup::CommandID](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~CommandID.html) or [ICommandGroup::ToolbarId](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~ToolbarId.html) after calling [ICommandGroup::Activate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~Activate.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandTab Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTab.html)

[ICommandTab Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTab_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0