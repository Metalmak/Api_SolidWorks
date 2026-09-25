<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateCoordinateSystem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateCoordinateSystem Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : CreateCoordinateSystem Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OriginPointEntity*
:   Entity (vertex, point, midpoint, or the default point of origin on a part or assembly) for the coordinate system origin

*XAxisEntities*
:   Array of entities (vertex, point, or midpoint; linear edge or sketch line; non-linear edge or sketch entity; or planar face) for the x axis

*YAxisEntities*
:   Array of entities (vertex, point, or midpoint; linear edge or sketch line; non-linear edge or sketch entity; or planar face) for the y axis

*ZAxisEntities*
:   Array of entities (vertex, point, or midpoint; linear edge or sketch line; non-linear edge or sketch entity; or planar face) for the z axis

Creates a coordinate system feature using the specified entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateCoordinateSystem( _    ByVal OriginPointEntity As System.Object, _    ByVal XAxisEntities As System.Object, _    ByVal YAxisEntities As System.Object, _    ByVal ZAxisEntities As System.Object _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim OriginPointEntity As System.Object Dim XAxisEntities As System.Object Dim YAxisEntities As System.Object Dim ZAxisEntities As System.Object Dim value As Feature   value = instance.CreateCoordinateSystem(OriginPointEntity, XAxisEntities, YAxisEntities, ZAxisEntities) ``` | |

| C# |  |
| --- | --- |
| ``` Feature CreateCoordinateSystem(     System.object OriginPointEntity,    System.object XAxisEntities,    System.object YAxisEntities,    System.object ZAxisEntities ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ CreateCoordinateSystem(  &   System.Object^ OriginPointEntity, &   System.Object^ XAxisEntities, &   System.Object^ YAxisEntities, &   System.Object^ ZAxisEntities ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OriginPointEntity*
:   Entity (vertex, point, midpoint, or the default point of origin on a part or assembly) for the coordinate system origin

*XAxisEntities*
:   Array of entities (vertex, point, or midpoint; linear edge or sketch line; non-linear edge or sketch entity; or planar face) for the x axis

*YAxisEntities*
:   Array of entities (vertex, point, or midpoint; linear edge or sketch line; non-linear edge or sketch entity; or planar face) for the y axis

*ZAxisEntities*
:   Array of entities (vertex, point, or midpoint; linear edge or sketch line; non-linear edge or sketch entity; or planar face) for the z axis

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::CreateCoordinateSystem.

# ![](dotnetimages/collapse.gif)Example

[Create Coordinate System Feature (VBA)](Create_Coordinate_System_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ICoordinateSystemFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoordinateSystemFeatureData.html)

[IFeatureManager::InsertCoordinateSystem Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCoordinateSystem.html)

[IFeatureManager::CreateCoordinateSystemUsingNumericalValues Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateCoordinateSystemUsingNumericalValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0