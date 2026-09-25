<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureCurvePattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureCurvePattern Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : FeatureCurvePattern Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Num1*
:   Number of instances in the first direction, including the original

*Spacing1*
:   Spacing in radians

*Num2*
:   Number of instances in the second direction

*Spacing2*
:   Spacing in radians

*FlipDir1*
:   True flips the direction of the first direction, false does not

*FlipDir2*
:   True flips the direction of the second direction, false does not

*EqualSpacing1*
:   True uses equal spacing between instances in the first direction, false does not

*EqualSpacing2*
:   True uses equal spacing between instances in the second direction, false does not

*UseCentroid*
:   True uses the centroid as reference point, false does not

*AlignToSeed*
:   True aligns the new objects with the seed feature, false does not

*OffsetCurve*
:   True offsets the curve, false transforms it

*PatternSeedOnly*
:   True uses only the seed feature in the second direction, false does not

Obsolete. See [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) and the Remarks of [ICurveDrivenPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurveDrivenPatternFeatureData.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub FeatureCurvePattern( _    ByVal Num1 As System.Integer, _    ByVal Spacing1 As System.Double, _    ByVal Num2 As System.Integer, _    ByVal Spacing2 As System.Double, _    ByVal FlipDir1 As System.Boolean, _    ByVal FlipDir2 As System.Boolean, _    ByVal EqualSpacing1 As System.Boolean, _    ByVal EqualSpacing2 As System.Boolean, _    ByVal UseCentroid As System.Boolean, _    ByVal AlignToSeed As System.Boolean, _    ByVal OffsetCurve As System.Boolean, _    ByVal PatternSeedOnly As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Num1 As System.Integer Dim Spacing1 As System.Double Dim Num2 As System.Integer Dim Spacing2 As System.Double Dim FlipDir1 As System.Boolean Dim FlipDir2 As System.Boolean Dim EqualSpacing1 As System.Boolean Dim EqualSpacing2 As System.Boolean Dim UseCentroid As System.Boolean Dim AlignToSeed As System.Boolean Dim OffsetCurve As System.Boolean Dim PatternSeedOnly As System.Boolean   instance.FeatureCurvePattern(Num1, Spacing1, Num2, Spacing2, FlipDir1, FlipDir2, EqualSpacing1, EqualSpacing2, UseCentroid, AlignToSeed, OffsetCurve, PatternSeedOnly) ``` | |

| C# |  |
| --- | --- |
| ``` void FeatureCurvePattern(     System.int Num1,    System.double Spacing1,    System.int Num2,    System.double Spacing2,    System.bool FlipDir1,    System.bool FlipDir2,    System.bool EqualSpacing1,    System.bool EqualSpacing2,    System.bool UseCentroid,    System.bool AlignToSeed,    System.bool OffsetCurve,    System.bool PatternSeedOnly ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void FeatureCurvePattern(  &   System.int Num1, &   System.double Spacing1, &   System.int Num2, &   System.double Spacing2, &   System.bool FlipDir1, &   System.bool FlipDir2, &   System.bool EqualSpacing1, &   System.bool EqualSpacing2, &   System.bool UseCentroid, &   System.bool AlignToSeed, &   System.bool OffsetCurve, &   System.bool PatternSeedOnly ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Num1*
:   Number of instances in the first direction, including the original

*Spacing1*
:   Spacing in radians

*Num2*
:   Number of instances in the second direction

*Spacing2*
:   Spacing in radians

*FlipDir1*
:   True flips the direction of the first direction, false does not

*FlipDir2*
:   True flips the direction of the second direction, false does not

*EqualSpacing1*
:   True uses equal spacing between instances in the first direction, false does not

*EqualSpacing2*
:   True uses equal spacing between instances in the second direction, false does not

*UseCentroid*
:   True uses the centroid as reference point, false does not

*AlignToSeed*
:   True aligns the new objects with the seed feature, false does not

*OffsetCurve*
:   True offsets the curve, false transforms it

*PatternSeedOnly*
:   True uses only the seed feature in the second direction, false does not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::FeatureCurvePattern.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0