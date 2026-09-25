<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetMeshQuality.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMeshQuality Method (ICWSolidBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html) : SetMeshQuality Method (ICWSolidBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NMeshQuality*
:   Mesh quality as defined in [swsMeshQuality\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshQuality_e.html)

Sets the mesh quality for the solid body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetMeshQuality( _    ByVal NMeshQuality As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidBody Dim NMeshQuality As System.Integer Dim value As System.Boolean   value = instance.SetMeshQuality(NMeshQuality) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetMeshQuality(     System.int NMeshQuality ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetMeshQuality(  &   System.int NMeshQuality ) ``` | |

#### Parameters

*NMeshQuality*
:   Mesh quality as defined in [swsMeshQuality\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshQuality_e.html)

#### Return Value

0 if successful

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSolidBody::SetMeshQuality.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html)

[ICWSolidBody Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2020 SP0