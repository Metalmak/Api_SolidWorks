<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertReferencePoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertReferencePoint Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertReferencePoint Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NRefPointType*
:   Type of reference point as defined by swRefPointType\_e

*NRefPointAlongCurveType*
:   Distance, percentage, or evenly distributed as defined by swRefPointAlongCurveType\_e

*DDistance\_or\_Percent*
:   Distance at which to create the reference point on the selected entities or percentage of the length of the selected entities at which to create the reference point if NRefPointAlongCurveType is swRefPointAlongCurveDistance or swRefPointAlongCurvePercentage, respectively

*NumberOfRefPoints*
:   Number of reference points to create and evenly distribute on the selected entities if swRefPointAlongCurveType is swRefPointAlongCurveEvenlyDistributed

Creates the geometry for the reference points based on any of these selected entities: edges, faces, planes, vertices, or sketch geometry.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertReferencePoint( _    ByVal NRefPointType As System.Integer, _    ByVal NRefPointAlongCurveType As System.Integer, _    ByVal DDistance_or_Percent As System.Double, _    ByVal NumberOfRefPoints As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim NRefPointType As System.Integer Dim NRefPointAlongCurveType As System.Integer Dim DDistance_or_Percent As System.Double Dim NumberOfRefPoints As System.Integer Dim value As System.Object   value = instance.InsertReferencePoint(NRefPointType, NRefPointAlongCurveType, DDistance_or_Percent, NumberOfRefPoints) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertReferencePoint(     System.int NRefPointType,    System.int NRefPointAlongCurveType,    System.double DDistance_or_Percent,    System.int NumberOfRefPoints ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertReferencePoint(  &   System.int NRefPointType, &   System.int NRefPointAlongCurveType, &   System.double DDistance_or_Percent, &   System.int NumberOfRefPoints ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NRefPointType*
:   Type of reference point as defined by swRefPointType\_e

*NRefPointAlongCurveType*
:   Distance, percentage, or evenly distributed as defined by swRefPointAlongCurveType\_e

*DDistance\_or\_Percent*
:   Distance at which to create the reference point on the selected entities or percentage of the length of the selected entities at which to create the reference point if NRefPointAlongCurveType is swRefPointAlongCurveDistance or swRefPointAlongCurvePercentage, respectively

*NumberOfRefPoints*
:   Number of reference points to create and evenly distribute on the selected entities if swRefPointAlongCurveType is swRefPointAlongCurveEvenlyDistributed

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertReferencePoint.

# ![](dotnetimages/collapse.gif)Example

[Insert Reference Points (VBA)](Insert_Reference_Points_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method creates one or more reference point features and adds them to the FeatureManager design tree. If the reference point feature is not created, a NULL value is returned.

The NumberOfRefPoints argument must contain a value of 1 to successfully create one reference point feature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::IInsertReferencePoint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertReferencePoint.html)

[IRefPointFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPointFeatureData.html)

[IFeatureManager::EditReferencePoint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~EditReferencePoint.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0