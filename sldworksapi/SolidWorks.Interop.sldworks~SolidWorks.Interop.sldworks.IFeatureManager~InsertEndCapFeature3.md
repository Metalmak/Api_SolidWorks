<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertEndCapFeature3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertEndCapFeature3 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertEndCapFeature3 Method (IFeatureManager) |

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

*BIsCornerTreatment*
:   True to chamfer or fillet the end cap corners, false to not; valid only if BIsGivenOffset is false

*DepthOffset*
:   Inset distance; valid only if BIsEndCapInward = 2

*BIsReverse*
:   True to reverse the offset or thickness ratio, false to not

*BIsEndCapInward*
:   Thickness direction as defined in swEndCapThicknessDirection\_e

Inserts an end cap feature for one or more pre-selected open ends of a structural member.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertEndCapFeature3( _    ByVal Depth As System.Double, _    ByVal BIsGivenOffset As System.Boolean, _    ByVal BIsChamfer As System.Boolean, _    ByVal OffsetValue As System.Double, _    ByVal WallThicknessRatio As System.Double, _    ByVal ChamferValue As System.Double, _    ByVal BIsCornerTreatment As System.Boolean, _    ByVal DepthOffset As System.Double, _    ByVal BIsReverse As System.Boolean, _    ByVal BIsEndCapInward As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Depth As System.Double Dim BIsGivenOffset As System.Boolean Dim BIsChamfer As System.Boolean Dim OffsetValue As System.Double Dim WallThicknessRatio As System.Double Dim ChamferValue As System.Double Dim BIsCornerTreatment As System.Boolean Dim DepthOffset As System.Double Dim BIsReverse As System.Boolean Dim BIsEndCapInward As System.Integer Dim value As Feature   value = instance.InsertEndCapFeature3(Depth, BIsGivenOffset, BIsChamfer, OffsetValue, WallThicknessRatio, ChamferValue, BIsCornerTreatment, DepthOffset, BIsReverse, BIsEndCapInward) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertEndCapFeature3(     System.double Depth,    System.bool BIsGivenOffset,    System.bool BIsChamfer,    System.double OffsetValue,    System.double WallThicknessRatio,    System.double ChamferValue,    System.bool BIsCornerTreatment,    System.double DepthOffset,    System.bool BIsReverse,    System.int BIsEndCapInward ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertEndCapFeature3(  &   System.double Depth, &   System.bool BIsGivenOffset, &   System.bool BIsChamfer, &   System.double OffsetValue, &   System.double WallThicknessRatio, &   System.double ChamferValue, &   System.bool BIsCornerTreatment, &   System.double DepthOffset, &   System.bool BIsReverse, &   System.int BIsEndCapInward ) ``` | |

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

*BIsCornerTreatment*
:   True to chamfer or fillet the end cap corners, false to not; valid only if BIsGivenOffset is false

*DepthOffset*
:   Inset distance; valid only if BIsEndCapInward = 2

*BIsReverse*
:   True to reverse the offset or thickness ratio, false to not

*BIsEndCapInward*
:   Thickness direction as defined in swEndCapThicknessDirection\_e

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertEndCapFeature3.

# ![](dotnetimages/collapse.gif)Example

[Insert Weldment End Cap (VBA)](Insert_Weldment_End_Cap_Example_VB.htm)

[Insert Weldment End Cap (VB.NET)](Insert_Weldment_End_Cap_Example_VBNET.htm)

[Insert Weldment End Cap (C#)](Insert_Weldment_End_Cap_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, select one or more end [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) of a structural member in the graphics area.

Instead of using this method, you can pass the faces in an argument array of [IFeatureManager::InsertEndCapFeature2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertEndCapFeature2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IEndCapFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0