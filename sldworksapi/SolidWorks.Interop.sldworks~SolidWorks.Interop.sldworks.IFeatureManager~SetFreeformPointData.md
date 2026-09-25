<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetFreeformPointData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFreeformPointData Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : SetFreeformPointData Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Direction*
:   Direction of the curve; valid values are either 0 or 1

*CurveParameter*
:   Curve where to add the point

*ParameterOnCurve*
:   Where on the curve to add the point

*XOffset*
:   Value by which to offset x (this value is typically 0, which indicates that the point
    was not modified)

*YOffset*
:   Value by which to offset y (this value is typically 0, which indicates that the point
    was not modified)

*ZOffset*
:   Value by which to offset z (this value is typically 0, which indicates that the point
    was not modified)

Adds a point to a curve for a Freeform feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFreeformPointData( _    ByVal Direction As System.Short, _    ByVal CurveParameter As System.Double, _    ByVal ParameterOnCurve As System.Double, _    ByVal XOffset As System.Double, _    ByVal YOffset As System.Double, _    ByVal ZOffset As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Direction As System.Short Dim CurveParameter As System.Double Dim ParameterOnCurve As System.Double Dim XOffset As System.Double Dim YOffset As System.Double Dim ZOffset As System.Double   instance.SetFreeformPointData(Direction, CurveParameter, ParameterOnCurve, XOffset, YOffset, ZOffset) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFreeformPointData(     System.short Direction,    System.double CurveParameter,    System.double ParameterOnCurve,    System.double XOffset,    System.double YOffset,    System.double ZOffset ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFreeformPointData(  &   System.short Direction, &   System.double CurveParameter, &   System.double ParameterOnCurve, &   System.double XOffset, &   System.double YOffset, &   System.double ZOffset ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   Direction of the curve; valid values are either 0 or 1

*CurveParameter*
:   Curve where to add the point

*ParameterOnCurve*
:   Where on the curve to add the point

*XOffset*
:   Value by which to offset x (this value is typically 0, which indicates that the point
    was not modified)

*YOffset*
:   Value by which to offset y (this value is typically 0, which indicates that the point
    was not modified)

*ZOffset*
:   Value by which to offset z (this value is typically 0, which indicates that the point
    was not modified)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::SetFreeformPointData.

# ![](dotnetimages/collapse.gif)Remarks

The SOLIDWORKS API Freeform-related methods are intended to journal the actions performed by an interactive user while creating the feature. Because user interaction is required to create a Freeform feature, fully automating the creation of it is not possible using the SOLIDWORKS API.

The typical steps performed by an interactive user to create a Freeform feature are:

1. Select the face to form.

   - Add curves on the selected face. Corresponds to [IFeatureManager::SetFreeformCurveData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~SetFreeformCurveData.html).

     - Add points on the curves. Corresponds to IFeatureManager::SetFreeformPointData.

       - Specify boundary continuity. Corresponds to [IFeatureManager::SetFreeformBoundaryContinuity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~SetFreeformBoundaryContinuity.html).

         Interactively pull or push the points to change the shape of the selected face.

         - Insert the Freeform feature. Corresponds to this method, [IFeatureManager::InsertFreeform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertFreeform2.html).

Record a macro while interactively creating a Freeform feature, then examine the macro to see the order in which the Freeform-related methods are recorded.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0