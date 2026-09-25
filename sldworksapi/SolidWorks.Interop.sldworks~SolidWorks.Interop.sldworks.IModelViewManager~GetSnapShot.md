<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~GetSnapShot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSnapShot Method (IModelViewManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html) : GetSnapShot Method (IModelViewManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SnapShotName*
:   Name of snapshot to get

Gets the specified snapshot of an assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSnapShot( _    ByVal SnapShotName As System.String _ ) As SnapShot ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelViewManager Dim SnapShotName As System.String Dim value As SnapShot   value = instance.GetSnapShot(SnapShotName) ``` | |

| C# |  |
| --- | --- |
| ``` SnapShot GetSnapShot(     System.string SnapShotName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SnapShot^ GetSnapShot(  &   System.String^ SnapShotName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SnapShotName*
:   Name of snapshot to get

#### Return Value

[ISnapShot](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISnapShot.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelViewManager::GetSnapShot.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for assemblies.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html)

[IModelViewManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager_members.html)

[IModelViewManager::AddSnapShot Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~AddSnapShot.html)

[IModelViewManager::DeleteSnapShot Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~DeleteSnapShot.html)

[IModelViewManager::GetSnapShots Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~GetSnapShots.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0