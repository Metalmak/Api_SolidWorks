<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunCommand.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RunCommand Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RunCommand Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandID*
:   SOLIDWORKS command as defined in swCommands\_e (see Remarks)

*NewTitle*
:   Your title for the SOLIDWORKS PropertyManager page, if invoked by this command

Runs the specified SOLIDWORKS command.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunCommand( _    ByVal CommandID As System.Integer, _    ByVal NewTitle As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim CommandID As System.Integer Dim NewTitle As System.String Dim value As System.Boolean   value = instance.RunCommand(CommandID, NewTitle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RunCommand(     System.int CommandID,    System.string NewTitle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RunCommand(  &   System.int CommandID, &   System.String^ NewTitle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandID*
:   SOLIDWORKS command as defined in swCommands\_e (see Remarks)

*NewTitle*
:   Your title for the SOLIDWORKS PropertyManager page, if invoked by this command

#### Return Value

True if the SOLIDWORKS command ran, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RunCommand.

# ![](dotnetimages/collapse.gif)Example

[Fire Events When PropertyManager Page Opened and Canceled (VBA)](Fire_Events_When_PropertyManager_Page_Opened_and_Canceled_Example_VB.htm)

[Record Macros (C#)](Record_Macros_Example_CSharp.htm)

[Record Macros (VB.NET)](Record_Macros_Example_VBNET.htm)

[Record Macros (VBA)](Record_Macros_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[IModelDocExtension::RunCommand Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~RunCommand.html)

[ISldWorks::IsCommandEnabled Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IsCommandEnabled.html)

[ISldWorks::GetRunningCommandInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetRunningCommandInfo.html)

[DSldWorksEvents\_CommandCloseNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_CommandCloseNotifyEventHandler.html)

[DSldWorksEvents\_CommandOpenPreNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_CommandOpenPreNotifyEventHandler.html)

[ISldWorks::RecordLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLine.html)

[ISldWorks::RecordLineCSharp Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLineCSharp.html)

[ISldWorks::RecordLineVBnet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLineVBnet.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0