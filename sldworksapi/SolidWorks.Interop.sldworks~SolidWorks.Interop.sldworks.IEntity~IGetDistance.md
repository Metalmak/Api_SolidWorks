<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity~IGetDistance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetDistance Method (IEntity) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEntity Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity.html) : IGetDistance Method (IEntity) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BaseEntity*
:   [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) of another edge or face to get distance from this entity (see **Remarks**)

*MinDistance*
:   True to return minimum distance; false to return maximum distance

*Parameter*
:   For in-process, unmanaged C++:

    > If MinDistance = False,
    >
    > * and BaseEntity is an edge or curve, specify an array of two doubles (Min, Max), where Min and Max make up the U-parameter range of BaseEntity* and BaseEntity is a face, specify an array of four doubles (UMin, VMin, UMax, VMax), where UMin, VMin, UMax, and VMax make up the UV-parameter range of the surface of BaseEntity
    >
    > If MinDistance = True,
    >
    > * and BaseEntity is an edge or curve, optionally specify an array of two doubles (Min, Max), where Min and Max make up the U-parameter range of BaseEntity* and BaseEntity is a face, optionally specify an array of four doubles (UMin, VMin, UMax, VMax), where UMin, VMin, UMax, and VMax make up the UV-parameter range of the surface of BaseEntity

    For VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*Position1*
:   * For in-process, unmanaged C++: pointer to an array of doubles (coordinates of this entity that were used to measure the distance)

      * For VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*Position2*
:   * For in-process, unmanaged C++: pointer to an array of doubles (coordinates of BaseEntity that were used to measure the distance)

    - For VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*Distance*
:   Minimum or maximum distance between entities; if Parameter is not specified, the minimum distance

Gets the minimum or maximum distance between this entity and the given face or edge entity (see **Remarks**).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetDistance( _    ByVal BaseEntity As Entity, _    ByVal MinDistance As System.Boolean, _    ByRef Parameter As System.Double, _    ByRef Position1 As System.Double, _    ByRef Position2 As System.Double, _    ByRef Distance As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEntity Dim BaseEntity As Entity Dim MinDistance As System.Boolean Dim Parameter As System.Double Dim Position1 As System.Double Dim Position2 As System.Double Dim Distance As System.Double Dim value As System.Integer   value = instance.IGetDistance(BaseEntity, MinDistance, Parameter, Position1, Position2, Distance) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetDistance(     Entity BaseEntity,    System.bool MinDistance,    ref System.double Parameter,    out System.double Position1,    out System.double Position2,    out System.double Distance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetDistance(  &   Entity^ BaseEntity, &   System.bool MinDistance, &   System.double% Parameter, &   [Out] System.double Position1, &   [Out] System.double Position2, &   [Out] System.double Distance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BaseEntity*
:   [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) of another edge or face to get distance from this entity (see **Remarks**)

*MinDistance*
:   True to return minimum distance; false to return maximum distance

*Parameter*
:   For in-process, unmanaged C++:

    > If MinDistance = False,
    >
    > * and BaseEntity is an edge or curve, specify an array of two doubles (Min, Max), where Min and Max make up the U-parameter range of BaseEntity* and BaseEntity is a face, specify an array of four doubles (UMin, VMin, UMax, VMax), where UMin, VMin, UMax, and VMax make up the UV-parameter range of the surface of BaseEntity
    >
    > If MinDistance = True,
    >
    > * and BaseEntity is an edge or curve, optionally specify an array of two doubles (Min, Max), where Min and Max make up the U-parameter range of BaseEntity* and BaseEntity is a face, optionally specify an array of four doubles (UMin, VMin, UMax, VMax), where UMin, VMin, UMax, and VMax make up the UV-parameter range of the surface of BaseEntity

    For VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*Position1*
:   * For in-process, unmanaged C++: pointer to an array of doubles (coordinates of this entity that were used to measure the distance)

      * For VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*Position2*
:   * For in-process, unmanaged C++: pointer to an array of doubles (coordinates of BaseEntity that were used to measure the distance)

    - For VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*Distance*
:   Minimum or maximum distance between entities; if Parameter is not specified, the minimum distance

#### Return Value

0 if success; -1 if failure

# ![](dotnetimages/collapse.gif)Remarks

Only face and edge entities are supported.

To populate Parameter you can find the UV parameter ranges as follows:

* For edges and curves, use [IEdge::GetCurveParams2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge~GetCurveParams2.html)* For faces, use [IFace2::GetUVBounds](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~GetUVBounds.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEntity Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity.html)

[IEntity Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity_members.html)

[IEntity::GetDistance Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity~GetDistance.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP5, Revision Number 17.5