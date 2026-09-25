<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetCommandID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCommandID Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetCommandID Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Clsid*
:   Add-in's class ID

*UserCmdID*
:   User-defined command ID for the add-in's control (see **Remarks**)

Gets the SOLIDWORKS command ID for an instance of an add-in's control (e.g., an add-in's toolbar button).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCommandID( _    ByVal Clsid As System.String, _    ByVal UserCmdID As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Clsid As System.String Dim UserCmdID As System.Integer Dim value As System.Integer   value = instance.GetCommandID(Clsid, UserCmdID) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCommandID(     System.string Clsid,    System.int UserCmdID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCommandID(  &   System.String^ Clsid, &   System.int UserCmdID ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Clsid*
:   Add-in's class ID

*UserCmdID*
:   User-defined command ID for the add-in's control (see **Remarks**)

#### Return Value

Actual runtime value that SOLIDWORKS assigned the add-in's control

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetCommandID.

# ![](dotnetimages/collapse.gif)Remarks

UserCmdId is the same user-defined command ID specified when you created the add-in control using [ICommandGroup::AddCommandItem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~AddCommandItem2.html). You need the SOLIDWORKS command ID if you want to do something like cause an add-in's toolbar button to flash when visible in SOLIDWORKS.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ICommandGroup::CommandID Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~CommandID.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP2, Revision Number 14.2