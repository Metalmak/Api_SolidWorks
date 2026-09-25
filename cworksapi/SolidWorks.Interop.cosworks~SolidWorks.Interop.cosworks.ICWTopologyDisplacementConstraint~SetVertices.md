<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint~SetVertices.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetVertices Method (ICWTopologyDisplacementConstraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyDisplacementConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint.html) : SetVertices Method (ICWTopologyDisplacementConstraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VerticesDispArray*
:   Array of vertexes

Sets the vertexes of a load-bearing face on which to apply this topology study displacement constraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetVertices( _    ByVal VerticesDispArray As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyDisplacementConstraint Dim VerticesDispArray As System.Object Dim value As System.Integer   value = instance.SetVertices(VerticesDispArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetVertices(     System.object VerticesDispArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetVertices(  &   System.Object^ VerticesDispArray ) ``` | |

#### Parameters

*VerticesDispArray*
:   Array of vertexes

#### Return Value

Result code as defined in [swsTopologyStudy\_DisplacementConstraintErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_DisplacementConstraintErrors_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyDisplacementConstraint::SetVertices.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyDisplacementConstraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWTopologyDisplacementConstraint::SetLocationPreference](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint~SetLocationPreference.html) sets [swsTopologyStudyDisplacementConstraintLocationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementConstraintLocationOption_e.html).swsTopologyDisplacementConstraintLocationOption\_UserDefine.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyDisplacementConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint.html)

[ICWTopologyDisplacementConstraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint_members.html)

 [ICWTopologyDisplacementConstraint::RemoveAllVertices Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDisplacementConstraint~RemoveAllVertices.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2020 SP0