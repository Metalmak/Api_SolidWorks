<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetEditStatus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetEditStatus Method (IFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : GetEditStatus Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the feature can currently be edited.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEditStatus() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim value As System.Integer   value = instance.GetEditStatus() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetEditStatus() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetEditStatus(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Editing status of feature as defined in swFeatureEditStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::GetEditStatus.

# ![](dotnetimages/collapse.gif)Example

[Get Editing Status of Features (VB.NET)](Get_Editing_Status_of_Features_Example_VBNET.htm)

[Get Editing Status of Features (VBA)](Get_Editing_Status_of_Features_Example_VB.htm)

[Get Editing Status of Features (C#)](Get_Editing_Status_of_Features_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Although swFeatureEditStatus\_e is a bitmask, you currently cannot combine its mutually exclusive enumerators and you must examine the bit value of the return value for the editing status of the feature.

|  |  |
| --- | --- |
| **If...** | **Then the return value will be...** |
| a feature and all of its dependent items are not currently being edited | 0 (swFeature\_Editable) for the feature and all of its dependent items |
| a feature is currently being edited | 1 (swFeature\_NonEditable); this will also be the return value for all of the feature's dependent items |
| a sketch is currently being edited | 2 (swFeature\_UnderEditing) |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0