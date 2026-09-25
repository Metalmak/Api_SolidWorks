<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint~SetVertex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetVertex Method (ICWTopologyDisplacementConstraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyDisplacementConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint.html) : SetVertex Method (ICWTopologyDisplacementConstraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispVertex*
:   Vertex

Obsolete. Superseded by [ICWTopologyDisplacementConstraint::SetVertices](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint~SetVertices.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetVertex( _    ByVal DispVertex As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyDisplacementConstraint Dim DispVertex As System.Object Dim value As System.Integer   value = instance.SetVertex(DispVertex) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetVertex(     System.object DispVertex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetVertex(  &   System.Object^ DispVertex ) ``` | |

#### Parameters

*DispVertex*
:   Vertex

#### Return Value

Result code as defined in [swsTopologyStudy\_DisplacementConstraintErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_DisplacementConstraintErrors_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyDisplacementConstraint::SetVertex.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWTopologyDisplacementConstraint::SetLocationPreference](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint~SetLocationPreference.html) sets [swsTopologyStudyDisplacementConstraintLocationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementConstraintLocationOption_e.html).swsTopologyDisplacementConstraintLocationOption\_UserDefine.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyDisplacementConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint.html)

[ICWTopologyDisplacementConstraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint_members.html)

[ICWTopologyDisplacementConstraint::RemoveVertex Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint~RemoveVertex.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0