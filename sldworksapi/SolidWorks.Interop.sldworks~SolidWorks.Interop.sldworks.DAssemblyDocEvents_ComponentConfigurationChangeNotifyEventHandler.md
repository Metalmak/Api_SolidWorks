<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_ComponentConfigurationChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_ComponentConfigurationChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_ComponentConfigurationChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*componentName*
:   Name of reference component whose configuration is changing

*oldConfigurationName*
:   Old name of reference component's configuration

*newConfigurationName*
:   New name of reference component's configuration

Fired when a reference component's configuration is being changed in an assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_ComponentConfigurationChangeNotifyEventHandler( _    ByVal componentName As System.String, _    ByVal oldConfigurationName As System.String, _    ByVal newConfigurationName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_ComponentConfigurationChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ComponentConfigurationChangeNotifyEventHandler(     System.string componentName,    System.string oldConfigurationName,    System.string newConfigurationName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ComponentConfigurationChangeNotifyEventHandler(  &   System.String^ componentName, &   System.String^ oldConfigurationName, &   System.String^ newConfigurationName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*componentName*
:   Name of reference component whose configuration is changing

*oldConfigurationName*
:   Old name of reference component's configuration

*newConfigurationName*
:   New name of reference component's configuration

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ComponentConfigurationChangeNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Notification When Changing Configuration of Reference Component (C#)](Fire_Notification_When_Changing_Configuration_of_Reference_Component_Example_CSharp.htm)

[Fire Notification When Changing Configuration of Reference Component (VB.NET)](Fire_Notification_When_Changing_Configuration_of_Reference_Component__Example_VBNET.htm)

[Fire Notification When Changing Configuration of Reference Component (VBA)](Fire_Notification_When_Changing_Configuration_of_Reference_Component_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblyComponentConfigurationChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP4, Revision Number 17.4