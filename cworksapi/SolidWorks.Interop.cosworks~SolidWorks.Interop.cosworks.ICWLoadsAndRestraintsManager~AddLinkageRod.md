<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddLinkageRod.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddLinkageRod Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddLinkageRod Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VertexOrCircularFacesForEnd1*
:   Array of vertex or concentric circular faces (or edges for shells) for End 1

*VertexOrCircularFacesForEnd2*
:   Array of vertex or concentric circular faces (or edges for shells) for End 2

*NUnitSys*
:   Units as defined by [swsUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsUnit_e.html)

*ErrorCode*
:   Error code as defined by [swsLinkageRodEndEditErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinkageRodEndEditErrors_e.html)

Adds the specified linkage rod connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddLinkageRod( _    ByVal VertexOrCircularFacesForEnd1 As System.Object, _    ByVal VertexOrCircularFacesForEnd2 As System.Object, _    ByVal NUnitSys As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As CWLinkageRod ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim VertexOrCircularFacesForEnd1 As System.Object Dim VertexOrCircularFacesForEnd2 As System.Object Dim NUnitSys As System.Integer Dim ErrorCode As System.Integer Dim value As CWLinkageRod   value = instance.AddLinkageRod(VertexOrCircularFacesForEnd1, VertexOrCircularFacesForEnd2, NUnitSys, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWLinkageRod AddLinkageRod(     System.object VertexOrCircularFacesForEnd1,    System.object VertexOrCircularFacesForEnd2,    System.int NUnitSys,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWLinkageRod^ AddLinkageRod(  &   System.Object^ VertexOrCircularFacesForEnd1, &   System.Object^ VertexOrCircularFacesForEnd2, &   System.int NUnitSys, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VertexOrCircularFacesForEnd1*
:   Array of vertex or concentric circular faces (or edges for shells) for End 1

*VertexOrCircularFacesForEnd2*
:   Array of vertex or concentric circular faces (or edges for shells) for End 2

*NUnitSys*
:   Units as defined by [swsUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsUnit_e.html)

*ErrorCode*
:   Error code as defined by [swsLinkageRodEndEditErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinkageRodEndEditErrors_e.html)

#### Return Value

[ICWLinkageRod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddLinkageRod.

# ![](dotnetimages/collapse.gif)Example

See the [ICWLinkageRod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0