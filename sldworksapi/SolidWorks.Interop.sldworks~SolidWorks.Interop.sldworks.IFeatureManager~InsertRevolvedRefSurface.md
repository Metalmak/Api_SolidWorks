<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertRevolvedRefSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRevolvedRefSurface Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertRevolvedRefSurface Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*
:   Angle of revolution in radians

*ReverseDir*
:   Angle is positive or negative (True or false)

*Angle2*
:   Angle of revolution in radians

*RevType*
:   Type of revolution (see **Remarks**)

Creates a revolved reference surface by revolving a profile around a centerline.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertRevolvedRefSurface( _    ByVal Angle As System.Double, _    ByVal ReverseDir As System.Boolean, _    ByVal Angle2 As System.Double, _    ByVal RevType As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Angle As System.Double Dim ReverseDir As System.Boolean Dim Angle2 As System.Double Dim RevType As System.Integer Dim value As Feature   value = instance.InsertRevolvedRefSurface(Angle, ReverseDir, Angle2, RevType) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertRevolvedRefSurface(     System.double Angle,    System.bool ReverseDir,    System.double Angle2,    System.int RevType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertRevolvedRefSurface(  &   System.double Angle, &   System.bool ReverseDir, &   System.double Angle2, &   System.int RevType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*
:   Angle of revolution in radians

*ReverseDir*
:   Angle is positive or negative (True or false)

*Angle2*
:   Angle of revolution in radians

*RevType*
:   Type of revolution (see **Remarks**)

#### Return Value

Pointer to [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertRevolvedRefSurface.

# ![](dotnetimages/collapse.gif)Remarks

Make the selections using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) before calling this method. See the SOLIDWORKS Help for information about what entities are valid for selection.

The RevType argument can be one of these values:

* 0 = One direction revolution.

  * 1 = MidPlane revolution. For this type of revolve, the angle specification specifies the full revolution. The angle to revolve is (angle/2) on either side of the sketch. The ReverseDir argument has no effect.

    * 2 = Two direction revolution. For a two direction revolve, Angle is the angle to revolve in Direction1 and Angle2 is the angle to revolve in Direction2.

This method does not support 3D sketches.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IRevolveFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevolveFeatureData2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0