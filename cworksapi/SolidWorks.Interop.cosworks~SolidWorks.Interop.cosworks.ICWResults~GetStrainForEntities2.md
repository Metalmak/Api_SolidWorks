<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetStrainForEntities2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetStrainForEntities2 Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetStrainForEntities2 Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BValueByNode*
:   True to get the strain value by node, false to get the strain value by element

*NComponent*
:   Strain as defined in [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html)

*NStepNumber*
:   Solution step number (use 1 for static)

*DispPlane*
:   Reference geometry

*ArraySelectedEntities*
:   Array of geometric entities

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Obsolete. Superseded by [ICWResults::GetStrainForEntities3](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWResults~GetStrainForEntities3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetStrainForEntities2( _    ByVal BValueByNode As System.Boolean, _    ByVal NComponent As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByVal DispPlane As System.Object, _    ByVal ArraySelectedEntities As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BValueByNode As System.Boolean Dim NComponent As System.Integer Dim NStepNumber As System.Integer Dim DispPlane As System.Object Dim ArraySelectedEntities As System.Object Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetStrainForEntities2(BValueByNode, NComponent, NStepNumber, DispPlane, ArraySelectedEntities, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetStrainForEntities2(     System.bool BValueByNode,    System.int NComponent,    System.int NStepNumber,    System.object DispPlane,    System.object ArraySelectedEntities,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetStrainForEntities2(  &   System.bool BValueByNode, &   System.int NComponent, &   System.int NStepNumber, &   System.Object^ DispPlane, &   System.Object^ ArraySelectedEntities, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BValueByNode*
:   True to get the strain value by node, false to get the strain value by element

*NComponent*
:   Strain as defined in [swsStrainComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrainComponent_e.html)

*NStepNumber*
:   Solution step number (use 1 for static)

*DispPlane*
:   Reference geometry

*ArraySelectedEntities*
:   Array of geometric entities

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of strain results (each node or element followed by the strain value)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetStrainForEntities2.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetMinMaxStrain Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxStrain.html)

[ICWResults::GetStrainComponentForAllStepsAtNode Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetStrainComponentForAllStepsAtNode.html)

[ICWResults::GetStrain Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetStrain.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP5.0