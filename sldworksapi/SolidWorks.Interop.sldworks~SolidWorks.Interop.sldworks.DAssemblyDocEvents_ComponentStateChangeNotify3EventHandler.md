<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_ComponentStateChangeNotify3EventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_ComponentStateChangeNotify3EventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_ComponentStateChangeNotify3EventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Component*
:   [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)

*CompName*
:   Name of the component

*oldCompState*
:   Previous state of the component as defined in swComponentSuppressionState\_e

*newCompState*
:   New state of the component as defined in swComponentSuppressionState\_e

Fired whenever the state of a component within this assembly changes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_ComponentStateChangeNotify3EventHandler( _    ByVal Component As System.Object, _    ByVal CompName As System.String, _    ByVal oldCompState As System.Short, _    ByVal newCompState As System.Short _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_ComponentStateChangeNotify3EventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ComponentStateChangeNotify3EventHandler(     System.object Component,    System.string CompName,    System.short oldCompState,    System.short newCompState ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ComponentStateChangeNotify3EventHandler(  &   System.Object^ Component, &   System.String^ CompName, &   System.short oldCompState, &   System.short newCompState ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Component*
:   [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)

*CompName*
:   Name of the component

*oldCompState*
:   Previous state of the component as defined in swComponentSuppressionState\_e

*newCompState*
:   New state of the component as defined in swComponentSuppressionState\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ComponentStateChangeNotify3 Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblyComponentStateChangeNotify3 to register for this notification.

SOLIDWORKS sends this notification:

* even if the assembly is not the active document.* when a component gets suppressed due to an internal ID mismatch.* not at all if a part is explicitly opened by the user or opened programmatically. In that case, SOLIDWORKS resolves the component part in any open assembly that references it. Your application must watch for the SOLIDWORKS event [FileOpenNotify2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_FileOpenNotify2EventHandler.html).

When a component is resolved or unsuppressed, its model document becomes available to your application. Within this notification, you can get this object and register for other events. This might be useful for project data management (PDM) applications that want to ask the user to check out the assembly component if the user tries to make changes.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0