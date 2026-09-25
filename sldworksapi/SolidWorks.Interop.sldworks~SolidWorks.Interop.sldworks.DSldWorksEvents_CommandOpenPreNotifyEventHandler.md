<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_CommandOpenPreNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_CommandOpenPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_CommandOpenPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Command*
:   SOLIDWORKS command ID as defined in swCommands\_e

*UserCommand*
:   Third-party application's command item's ID (see **Remarks**)

Fired before a command, including a PropertyManager page, executes or opens.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_CommandOpenPreNotifyEventHandler( _    ByVal Command As System.Integer, _    ByVal UserCommand As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_CommandOpenPreNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_CommandOpenPreNotifyEventHandler(     System.int Command,    System.int UserCommand ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_CommandOpenPreNotifyEventHandler(  &   System.int Command, &   System.int UserCommand ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Command*
:   SOLIDWORKS command ID as defined in swCommands\_e

*UserCommand*
:   Third-party application's command item's ID (see **Remarks**)

#### Return Value

0 to execute the command or open a PropertyManager page, 1 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CommandOpenPreNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Example

[Fire Events When PropertyManager Page Opened and Canceled (VBA)](Fire_Events_When_PropertyManager_Page_Opened_and_Canceled_Example_VB.htm)

[Fire Events When PropertyManager Page Opened and Canceled (VB.NET)](Fire_Events_When_PropertyManager_Page_Opened_and_Canceled_Example_VBNET.htm)

[Fire Events When PropertyManager Page Opened and Canceled (C#)](Fire_Events_When_PropertyManager_Page_Opened_and_Canceled_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAppCommandOpenPreNotify to register for this notification.

The UserCommand argument is the ID assigned to your application's command item when it was added to a CommandGroup. For example:

```
cmdIndex0 = cmdGroup.AddCommandItem("CreateCube", -1, "Create a cube", "Create cube", 0, "CreateCube", "", 0);
```

```
cmdIds[0] = cmdGroup.get_CommandID(cmdIndex0);
```

Selecting the **Create cube** command in the user interface causes the CommandOpenPreNotify event to fire. The Command parameter is swCommands\_e.swCommands\_User\_Toolbar\_Min, and the userCommand parameter is cmdIDs[0].

Call [CommandCloseNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_CommandCloseNotifyEventHandler.html) to fire an event when the PropertyManager page is okay'd or canceled.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0