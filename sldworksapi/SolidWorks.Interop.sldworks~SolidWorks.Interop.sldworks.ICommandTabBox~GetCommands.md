<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~GetCommands.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCommands Method (ICommandTabBox) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html) : GetCommands Method (ICommandTabBox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandIDs*
:   Array of command IDs for the buttons

*TextDisplayStyles*
:   Array of the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

Gets the buttons' command IDs, text display styles, and number of commands on the CommandManager tab box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCommands( _    ByRef CommandIDs As System.Object, _    ByRef TextDisplayStyles As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICommandTabBox Dim CommandIDs As System.Object Dim TextDisplayStyles As System.Object Dim value As System.Integer   value = instance.GetCommands(CommandIDs, TextDisplayStyles) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCommands(     out System.object CommandIDs,    out System.object TextDisplayStyles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCommands(  &   [Out] System.Object^ CommandIDs, &   [Out] System.Object^ TextDisplayStyles ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandIDs*
:   Array of command IDs for the buttons

*TextDisplayStyles*
:   Array of the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

#### Return Value

Number of buttons on this CommandManager tab box

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CommandTabBox::GetCommands.

# ![](dotnetimages/collapse.gif)Example

[Create CommandManager Tab and Tab Boxes (C#)](Create_CommandManager_Tab_and_Tab_Boxes_Example_CSharp.htm)

[Create CommandManager Tab and Tab Boxes (VB.NET)](Create_CommandManager_Tab_and_Tab_Boxes_Example_VB.NET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html)

[ICommandTabBox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox_members.html)

[ICommandTabBox::IGetCommands Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~IGetCommands.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0