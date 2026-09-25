<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertEndCapFeature2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertEndCapFeature2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertEndCapFeature2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Depth*
:   Depth of the end cap

*BIsGivenOffset*
:   True if end cap is offset, false if not

*BIsChamfer*
:   True if end cap feature is chamfered, false If not

*OffsetValue*
:   Value by which to offset the end cap

*WallThicknessRatio*
:   Wall thickness ratio

*ChamferValue*
:   Angle of the chamfer

*Faces*
:   Array of [Face2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) objects

Inserts an end cap feature using the specified end faces of a structural member.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertEndCapFeature2( _    ByVal Depth As System.Double, _    ByVal BIsGivenOffset As System.Boolean, _    ByVal BIsChamfer As System.Boolean, _    ByVal OffsetValue As System.Double, _    ByVal WallThicknessRatio As System.Double, _    ByVal ChamferValue As System.Double, _    ByVal Faces As System.Object _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Depth As System.Double Dim BIsGivenOffset As System.Boolean Dim BIsChamfer As System.Boolean Dim OffsetValue As System.Double Dim WallThicknessRatio As System.Double Dim ChamferValue As System.Double Dim Faces As System.Object Dim value As Feature   value = instance.InsertEndCapFeature2(Depth, BIsGivenOffset, BIsChamfer, OffsetValue, WallThicknessRatio, ChamferValue, Faces) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertEndCapFeature2(     System.double Depth,    System.bool BIsGivenOffset,    System.bool BIsChamfer,    System.double OffsetValue,    System.double WallThicknessRatio,    System.double ChamferValue,    System.object Faces ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertEndCapFeature2(  &   System.double Depth, &   System.bool BIsGivenOffset, &   System.bool BIsChamfer, &   System.double OffsetValue, &   System.double WallThicknessRatio, &   System.double ChamferValue, &   System.Object^ Faces ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Depth*
:   Depth of the end cap

*BIsGivenOffset*
:   True if end cap is offset, false if not

*BIsChamfer*
:   True if end cap feature is chamfered, false If not

*OffsetValue*
:   Value by which to offset the end cap

*WallThicknessRatio*
:   Wall thickness ratio

*ChamferValue*
:   Angle of the chamfer

*Faces*
:   Array of [Face2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) objects

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertEndCapFeature2.

# ![](dotnetimages/collapse.gif)Example

[Insert Weldment Features (VBA)](Insert_Weldment_Features_Example_VB.htm)

[Insert Weldment Features (VB.NET)](Insert_Weldment_Features_Example_VBNET.htm)

[Insert Weldment Features (C#)](Insert_Weldment_Features_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [IFeatureManager::InsertEndCapFeature3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertEndCapFeature3.html) if you want to pre-select the faces to end-cap in the graphics area.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IEndCapFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0