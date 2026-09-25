<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl~SetAutoDetermineCentralMidPlane2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetAutoDetermineCentralMidPlane2 Method (ICWTopologyDemoldControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyDemoldControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl.html) : SetAutoDetermineCentralMidPlane2 Method (ICWTopologyDemoldControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BFlag*
:   -1 or true to automatically determine the central mid plane, 0 or false to explicitly specify it

Sets whether to atomatically determine the central mid plane of this topology study de-mold manufacturing control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetAutoDetermineCentralMidPlane2( _    ByVal BFlag As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyDemoldControl Dim BFlag As System.Boolean   instance.SetAutoDetermineCentralMidPlane2(BFlag) ``` | |

| C# |  |
| --- | --- |
| ``` void SetAutoDetermineCentralMidPlane2(     System.bool BFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetAutoDetermineCentralMidPlane2(  &   System.bool BFlag ) ``` | |

#### Parameters

*BFlag*
:   -1 or true to automatically determine the central mid plane, 0 or false to explicitly specify it

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyDemoldControl](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWTopologyDemoldControl::SelectDemoldDirection](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl~SelectDemoldDirection.html) sets NDir to [swsTopologyDemoldDirectionOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyDemoldDirectionOption_e.html).swsTopologyDemoldDirection\_TwoDirectionMidPlane.

If BFlag is set to:

* 0, use [ICWTopologyDemoldControl::SelectPlaneForDirection](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl~SelectPlaneForDirection.html) to specify the central mid plane.* -1, use [ICWTopologyDemoldControl::SelectEdgeForPullDirection](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl~SelectEdgeForPullDirection.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyDemoldControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl.html)

[ICWTopologyDemoldControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyDemoldControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30