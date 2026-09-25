<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertConnectionPoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertConnectionPoint Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertConnectionPoint Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Route type as defined in swConnectionPointType\_e

*SubType*
:   Electrical route sub-type as defined in swElectricalConnectionPointType\_e

*ReverseDirection*
:   True to flip the direction in which the route exits the fitting, false to not

*Diameter*
:   Nominal diameter (for pipe, tube, and electrical conduit fittings only)

*StubLength*
:   Default stub length to extend from the connector or fitting when inserted into routes

    **NOTE**: For ribbon cables, leave stub length at 0 or set it to a value greater than half the width of the cable to assure that folds made near the connector can be created properly.

*MinimumStraight*
:   Minimum straight length (for tubes only)

*EndLengthAdjustment*
:   End length adjustment (for tubes only)

*ConductorSplitLength*
:   Conductor split length (for electrical only)

*SchematicPinID*
:   2D schematic pin ID (for ribbon cables only)

*CableWidth*
:   Width (for ribbon cables only)

*CableThickness*
:   Cable thickness (for ribbon cables only)

*SwitchPin1Position*
:   Switch Pin1 position (for ribbon cables only)

*SpecificationFieldName*
:   Specification field name (for pipes and tubes only)

*SpecificationValue*
:   Specification value (for pipes and tubes only)

Adds a connection point based on the selected entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertConnectionPoint( _    ByVal Type As System.Integer, _    ByVal SubType As System.Integer, _    ByVal ReverseDirection As System.Boolean, _    ByVal Diameter As System.Double, _    ByVal StubLength As System.Double, _    ByVal MinimumStraight As System.Double, _    ByVal EndLengthAdjustment As System.Double, _    ByVal ConductorSplitLength As System.Double, _    ByVal SchematicPinID As System.String, _    ByVal CableWidth As System.Double, _    ByVal CableThickness As System.Double, _    ByVal SwitchPin1Position As System.Boolean, _    ByVal SpecificationFieldName As System.String, _    ByVal SpecificationValue As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Type As System.Integer Dim SubType As System.Integer Dim ReverseDirection As System.Boolean Dim Diameter As System.Double Dim StubLength As System.Double Dim MinimumStraight As System.Double Dim EndLengthAdjustment As System.Double Dim ConductorSplitLength As System.Double Dim SchematicPinID As System.String Dim CableWidth As System.Double Dim CableThickness As System.Double Dim SwitchPin1Position As System.Boolean Dim SpecificationFieldName As System.String Dim SpecificationValue As System.String Dim value As System.Boolean   value = instance.InsertConnectionPoint(Type, SubType, ReverseDirection, Diameter, StubLength, MinimumStraight, EndLengthAdjustment, ConductorSplitLength, SchematicPinID, CableWidth, CableThickness, SwitchPin1Position, SpecificationFieldName, SpecificationValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertConnectionPoint(     System.int Type,    System.int SubType,    System.bool ReverseDirection,    System.double Diameter,    System.double StubLength,    System.double MinimumStraight,    System.double EndLengthAdjustment,    System.double ConductorSplitLength,    System.string SchematicPinID,    System.double CableWidth,    System.double CableThickness,    System.bool SwitchPin1Position,    System.string SpecificationFieldName,    System.string SpecificationValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertConnectionPoint(  &   System.int Type, &   System.int SubType, &   System.bool ReverseDirection, &   System.double Diameter, &   System.double StubLength, &   System.double MinimumStraight, &   System.double EndLengthAdjustment, &   System.double ConductorSplitLength, &   System.String^ SchematicPinID, &   System.double CableWidth, &   System.double CableThickness, &   System.bool SwitchPin1Position, &   System.String^ SpecificationFieldName, &   System.String^ SpecificationValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Route type as defined in swConnectionPointType\_e

*SubType*
:   Electrical route sub-type as defined in swElectricalConnectionPointType\_e

*ReverseDirection*
:   True to flip the direction in which the route exits the fitting, false to not

*Diameter*
:   Nominal diameter (for pipe, tube, and electrical conduit fittings only)

*StubLength*
:   Default stub length to extend from the connector or fitting when inserted into routes

    **NOTE**: For ribbon cables, leave stub length at 0 or set it to a value greater than half the width of the cable to assure that folds made near the connector can be created properly.

*MinimumStraight*
:   Minimum straight length (for tubes only)

*EndLengthAdjustment*
:   End length adjustment (for tubes only)

*ConductorSplitLength*
:   Conductor split length (for electrical only)

*SchematicPinID*
:   2D schematic pin ID (for ribbon cables only)

*CableWidth*
:   Width (for ribbon cables only)

*CableThickness*
:   Cable thickness (for ribbon cables only)

*SwitchPin1Position*
:   Switch Pin1 position (for ribbon cables only)

*SpecificationFieldName*
:   Specification field name (for pipes and tubes only)

*SpecificationValue*
:   Specification value (for pipes and tubes only)

#### Return Value

True if the connection is inserted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertConnectionPoint.

# ![](dotnetimages/collapse.gif)Example

[Insert Connection Point (C#)](Insert_Connection_Point_Example_CSharp.htm)

[Insert Connection Point (VB.NET)](Insert_Connection_Point_Example_VBNET.htm)

[Insert Connection Point (VBA)](Insert_Connection_Point_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only works when the SOLIDWORKS Routing add-in is loaded (click **Tools > Add-Ins**  and select **SOLIDWORKS Routing**). This method currently supports part documents only.

Use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with:

* Mark = 1, which can be any one of the following entities to indicate the origin of a route:
  + Circular edge+ Circular face+ Face or plane plus a sketch point or vertex (select the plane or face where the routing segment exits the fitting, then select the sketch point that defines the end of the adjoining route segment)* Mark = 2, which can be a reference axis or edge to indicate which entity to align the width of the cable (for ribbon cables only)

See the SOLIDWORKS Help for details about connection points and routing.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IAssemblyDoc::GetRouteManager Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~GetRouteManager.html)

[IModelDoc2::InsertRoutePoint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertRoutePoint.html)

[IConnectionPointFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConnectionPointFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP03, Revision Number 17.03