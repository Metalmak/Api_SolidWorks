<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~IAddCommands.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddCommands Method (ICommandTabBox) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html) : IAddCommands Method (ICommandTabBox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandIDCount*
:   Number of buttons to add

*CommandIDs*
:   * in-process, unmanaged C++: Pointer to an array of command IDs (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*TextDisplayStyles*
:   * in-process, unmanaged C++: Pointer to an array the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

Adds buttons to this CommandManager tab box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddCommands( _    ByVal CommandIDCount As System.Integer, _    ByRef CommandIDs As System.Integer, _    ByRef TextDisplayStyles As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICommandTabBox Dim CommandIDCount As System.Integer Dim CommandIDs As System.Integer Dim TextDisplayStyles As System.Integer Dim value As System.Boolean   value = instance.IAddCommands(CommandIDCount, CommandIDs, TextDisplayStyles) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IAddCommands(     System.int CommandIDCount,    ref System.int CommandIDs,    ref System.int TextDisplayStyles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IAddCommands(  &   System.int CommandIDCount, &   System.int% CommandIDs, &   System.int% TextDisplayStyles ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandIDCount*
:   Number of buttons to add

*CommandIDs*
:   * in-process, unmanaged C++: Pointer to an array of command IDs (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*TextDisplayStyles*
:   * in-process, unmanaged C++: Pointer to an array the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

#### Return Value

True if the buttons are added to the CommandManager tab box, false if not

# ![](dotnetimages/collapse.gif)Remarks

You can get the CommandID values using [ICommandGroup::CommandID](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~CommandID.html) or [ICommandGroup::ToolbarId](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~ToolbarId.html) after calling [ICommandGroup::Activate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~Activate.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html)

[ICommandTabBox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox_members.html)

[ICommandTabBox::AddCommands Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~AddCommands.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0