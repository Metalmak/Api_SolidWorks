<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetFavLibraryMaterialToSelectedEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFavLibraryMaterialToSelectedEntities Method (ICWSolidManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html) : SetFavLibraryMaterialToSelectedEntities Method (ICWSolidManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SFavLibName*
:   Name of favorite material library

*SFavMaterialName*
:   Name of material in SFavLibName

Applies the specified favorite library material to selected entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFavLibraryMaterialToSelectedEntities( _    ByVal SFavLibName As System.String, _    ByVal SFavMaterialName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidManager Dim SFavLibName As System.String Dim SFavMaterialName As System.String Dim value As System.Integer   value = instance.SetFavLibraryMaterialToSelectedEntities(SFavLibName, SFavMaterialName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFavLibraryMaterialToSelectedEntities(     System.string SFavLibName,    System.string SFavMaterialName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFavLibraryMaterialToSelectedEntities(  &   System.String^ SFavLibName, &   System.String^ SFavMaterialName ) ``` | |

#### Parameters

*SFavLibName*
:   Name of favorite material library

*SFavMaterialName*
:   Name of material in SFavLibName

#### Return Value

0 if material library and material name are set, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSolidManager::SetFavLibraryMaterialToSelectedEntities.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, select one or more components to which to apply the specified favorite library material.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html)

[ICWSolidManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager_members.html)

[ICWSolidManager::SetLibraryMaterialToSelectedEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetLibraryMaterialToSelectedEntities.html)

[ICWSolidManager::SetFavLibraryMaterialToAllBodiesByCompName Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetFavLibraryMaterialToAllBodiesByCompName.html)

[ICWSolidManager::SetLibraryMaterialToAllBodiesByCompName Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetLibraryMaterialToAllBodiesByCompName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0