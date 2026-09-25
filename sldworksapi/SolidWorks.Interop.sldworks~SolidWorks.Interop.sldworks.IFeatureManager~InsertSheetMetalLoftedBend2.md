<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSheetMetalLoftedBend2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalLoftedBend2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSheetMetalLoftedBend2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ThickDirType*
:   Toggles the thickening direction:

    * 0 = outside

      * 1 = inside (default value)

*Thickness*
:   Thickness of the bend

*BFormed*
:   True to insert a formed lofted bend; false to insert a bent lofted bend (default)

*DRadius*
:   Bend radius; valid only if BFormed is false

*BReferToEndPoint*
:   True to calculate facet transitions using theoretical vertexes, false to calculate facet transitions using the smallest possible arcs that avoid interference between bend areas; valid only if BFormed is false

*EFacetOption*
:   Faceting option as defined in swLoftedBendFacetOptions\_e; valid only if BFormed is false

*DChordTol*
:   Chord tolerance or maximum distance between the arc and linear segment of a chord; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swChordTolerance and BFormed is false

*INumBends*
:   Maximum number of bends per transition segment; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swBendsPerTransitionSegment and BFormed is false

*DSegLength*
:   Maximum length of the linear segment; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swSegmentLength and BFormed is false

*DSegAngle*
:   Maximum angle between adjacent linear segments; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swSegmentAngle and BFormed is false

Inserts a lofted bend in a sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSheetMetalLoftedBend2( _    ByVal ThickDirType As System.Integer, _    ByVal Thickness As System.Double, _    ByVal BFormed As System.Boolean, _    ByVal DRadius As System.Double, _    ByVal BReferToEndPoint As System.Boolean, _    ByVal EFacetOption As System.Integer, _    ByVal DChordTol As System.Double, _    ByVal INumBends As System.Integer, _    ByVal DSegLength As System.Double, _    ByVal DSegAngle As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim ThickDirType As System.Integer Dim Thickness As System.Double Dim BFormed As System.Boolean Dim DRadius As System.Double Dim BReferToEndPoint As System.Boolean Dim EFacetOption As System.Integer Dim DChordTol As System.Double Dim INumBends As System.Integer Dim DSegLength As System.Double Dim DSegAngle As System.Double Dim value As Feature   value = instance.InsertSheetMetalLoftedBend2(ThickDirType, Thickness, BFormed, DRadius, BReferToEndPoint, EFacetOption, DChordTol, INumBends, DSegLength, DSegAngle) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertSheetMetalLoftedBend2(     System.int ThickDirType,    System.double Thickness,    System.bool BFormed,    System.double DRadius,    System.bool BReferToEndPoint,    System.int EFacetOption,    System.double DChordTol,    System.int INumBends,    System.double DSegLength,    System.double DSegAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertSheetMetalLoftedBend2(  &   System.int ThickDirType, &   System.double Thickness, &   System.bool BFormed, &   System.double DRadius, &   System.bool BReferToEndPoint, &   System.int EFacetOption, &   System.double DChordTol, &   System.int INumBends, &   System.double DSegLength, &   System.double DSegAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ThickDirType*
:   Toggles the thickening direction:

    * 0 = outside

      * 1 = inside (default value)

*Thickness*
:   Thickness of the bend

*BFormed*
:   True to insert a formed lofted bend; false to insert a bent lofted bend (default)

*DRadius*
:   Bend radius; valid only if BFormed is false

*BReferToEndPoint*
:   True to calculate facet transitions using theoretical vertexes, false to calculate facet transitions using the smallest possible arcs that avoid interference between bend areas; valid only if BFormed is false

*EFacetOption*
:   Faceting option as defined in swLoftedBendFacetOptions\_e; valid only if BFormed is false

*DChordTol*
:   Chord tolerance or maximum distance between the arc and linear segment of a chord; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swChordTolerance and BFormed is false

*INumBends*
:   Maximum number of bends per transition segment; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swBendsPerTransitionSegment and BFormed is false

*DSegLength*
:   Maximum length of the linear segment; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swSegmentLength and BFormed is false

*DSegAngle*
:   Maximum angle between adjacent linear segments; valid only if EFacetOption is set to swLoftedBendFacetOptions\_e.swSegmentAngle and BFormed is false

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSheetMetalLoftedBend2.

# ![](dotnetimages/collapse.gif)Example

[Insert Lofted Bend Feature (VBA)](Insert_Lofted_Bend_Feature_Example_VB.htm)

[Insert Lofted Bend Feature (VB.NET)](Insert_Lofted_Bend_Feature_Example_VBNET.htm)

[Insert Lofted Bend Feature (C#)](Insert_Lofted_Bend_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must select at least two sketch profiles that are on parallel planes. You can either multi-select them in the graphics area or call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Mark = 1 for each sketch profile you want to select.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ILoftedBendsFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoftedBendsFeatureData.html)

[ILoftFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoftFeatureData.html)

[ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0