<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetFreeformCurveData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFreeformCurveData Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : SetFreeformCurveData Method (IFeatureManager) |

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
:   Where on the face to add the curve; valid values are between 0 and 1

*Tangent0X*
:   Tangent vector at one end of curve

*Tangent0Y*
:   Tangent vector at one end of curve

*Tangent0Z*
:   Tangent vector at one end of curve

*Tangent1X*
:   Tangent vector at other end of curve

*Tangent1Y*
:   Tangent vector at other end of curve

*Tangent1Z*
:   Tangent vector at other end of curve

Adds a curve to the pre-selected face for a Freeform feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFreeformCurveData( _    ByVal Direction As System.Short, _    ByVal CurveParameter As System.Double, _    ByVal Tangent0X As System.Double, _    ByVal Tangent0Y As System.Double, _    ByVal Tangent0Z As System.Double, _    ByVal Tangent1X As System.Double, _    ByVal Tangent1Y As System.Double, _    ByVal Tangent1Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Direction As System.Short Dim CurveParameter As System.Double Dim Tangent0X As System.Double Dim Tangent0Y As System.Double Dim Tangent0Z As System.Double Dim Tangent1X As System.Double Dim Tangent1Y As System.Double Dim Tangent1Z As System.Double   instance.SetFreeformCurveData(Direction, CurveParameter, Tangent0X, Tangent0Y, Tangent0Z, Tangent1X, Tangent1Y, Tangent1Z) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFreeformCurveData(     System.short Direction,    System.double CurveParameter,    System.double Tangent0X,    System.double Tangent0Y,    System.double Tangent0Z,    System.double Tangent1X,    System.double Tangent1Y,    System.double Tangent1Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFreeformCurveData(  &   System.short Direction, &   System.double CurveParameter, &   System.double Tangent0X, &   System.double Tangent0Y, &   System.double Tangent0Z, &   System.double Tangent1X, &   System.double Tangent1Y, &   System.double Tangent1Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   Direction of the curve; valid values are either 0 or 1

*CurveParameter*
:   Where on the face to add the curve; valid values are between 0 and 1

*Tangent0X*
:   Tangent vector at one end of curve

*Tangent0Y*
:   Tangent vector at one end of curve

*Tangent0Z*
:   Tangent vector at one end of curve

*Tangent1X*
:   Tangent vector at other end of curve

*Tangent1Y*
:   Tangent vector at other end of curve

*Tangent1Z*
:   Tangent vector at other end of curve

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::SetFreeformCurveData.

# ![](dotnetimages/collapse.gif)Remarks

The SOLIDWORKS API Freeform-related methods are intended to journal the actions performed by an interactive user while creating the feature. Because user interaction is required to create a Freeform feature, fully automating the creation of it is not possible using the SOLIDWORKS API.

The typical steps performed by an interactive user to create a Freeform feature are:

1. Select the face to form.

   - Add curves on the selected face. Corresponds to IFeatureManager::SetFreeformCurveData.

     - Add points on the curves. Corresponds to [IFeatureManager::SetFreeformPointData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~SetFreeformPointData.html).

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