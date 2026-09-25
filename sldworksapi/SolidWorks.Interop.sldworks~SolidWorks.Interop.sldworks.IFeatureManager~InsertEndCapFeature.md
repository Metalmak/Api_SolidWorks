<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertEndCapFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertEndCapFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertEndCapFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Depth*
:   Thickness of the end cap

*BIsGivenOffset*
:   True to provide an offset value, false to provide a thickness ratio

*BIsChamfer*
:   True if end cap feature is chamfered, false if end cap is filleted

*OffsetValue*
:   Edge offset value; valid only if BIsGivenOffset is true

*WallThicknessRatio*
:   Wall thickness ratio; valid only if BIsGivenOffset is false

*ChamferValue*
:   Chamfer distance if BIsChamfer is true, fillet radius if BIsChamfer is false

Obsolete. Superseded by [IFeatureManager::InsertEndCapFeature3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertEndCapFeature3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertEndCapFeature( _    ByVal Depth As System.Double, _    ByVal BIsGivenOffset As System.Boolean, _    ByVal BIsChamfer As System.Boolean, _    ByVal OffsetValue As System.Double, _    ByVal WallThicknessRatio As System.Double, _    ByVal ChamferValue As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Depth As System.Double Dim BIsGivenOffset As System.Boolean Dim BIsChamfer As System.Boolean Dim OffsetValue As System.Double Dim WallThicknessRatio As System.Double Dim ChamferValue As System.Double Dim value As Feature   value = instance.InsertEndCapFeature(Depth, BIsGivenOffset, BIsChamfer, OffsetValue, WallThicknessRatio, ChamferValue) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertEndCapFeature(     System.double Depth,    System.bool BIsGivenOffset,    System.bool BIsChamfer,    System.double OffsetValue,    System.double WallThicknessRatio,    System.double ChamferValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertEndCapFeature(  &   System.double Depth, &   System.bool BIsGivenOffset, &   System.bool BIsChamfer, &   System.double OffsetValue, &   System.double WallThicknessRatio, &   System.double ChamferValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Depth*
:   Thickness of the end cap

*BIsGivenOffset*
:   True to provide an offset value, false to provide a thickness ratio

*BIsChamfer*
:   True if end cap feature is chamfered, false if end cap is filleted

*OffsetValue*
:   Edge offset value; valid only if BIsGivenOffset is true

*WallThicknessRatio*
:   Wall thickness ratio; valid only if BIsGivenOffset is false

*ChamferValue*
:   Chamfer distance if BIsChamfer is true, fillet radius if BIsChamfer is false

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertEndCapFeature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)