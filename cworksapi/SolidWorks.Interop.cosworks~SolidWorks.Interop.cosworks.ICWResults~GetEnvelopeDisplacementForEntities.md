<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetEnvelopeDisplacementForEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetEnvelopeDisplacementForEntities Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetEnvelopeDisplacementForEntities Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BValueByNode*
:   True to get the displacement value by node, false to get the stress value by element

*NComponent*
:   Displacement component as defined in [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html)

*NEnvelopeType*
:   Envelope plot type as defined in [swsEnvelopePlotType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEnvelopePlotType_e.html)

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if NComponent is not a directional component

*ArraySelectedEntities*
:   Array of geometric entities

*NUnits*
:   Linear units as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*NShellFace*
:   Option as defined in [swsShellFace\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsShellFace_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the specified envelope displacement for the specified entities across all solution steps.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEnvelopeDisplacementForEntities( _    ByVal BValueByNode As System.Boolean, _    ByVal NComponent As System.Integer, _    ByVal NEnvelopeType As System.Integer, _    ByVal DispPlane As System.Object, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NUnits As System.Integer, _    ByVal NShellFace As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BValueByNode As System.Boolean Dim NComponent As System.Integer Dim NEnvelopeType As System.Integer Dim DispPlane As System.Object Dim ArraySelectedEntities As System.Object Dim NUnits As System.Integer Dim NShellFace As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetEnvelopeDisplacementForEntities(BValueByNode, NComponent, NEnvelopeType, DispPlane, ArraySelectedEntities, NUnits, NShellFace, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetEnvelopeDisplacementForEntities(     System.bool BValueByNode,    System.int NComponent,    System.int NEnvelopeType,    System.object DispPlane,    System.object ArraySelectedEntities,    System.int NUnits,    System.int NShellFace,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetEnvelopeDisplacementForEntities(  &   System.bool BValueByNode, &   System.int NComponent, &   System.int NEnvelopeType, &   System.Object^ DispPlane, &   System.Object^ ArraySelectedEntities, &   System.int NUnits, &   System.int NShellFace, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BValueByNode*
:   True to get the displacement value by node, false to get the stress value by element

*NComponent*
:   Displacement component as defined in [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html)

*NEnvelopeType*
:   Envelope plot type as defined in [swsEnvelopePlotType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEnvelopePlotType_e.html)

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if NComponent is not a directional component

*ArraySelectedEntities*
:   Array of geometric entities

*NUnits*
:   Linear units as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*NShellFace*
:   Option as defined in [swsShellFace\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsShellFace_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of displacement component values

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetEnvelopeDisplacementForEntities.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0