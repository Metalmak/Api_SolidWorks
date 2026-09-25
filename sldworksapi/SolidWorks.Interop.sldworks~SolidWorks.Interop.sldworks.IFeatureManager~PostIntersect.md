<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PostIntersect.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PostIntersect Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : PostIntersect Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IntersectionsToExclude*
:   Array of booleans indicating which bodies returned by [IFeatureManager::PreIntersect](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~PreIntersect.html) to exclude from this intersect feature

*Merge*
:   True to merge all intersect regions into one body, false to not

*Consume*
:   True to remove input surfaces from the FeatureManager design tree, false to not

Creates an intersect feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function PostIntersect( _    ByVal IntersectionsToExclude As System.Object, _    ByVal Merge As System.Boolean, _    ByVal Consume As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim IntersectionsToExclude As System.Object Dim Merge As System.Boolean Dim Consume As System.Boolean Dim value As Feature   value = instance.PostIntersect(IntersectionsToExclude, Merge, Consume) ``` | |

| C# |  |
| --- | --- |
| ``` Feature PostIntersect(     System.object IntersectionsToExclude,    System.bool Merge,    System.bool Consume ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ PostIntersect(  &   System.Object^ IntersectionsToExclude, &   System.bool Merge, &   System.bool Consume ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IntersectionsToExclude*
:   Array of booleans indicating which bodies returned by [IFeatureManager::PreIntersect](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~PreIntersect.html) to exclude from this intersect feature

*Merge*
:   True to merge all intersect regions into one body, false to not

*Consume*
:   True to remove input surfaces from the FeatureManager design tree, false to not

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::PostIntersect.

# ![](dotnetimages/collapse.gif)Example

[Get Intersect Feature Data (VBA)](Get_Intersect_Feature_Data_Example_VB.htm)

[Get Intersect Feature Data (VB.NET)](Get_Intersect_Feature_Data_Example_VBNET.htm)

[Get Intersect Feature Data (C#)](Get_Intersect_Feature_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call [IFeatureManager::PreIntersect](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~PreIntersect.html) to obtain the intersect bodies.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IIntersectFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIntersectFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0