<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddBearingLoad.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddBearingLoad Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddBearingLoad Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CoordinateSystem*
:   Coordinate system (see **Remarks**)

*FirstFace*
:   Array of cylindrical faces or circular shell edges (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsLoadsAndRestraintsManagerBearingLoadError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLoadsAndRestraintsManagerBearingLoadError_e.html)

Adds a bearing load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddBearingLoad( _    ByVal CoordinateSystem As System.Object, _    ByVal FirstFace As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWBearingLoad ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim CoordinateSystem As System.Object Dim FirstFace As System.Object Dim ErrorCode As System.Integer Dim value As CWBearingLoad   value = instance.AddBearingLoad(CoordinateSystem, FirstFace, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWBearingLoad AddBearingLoad(     System.object CoordinateSystem,    System.object FirstFace,    ref System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWBearingLoad^ AddBearingLoad(  &   System.Object^ CoordinateSystem, &   System.Object^ FirstFace, &   System.int% ErrorCode ) ``` | |

#### Parameters

*CoordinateSystem*
:   Coordinate system (see **Remarks**)

*FirstFace*
:   Array of cylindrical faces or circular shell edges (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsLoadsAndRestraintsManagerBearingLoadError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLoadsAndRestraintsManagerBearingLoadError_e.html)

#### Return Value

[Bearing load](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBearingLoad.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddBearingLoad.

# ![](dotnetimages/collapse.gif)Example

[Add Bearing Load (VBA)](Add_Bearing_Load_Example_VB.htm)

[Add Bearing Load (VB.NET)](Add_Bearing_Load_Example_VBNET.htm)

[Add Bearing Load (C#)](Add_Bearing_Load_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The Z-axis of CoordinateSystem must coincide with the axes of the faces in the FirstFace array.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0