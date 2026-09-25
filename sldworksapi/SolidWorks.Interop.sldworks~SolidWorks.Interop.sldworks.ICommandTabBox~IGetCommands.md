<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~IGetCommands.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetCommands Method (ICommandTabBox) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html) : IGetCommands Method (ICommandTabBox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandIDs*
:   * in-process, unmanaged C++: Pointer to an array of command IDs (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*TextDisplayStyles*
:   * in-process, unmanaged C++: Pointer to an array the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method

Gets the buttons' Command IDs, text display styles, and number of commands on the CommandManager tab box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetCommands( _    ByRef CommandIDs As System.Integer, _    ByRef TextDisplayStyles As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICommandTabBox Dim CommandIDs As System.Integer Dim TextDisplayStyles As System.Integer Dim value As System.Integer   value = instance.IGetCommands(CommandIDs, TextDisplayStyles) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetCommands(     out System.int CommandIDs,    out System.int TextDisplayStyles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetCommands(  &   [Out] System.int CommandIDs, &   [Out] System.int TextDisplayStyles ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandIDs*
:   * in-process, unmanaged C++: Pointer to an array of command IDs (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*TextDisplayStyles*
:   * in-process, unmanaged C++: Pointer to an array the text display styles for the buttons as defined in swCommandTabButtonTextDisplay\_e

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method

#### Return Value

Number of buttons on this CommandManager tab box

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CommandTabBox::IGetCommands.

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandTabBox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox.html)

[ICommandTabBox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox_members.html)

[ICommandTabBox::GetCommands Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandTabBox~GetCommands.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0