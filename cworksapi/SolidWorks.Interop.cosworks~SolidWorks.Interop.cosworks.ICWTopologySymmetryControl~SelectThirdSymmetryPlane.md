<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl~SelectThirdSymmetryPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SelectThirdSymmetryPlane Method (ICWTopologySymmetryControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologySymmetryControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl.html) : SelectThirdSymmetryPlane Method (ICWTopologySymmetryControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PlaneDisp*
:   Third symmetry plane

Sets the third symmetry plane to cut the model into eight identical bodies in this topology study symmetry manufacturing control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SelectThirdSymmetryPlane( _    ByVal PlaneDisp As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologySymmetryControl Dim PlaneDisp As System.Object   instance.SelectThirdSymmetryPlane(PlaneDisp) ``` | |

| C# |  |
| --- | --- |
| ``` void SelectThirdSymmetryPlane(     System.object PlaneDisp ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SelectThirdSymmetryPlane(  &   System.Object^ PlaneDisp ) ``` | |

#### Parameters

*PlaneDisp*
:   Third symmetry plane

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologySymmetryControl::SelectThirdSymmetryPlane.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologySymmetryControl](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method is not valid if [ICWTopologySymmetryControl::SelectSymmetryType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl~SelectSymmetryType.html) is set to:

* [swsTopologySymmetryControlOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologySymmetryControlOption_e.html).swsTopologySymmetryControlType\_HalfSymmetry

    - or -

* [swsTopologySymmetryControlOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologySymmetryControlOption_e.html).swsTopologySymmetryControlType\_QuarterSymmetry

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologySymmetryControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl.html)

[ICWTopologySymmetryControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl_members.html)

[ICWTopologySymmetryControl::ClearSelPlanes Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologySymmetryControl~ClearSelPlanes.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0