<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~SetDroppedFileConfigName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDroppedFileConfigName Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : SetDroppedFileConfigName Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ConfigName*
:   Name of the configuration to set

Sets the configuration name for the recently dropped file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDroppedFileConfigName( _    ByVal ConfigName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim ConfigName As System.String Dim value As System.Boolean   value = instance.SetDroppedFileConfigName(ConfigName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDroppedFileConfigName(     System.string ConfigName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDroppedFileConfigName(  &   System.String^ ConfigName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ConfigName*
:   Name of the configuration to set

#### Return Value

True if the name is successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::SetDroppedFileConfigName.

# ![](dotnetimages/collapse.gif)Remarks

If the configuration name is set in response to the [FileDropNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DAssemblyDocEvents_FileDropNotifyEventHandler.html) event, SOLIDWORKS does not display the dialog for the selected configuration names when a file is dropped in an assembly.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::SetDroppedFileName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~SetDroppedFileName.html)

[IAssemblyDoc::GetDroppedAtEntity Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~GetDroppedAtEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99 SP03, datecode 1999271