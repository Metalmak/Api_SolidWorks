<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl~SelectSymmetryType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SelectSymmetryType Method (ICWTopologySymmetryControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologySymmetryControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl.html) : SelectSymmetryType Method (ICWTopologySymmetryControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NType*
:   Type of symmetry as defined in [swsTopologySymmetryControlOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologySymmetryControlOption_e.html)

Sets the type of symmetry in this topology study symmetry manufacturing control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SelectSymmetryType( _    ByVal NType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologySymmetryControl Dim NType As System.Integer   instance.SelectSymmetryType(NType) ``` | |

| C# |  |
| --- | --- |
| ``` void SelectSymmetryType(     System.int NType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SelectSymmetryType(  &   System.int NType ) ``` | |

#### Parameters

*NType*
:   Type of symmetry as defined in [swsTopologySymmetryControlOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologySymmetryControlOption_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologySymmetryControl::SelectSymmetryType.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologySymmetryControl](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl.html) example.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologySymmetryControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl.html)

[ICWTopologySymmetryControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0