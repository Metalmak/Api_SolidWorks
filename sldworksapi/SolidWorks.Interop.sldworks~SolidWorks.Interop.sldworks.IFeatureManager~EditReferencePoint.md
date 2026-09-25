<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~EditReferencePoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditReferencePoint Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : EditReferencePoint Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NRefPointType*
:   :   Type of reference point as defined by swRefPointType\_e

*NRefPointAlongCurveType*
:   Distance, percentage, or evenly distributed as defined by swRefPointAlongCurveType\_e

*DDistance\_or\_Percent*
:   :   Distance at which to create the reference point on the selected entities or percentage of the length of the selected entities at which to create the reference point if NRefPointAlongCurveType is swRefPointAlongCurveDistance or swRefPointAlongCurvePercentage, respectively

*NumberOfRefPoints*
:   :   Number of reference points to create and evenly distribute on the selected entities if swRefPointAlongCurveType is swRefPointAlongCurveEvenlyDistributed

Edits the selected reference points.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EditReferencePoint( _    ByVal NRefPointType As System.Integer, _    ByVal NRefPointAlongCurveType As System.Integer, _    ByVal DDistance_or_Percent As System.Double, _    ByVal NumberOfRefPoints As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim NRefPointType As System.Integer Dim NRefPointAlongCurveType As System.Integer Dim DDistance_or_Percent As System.Double Dim NumberOfRefPoints As System.Integer Dim value As System.Boolean   value = instance.EditReferencePoint(NRefPointType, NRefPointAlongCurveType, DDistance_or_Percent, NumberOfRefPoints) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EditReferencePoint(     System.int NRefPointType,    System.int NRefPointAlongCurveType,    System.double DDistance_or_Percent,    System.int NumberOfRefPoints ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool EditReferencePoint(  &   System.int NRefPointType, &   System.int NRefPointAlongCurveType, &   System.double DDistance_or_Percent, &   System.int NumberOfRefPoints ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NRefPointType*
:   :   Type of reference point as defined by swRefPointType\_e

*NRefPointAlongCurveType*
:   Distance, percentage, or evenly distributed as defined by swRefPointAlongCurveType\_e

*DDistance\_or\_Percent*
:   :   Distance at which to create the reference point on the selected entities or percentage of the length of the selected entities at which to create the reference point if NRefPointAlongCurveType is swRefPointAlongCurveDistance or swRefPointAlongCurvePercentage, respectively

*NumberOfRefPoints*
:   :   Number of reference points to create and evenly distribute on the selected entities if swRefPointAlongCurveType is swRefPointAlongCurveEvenlyDistributed

#### Return Value

True if the operation succeeds, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::EditReferencePoint.

# ![](dotnetimages/collapse.gif)Remarks

A reference point is a feature. To programatically create a reference point feature, you can use [IFeatureManager::InsertReferencePoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertReferencePoint.html) or [IFeatureManager::IInsertReferencePoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~IInsertReferencePoint.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IRefPointFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPointFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0