<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddRestraint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddRestraint Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddRestraint Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NRestraintType*
:   Type of restraint as defined in [swsRestraintType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRestraintType_e.html)

*DispArray*
:   Array of entities to which to apply the restraint

*RefGeom*
:   Reference geometry entity for direction; valid only if NRestraintType is set to swsRestraintType\_e.swsRestraintTypeReferenceGeometry

*ErrorCode*
:   Error code as defined in [swsRestraintError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRestraintError_e.html)

Creates a restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddRestraint( _    ByVal NRestraintType As System.Integer, _    ByVal DispArray As System.Object, _    ByVal RefGeom As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWRestraint ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim NRestraintType As System.Integer Dim DispArray As System.Object Dim RefGeom As System.Object Dim ErrorCode As System.Integer Dim value As CWRestraint   value = instance.AddRestraint(NRestraintType, DispArray, RefGeom, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWRestraint AddRestraint(     System.int NRestraintType,    System.object DispArray,    System.object RefGeom,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWRestraint^ AddRestraint(  &   System.int NRestraintType, &   System.Object^ DispArray, &   System.Object^ RefGeom, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NRestraintType*
:   Type of restraint as defined in [swsRestraintType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRestraintType_e.html)

*DispArray*
:   Array of entities to which to apply the restraint

*RefGeom*
:   Reference geometry entity for direction; valid only if NRestraintType is set to swsRestraintType\_e.swsRestraintTypeReferenceGeometry

*ErrorCode*
:   Error code as defined in [swsRestraintError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRestraintError_e.html)

#### Return Value

[Restraint](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRestraint.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddRestraint.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0