<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWrapFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertWrapFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertWrapFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type of wrap as defined in swWrapSketchType\_e

*Thickness*
:   Thickness; 0.00001 (thinnest) - 10000 (thickest)

*ReverseDir*
:   True to reverse the direction of the wrap, false to not

Obsolete. Superseded by [IFeatureManager::InsertWrapFeature2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWrapFeature2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertWrapFeature( _    ByVal Type As System.Integer, _    ByVal Thickness As System.Double, _    ByVal ReverseDir As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Type As System.Integer Dim Thickness As System.Double Dim ReverseDir As System.Boolean Dim value As Feature   value = instance.InsertWrapFeature(Type, Thickness, ReverseDir) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertWrapFeature(     System.int Type,    System.double Thickness,    System.bool ReverseDir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertWrapFeature(  &   System.int Type, &   System.double Thickness, &   System.bool ReverseDir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Type of wrap as defined in swWrapSketchType\_e

*Thickness*
:   Thickness; 0.00001 (thinnest) - 10000 (thickest)

*ReverseDir*
:   True to reverse the direction of the wrap, false to not

#### Return Value

Wrap [feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertWrapFeature.

# ![](dotnetimages/collapse.gif)Example

[Change Wrap Feature Face (C#)](Change_Wrap_Feature_Face_Example_CSharp.htm)

[Change Wrap Feature Face (VB.NET)](Change_Wrap_Feature_Face_Example_VBNET.htm)

[Change Wrap Feature Face (VBA)](Change_Wrap_Feature_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) and these values to mark these selections:

* 1 = Face on which to place the wrap feature

* 2 = Pull direction if Type is swWrapSketchType\_e.swWrapSketchType\_Emboss or swWrapSketchType\_e.swWrapSketchType\_Engrave

  * 4 = 2D sketch of wrap feature; 3D sketches are invalid

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IWrapSketchFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWrapSketchFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0