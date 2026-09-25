<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetLibraryMaterialToAllBodiesByCompName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetLibraryMaterialToAllBodiesByCompName Method (ICWSolidManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html) : SetLibraryMaterialToAllBodiesByCompName Method (ICWSolidManager) |

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

*SLibName*
:   Name of material library

*SMaterialName*
:   Name of material in SLibName

Applies the specified library material to all bodies in the specified component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLibraryMaterialToAllBodiesByCompName( _    ByVal SCompName As System.String, _    ByVal SLibName As System.String, _    ByVal SMaterialName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidManager Dim SCompName As System.String Dim SLibName As System.String Dim SMaterialName As System.String Dim value As System.Integer   value = instance.SetLibraryMaterialToAllBodiesByCompName(SCompName, SLibName, SMaterialName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetLibraryMaterialToAllBodiesByCompName(     System.string SCompName,    System.string SLibName,    System.string SMaterialName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetLibraryMaterialToAllBodiesByCompName(  &   System.String^ SCompName, &   System.String^ SLibName, &   System.String^ SMaterialName ) ``` | |

#### Parameters

*SCompName*
:   Name of component

*SLibName*
:   Name of material library

*SMaterialName*
:   Name of material in SLibName

#### Return Value

0 if material library and material name are set, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSolidManager::SetLibraryMaterialToAllBodiesByCompName.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html)

[ICWSolidManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager_members.html)

[ICWSolidManager::SetFavLibraryMaterialToAllBodiesByCompName Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetFavLibraryMaterialToAllBodiesByCompName.html)

[ICWSolidManager::SetFavLibraryMaterialToSelectedEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetFavLibraryMaterialToSelectedEntities.html)

[ICWSolidManager::SetLibraryMaterialToSelectedEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~SetLibraryMaterialToSelectedEntities.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0