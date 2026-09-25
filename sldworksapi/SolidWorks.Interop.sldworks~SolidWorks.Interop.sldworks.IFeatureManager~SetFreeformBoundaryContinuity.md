<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetFreeformBoundaryContinuity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFreeformBoundaryContinuity Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : SetFreeformBoundaryContinuity Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BoundaryIndex*
:   0-based index of the boundary to modify (i.e., a value ranging from 0 to (Number of face boundaries-1))

*Continuity*
:   * -1 = Movaeable* 0 = Contact* 1 = Tangenet* 2= Curvature

Sets the boundary continuity for this Freeform feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFreeformBoundaryContinuity( _    ByVal BoundaryIndex As System.Short, _    ByVal Continuity As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BoundaryIndex As System.Short Dim Continuity As System.Short   instance.SetFreeformBoundaryContinuity(BoundaryIndex, Continuity) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFreeformBoundaryContinuity(     System.short BoundaryIndex,    System.short Continuity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFreeformBoundaryContinuity(  &   System.short BoundaryIndex, &   System.short Continuity ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BoundaryIndex*
:   0-based index of the boundary to modify (i.e., a value ranging from 0 to (Number of face boundaries-1))

*Continuity*
:   * -1 = Movaeable* 0 = Contact* 1 = Tangenet* 2= Curvature

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::SetFreeformBoundaryContinuity.

# ![](dotnetimages/collapse.gif)Remarks

The SOLIDWORKS API Freeform-related methods are intended to journal the actions performed by an interactive user while creating the feature. Because user interaction is required to create a Freeform feature, fully automating the creation of it is not possible using the SOLIDWORKS API.

The typical steps performed by an interactive user to create a Freeform feature are:

1. Select the face to form.

   - Add curves on the selected face. Corresponds to [IFeatureManager::SetFreeformCurveData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~SetFreeformCurveData.html).

     - Add points on the curves. Corresponds to [IFeatureManager::SetFreeformPointData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~SetFreeformPointData.html).

       - Specify boundary continuity. Corresponds to IFeatureManager::SetFreeformBoundaryContinuity.

         Interactively pull or push the points to change the shape of the selected face.

         - Insert the Freeform feature. Corresponds to this method, [IFeatureManager::InsertFreeform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertFreeform2.html).

Record a macro while interactively creating a Freeform feature, then examine the macro to see the order in which the Freeform-related methods are recorded.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0