<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureManager.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureManager Property (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : FeatureManager Property (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the [IFeatureManager](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager.html) object, which allows access to the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property FeatureManager As FeatureManager ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim value As FeatureManager   value = instance.FeatureManager ``` | |

| C# |  |
| --- | --- |
| ``` FeatureManager FeatureManager {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property FeatureManager^ FeatureManager {    FeatureManager^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

[IFeatureManager](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::FeatureManager.

# ![](dotnetimages/collapse.gif)Example

[Insert Macro Feature (C++)](Insert_Macro_Feature_Example_CPlusPlus_COM.htm)

[Insert DXF File and Add Dimension (VBA)](Insert_DXF_File_and_Add_Dimension_Example_VB.htm)

[Insert Folder in FeatureManager Design Tree (VBA)](Insert_Folder_in_FeatureManager_Design_Tree_Example_VB.htm)

[Insert Reference POints (VBA)](Insert_Reference_Points_Example_VB.htm)

[Update FeatureManager Design Tree (VBA)](Update_FeatureManager_Design_Tree_Example_VB.htm)

[Insert MidSurface in Component (C#)](Insert_MidSurface_in_Component_Example_CSharp.htm)

[Insert MidSurface in Component (VB.NET)](Insert_MidSurface_in_Component_Example_VBNET.htm)

[Insert MidSurface in Component (VBA)](Insert_MidSurface_in_Component_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0