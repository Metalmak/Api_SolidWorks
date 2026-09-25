<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetFavLibraryMaterialToAllBodiesByCompName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFavLibraryMaterialToAllBodiesByCompName Method (ICWSolidManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html) : SetFavLibraryMaterialToAllBodiesByCompName Method (ICWSolidManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SCompName*
:   Name of component

*SFavLibName*
:   Name of favorite material library

*SFavMaterialName*
:   Name of material in SFavLibName

Applies the specified favorite library material to all bodies in the specified component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFavLibraryMaterialToAllBodiesByCompName( _    ByVal SCompName As System.String, _    ByVal SFavLibName As System.String, _    ByVal SFavMaterialName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidManager Dim SCompName As System.String Dim SFavLibName As System.String Dim SFavMaterialName As System.String Dim value As System.Integer   value = instance.SetFavLibraryMaterialToAllBodiesByCompName(SCompName, SFavLibName, SFavMaterialName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFavLibraryMaterialToAllBodiesByCompName(     System.string SCompName,    System.string SFavLibName,    System.string SFavMaterialName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFavLibraryMaterialToAllBodiesByCompName(  &   System.String^ SCompName, &   System.String^ SFavLibName, &   System.String^ SFavMaterialName ) ``` | |

#### Parameters

*SCompName*
:   Name of component

*SFavLibName*
:   Name of favorite material library

*SFavMaterialName*
:   Name of material in SFavLibName

#### Return Value

0 if material library and material name are set, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSolidManager::SetFavLibraryMaterialToAllBodiesByCompName.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html)

[ICWSolidManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager_members.html)

[ICWSolidManager::SetLibraryMaterialToAllBodiesByCompName Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetLibraryMaterialToAllBodiesByCompName.html)

[ICWSolidManager::SetFavLibraryMaterialToSelectedEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetFavLibraryMaterialToSelectedEntities.html)

[ICWSolidManager::SetLibraryMaterialToSelectedEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetLibraryMaterialToSelectedEntities.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0