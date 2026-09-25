<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~MoveToFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MoveToFolder Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : MoveToFolder Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MoveToFeat*
:   Folder to which to move feature

*MoveFromFeat*
:   Folder from which to move feature

*IsFolder*
:   True if feature is a folder, false if a feature

Moves the selected feature or folder in the Solid Bodies Feature Manager design tree structure to the specified folder in the Solid Bodies Feature Manager design tree structure.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MoveToFolder( _    ByVal MoveToFeat As System.String, _    ByVal MoveFromFeat As System.String, _    ByVal IsFolder As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim MoveToFeat As System.String Dim MoveFromFeat As System.String Dim IsFolder As System.Boolean Dim value As System.Boolean   value = instance.MoveToFolder(MoveToFeat, MoveFromFeat, IsFolder) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MoveToFolder(     System.string MoveToFeat,    System.string MoveFromFeat,    System.bool IsFolder ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool MoveToFolder(  &   System.String^ MoveToFeat, &   System.String^ MoveFromFeat, &   System.bool IsFolder ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MoveToFeat*
:   Folder to which to move feature

*MoveFromFeat*
:   Folder from which to move feature

*IsFolder*
:   True if feature is a folder, false if a feature

#### Return Value

True if feature is moved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::MoveToFolder.

# ![](dotnetimages/collapse.gif)Remarks

This method is specific to the Solid Bodies folder only; it does not work for components.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0