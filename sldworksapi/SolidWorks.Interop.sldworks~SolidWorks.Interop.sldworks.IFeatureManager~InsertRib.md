<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertRib.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRib Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertRib Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Is2Sided*
:   True if the rib is double-sided, false if the rib is single sided; a double-sided rib thickens on both sides of the sketch

*ReverseThicknessDir*
:   True to thicken the opposite side of the sketch normal, false to not; only valid for single-sided ribs

*Thickness*
:   Rib thickness

*ReferenceEdgeIndex*
:   Edge in the sketch to use to determine the material direction and for draft reference; when the rib is drafted, the mid point of this edge maintains the thickness value; other points on the rib may have a different thicknesses due to the draft

*ReverseMaterialDir*
:   True to flip the direction of the extrusion, false to not

*IsDrafted*
:   True to draft the rib, false to not

*DraftOutward*
:   True to draft the rib outward, false to not; only valid if IsDrafted is true

*DraftAngle*
:   Draft angle of the rib; only valid if IsDrafted is true

*IsNormToSketch*
:   True if extrusion direction is normal to sketch, false if parallel to sketch

*IsDraftedFromWall*
:   True if draft is from wall, false if not; only valid if IsDrafted is true

Inserts a rib.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertRib( _    ByVal Is2Sided As System.Boolean, _    ByVal ReverseThicknessDir As System.Boolean, _    ByVal Thickness As System.Double, _    ByVal ReferenceEdgeIndex As System.Integer, _    ByVal ReverseMaterialDir As System.Boolean, _    ByVal IsDrafted As System.Boolean, _    ByVal DraftOutward As System.Boolean, _    ByVal DraftAngle As System.Double, _    ByVal IsNormToSketch As System.Boolean, _    ByVal IsDraftedFromWall As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Is2Sided As System.Boolean Dim ReverseThicknessDir As System.Boolean Dim Thickness As System.Double Dim ReferenceEdgeIndex As System.Integer Dim ReverseMaterialDir As System.Boolean Dim IsDrafted As System.Boolean Dim DraftOutward As System.Boolean Dim DraftAngle As System.Double Dim IsNormToSketch As System.Boolean Dim IsDraftedFromWall As System.Boolean   instance.InsertRib(Is2Sided, ReverseThicknessDir, Thickness, ReferenceEdgeIndex, ReverseMaterialDir, IsDrafted, DraftOutward, DraftAngle, IsNormToSketch, IsDraftedFromWall) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertRib(     System.bool Is2Sided,    System.bool ReverseThicknessDir,    System.double Thickness,    System.int ReferenceEdgeIndex,    System.bool ReverseMaterialDir,    System.bool IsDrafted,    System.bool DraftOutward,    System.double DraftAngle,    System.bool IsNormToSketch,    System.bool IsDraftedFromWall ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertRib(  &   System.bool Is2Sided, &   System.bool ReverseThicknessDir, &   System.double Thickness, &   System.int ReferenceEdgeIndex, &   System.bool ReverseMaterialDir, &   System.bool IsDrafted, &   System.bool DraftOutward, &   System.double DraftAngle, &   System.bool IsNormToSketch, &   System.bool IsDraftedFromWall ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Is2Sided*
:   True if the rib is double-sided, false if the rib is single sided; a double-sided rib thickens on both sides of the sketch

*ReverseThicknessDir*
:   True to thicken the opposite side of the sketch normal, false to not; only valid for single-sided ribs

*Thickness*
:   Rib thickness

*ReferenceEdgeIndex*
:   Edge in the sketch to use to determine the material direction and for draft reference; when the rib is drafted, the mid point of this edge maintains the thickness value; other points on the rib may have a different thicknesses due to the draft

*ReverseMaterialDir*
:   True to flip the direction of the extrusion, false to not

*IsDrafted*
:   True to draft the rib, false to not

*DraftOutward*
:   True to draft the rib outward, false to not; only valid if IsDrafted is true

*DraftAngle*
:   Draft angle of the rib; only valid if IsDrafted is true

*IsNormToSketch*
:   True if extrusion direction is normal to sketch, false if parallel to sketch

*IsDraftedFromWall*
:   True if draft is from wall, false if not; only valid if IsDrafted is true

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertRib.

# ![](dotnetimages/collapse.gif)Example

[Get Rib Feature Data (VBA)](Get_Rib_Feature_Data_Example_VB.htm)

[Get Rib Feature Data (VB.NET)](Get_Rib_Feature_Data_Example_VBNET.htm)

[Get Rib Feature Data (C#)](Get_Rib_Feature_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IRibFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0