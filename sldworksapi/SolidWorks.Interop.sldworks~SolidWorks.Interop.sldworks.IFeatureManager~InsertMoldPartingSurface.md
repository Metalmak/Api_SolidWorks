<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldPartingSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMoldPartingSurface Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMoldPartingSurface Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Radiate*
:   Radiate mold parting surface as defined by swPartingSurfaceMoldParmType\_e

*ReverseAlignment*
:   True to reverse alignment, false to not; only available when radiate set to swPartingSurfaceMoldParmNormal and a parting line does not yet exist (see **Remarks**)

*ReverseOffset*
:   True to reverse offset direction, false to not

*OffsetDistance*
:   True to reverse offset direction, false to not

*Angle*
:   Angle of mold parting surface; only available when radiate set to either swPartingSurfaceMoldParmTangent or swPartingSurfaceMoldParmNormal

*Smooth*
:   Smooth mold parting surface as defined by swPartingSurfaceSmoothingType\_e

*SmoothDistance*
:   Distance to smooth mold parting surface; only available when smooth set to swPartingSurfaceSmooth

*Knit*
:   True to knit all surfaces, false to not

Inserts a mold parting surface feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMoldPartingSurface( _    ByVal Radiate As System.Integer, _    ByVal ReverseAlignment As System.Boolean, _    ByVal ReverseOffset As System.Boolean, _    ByVal OffsetDistance As System.Double, _    ByVal Angle As System.Double, _    ByVal Smooth As System.Integer, _    ByVal SmoothDistance As System.Double, _    ByVal Knit As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Radiate As System.Integer Dim ReverseAlignment As System.Boolean Dim ReverseOffset As System.Boolean Dim OffsetDistance As System.Double Dim Angle As System.Double Dim Smooth As System.Integer Dim SmoothDistance As System.Double Dim Knit As System.Boolean Dim value As Feature   value = instance.InsertMoldPartingSurface(Radiate, ReverseAlignment, ReverseOffset, OffsetDistance, Angle, Smooth, SmoothDistance, Knit) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMoldPartingSurface(     System.int Radiate,    System.bool ReverseAlignment,    System.bool ReverseOffset,    System.double OffsetDistance,    System.double Angle,    System.int Smooth,    System.double SmoothDistance,    System.bool Knit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMoldPartingSurface(  &   System.int Radiate, &   System.bool ReverseAlignment, &   System.bool ReverseOffset, &   System.double OffsetDistance, &   System.double Angle, &   System.int Smooth, &   System.double SmoothDistance, &   System.bool Knit ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Radiate*
:   Radiate mold parting surface as defined by swPartingSurfaceMoldParmType\_e

*ReverseAlignment*
:   True to reverse alignment, false to not; only available when radiate set to swPartingSurfaceMoldParmNormal and a parting line does not yet exist (see **Remarks**)

*ReverseOffset*
:   True to reverse offset direction, false to not

*OffsetDistance*
:   True to reverse offset direction, false to not

*Angle*
:   Angle of mold parting surface; only available when radiate set to either swPartingSurfaceMoldParmTangent or swPartingSurfaceMoldParmNormal

*Smooth*
:   Smooth mold parting surface as defined by swPartingSurfaceSmoothingType\_e

*SmoothDistance*
:   Distance to smooth mold parting surface; only available when smooth set to swPartingSurfaceSmooth

*Knit*
:   True to knit all surfaces, false to not

#### Return Value

Pointer to [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMoldPartingSurface.

# ![](dotnetimages/collapse.gif)Remarks

f a parting line feature does not yet exist in the model, you must first select the direction of pull and the edges for the parting line using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html). For example, a face (direction of pull) has a mark of 1 and edges (parting lines) a mark of 4.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IPartingSurfaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingSurfaceFeatureData.html)

[IFeatureManager::InsertMoldCoreCavitySolids Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldCoreCavitySolids.html)

[IFeatureManager::InsertMoldPartingLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldPartingLine.html)

[IFeatureManager::InsertMoldShutOffSurface Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoldShutOffSurface.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0