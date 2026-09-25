<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldCoreCavitySolids.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMoldCoreCavitySolids Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMoldCoreCavitySolids Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Dist1*
:   Length of the extrusion in Direction 1

*Dist2*
:   Length of the extrusion in Direction 2

*Setback*
:   True to enable setback surface, false to not

*Angle*
:   Draft angle for the setback surface

Creates a core/cavity solid feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMoldCoreCavitySolids( _    ByVal Dist1 As System.Double, _    ByVal Dist2 As System.Double, _    ByVal Setback As System.Boolean, _    ByVal Angle As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Dist1 As System.Double Dim Dist2 As System.Double Dim Setback As System.Boolean Dim Angle As System.Double Dim value As Feature   value = instance.InsertMoldCoreCavitySolids(Dist1, Dist2, Setback, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMoldCoreCavitySolids(     System.double Dist1,    System.double Dist2,    System.bool Setback,    System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMoldCoreCavitySolids(  &   System.double Dist1, &   System.double Dist2, &   System.bool Setback, &   System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Dist1*
:   Length of the extrusion in Direction 1

*Dist2*
:   Length of the extrusion in Direction 2

*Setback*
:   True to enable setback surface, false to not

*Angle*
:   Draft angle for the setback surface

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMoldCoreCavitySolids.

# ![](dotnetimages/collapse.gif)Remarks

To use this method:

* The Parting Line feature must exist.

  * The parting surface must be generated.

    * The part must be separated into core and cavity (sheet bodies).

      * A sketch describing the outline of the mold block must exist. The sketch must be perpendicular to the pull direction. Usually, the sketch is a rectangle that includes the part (core and cavity).

The location of the sketch plane specifies the parting plane in the setback surface option.

* Without the setback surface option, the parting surface must extend beyond the block sketch so that the parting surface is cut off by the block.

  * With the setback surface option, the parting surface should be included within the block sketch. The parting plane (sketch plane) cannot intersect with the parting surface. Therefore, the parting plane must be either higher or lower than the parting surface. From the parting surface, a set of ruled surfaces is generated to be trimmed by the parting plane.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::InsertMoldPartingLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldPartingLine.html)

[IFeatureManager::InsertMoldPartingSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldPartingSurface.html)

[IFeatureManager::InsertMoldShutOffSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldShutOffSurface.html)

[ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html)

[ICavityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0