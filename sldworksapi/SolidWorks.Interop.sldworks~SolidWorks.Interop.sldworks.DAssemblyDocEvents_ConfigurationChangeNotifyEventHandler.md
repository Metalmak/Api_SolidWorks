<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_ConfigurationChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_ConfigurationChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_ConfigurationChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ConfigurationName*
:   Name of the configuration that has changed

*Object*
:   Object that has changed

*ObjectType*
:   Type of the object that has changed as defined in swSelectType\_e:

    * swSelDIMENSIONS* swSelDATUMPOINTS* swSelDATUMPLANES* swSelDATUMAXES* swSelHELIX* swSelBODYFEATURES* swSelMATEGROUP* swSelMATES* swSelCOORDSYS* swSelCOMPONENTS* swSelCONFIGURATIONS* swSelSKETCHES* swSelREFCURVES* swSelDISPLAYSTATE

    All other types are returned as swSelUNSUPPORTED.

*changeType*
:   Type of change as defined by swConfigurationChangeTypes\_e

Gets information about an object or feature that has had one of its configurable parameters changed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_ConfigurationChangeNotifyEventHandler( _    ByVal ConfigurationName As System.String, _    ByVal Object As System.Object, _    ByVal ObjectType As System.Integer, _    ByVal changeType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_ConfigurationChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ConfigurationChangeNotifyEventHandler(     System.string ConfigurationName,    System.object Object,    System.int ObjectType,    System.int changeType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ConfigurationChangeNotifyEventHandler(  &   System.String^ ConfigurationName, &   System.Object^ Object, &   System.int ObjectType, &   System.int changeType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ConfigurationName*
:   Name of the configuration that has changed

*Object*
:   Object that has changed

*ObjectType*
:   Type of the object that has changed as defined in swSelectType\_e:

    * swSelDIMENSIONS* swSelDATUMPOINTS* swSelDATUMPLANES* swSelDATUMAXES* swSelHELIX* swSelBODYFEATURES* swSelMATEGROUP* swSelMATES* swSelCOORDSYS* swSelCOMPONENTS* swSelCONFIGURATIONS* swSelSKETCHES* swSelREFCURVES* swSelDISPLAYSTATE

    All other types are returned as swSelUNSUPPORTED.

*changeType*
:   Type of change as defined by swConfigurationChangeTypes\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationChangeNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblyConfigurationChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0