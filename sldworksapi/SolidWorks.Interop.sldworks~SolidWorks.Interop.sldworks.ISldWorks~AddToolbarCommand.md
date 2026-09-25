<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbarCommand.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddToolbarCommand Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddToolbarCommand Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModuleName*

*ToolbarId*

*ToolbarIndex*

*CommandString*

Obsolete. Superseded by [ISldWorks::AddToolbarCommand2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~AddToolbarCommand2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddToolbarCommand( _    ByVal ModuleName As System.String, _    ByVal ToolbarId As System.Integer, _    ByVal ToolbarIndex As System.Integer, _    ByVal CommandString As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim ModuleName As System.String Dim ToolbarId As System.Integer Dim ToolbarIndex As System.Integer Dim CommandString As System.String Dim value As System.Boolean   value = instance.AddToolbarCommand(ModuleName, ToolbarId, ToolbarIndex, CommandString) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddToolbarCommand(     System.string ModuleName,    System.int ToolbarId,    System.int ToolbarIndex,    System.string CommandString ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddToolbarCommand(  &   System.String^ ModuleName, &   System.int ToolbarId, &   System.int ToolbarIndex, &   System.String^ CommandString ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModuleName*

*ToolbarId*

*ToolbarIndex*

*CommandString*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddToolbarCommand.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)