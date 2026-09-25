<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl~SetIncludeMinMemberThickness.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetIncludeMinMemberThickness Method (ICWTopologyThicknessControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyThicknessControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl.html) : SetIncludeMinMemberThickness Method (ICWTopologyThicknessControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BFlag*
:   1 to specify the minimum member thickness, 0 to not

Obsolete. Superseded by [ICWTopologyThicknessControl::SetIncludeMinMemberThickness2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl~SetIncludeMinMemberThickness2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetIncludeMinMemberThickness( _    ByVal BFlag As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyThicknessControl Dim BFlag As System.Integer   instance.SetIncludeMinMemberThickness(BFlag) ``` | |

| C# |  |
| --- | --- |
| ``` void SetIncludeMinMemberThickness(     System.int BFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetIncludeMinMemberThickness(  &   System.int BFlag ) ``` | |

#### Parameters

*BFlag*
:   1 to specify the minimum member thickness, 0 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyThicknessControl::SetIncludeMinMemberThickness.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyThicknessControl](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl.html) example.

# ![](dotnetimages/collapse.gif)Remarks

If BFlag is set to true, set [ICWTopologyThicknessControl::SetMinimumMemberThickness](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl~SetMinimumMemberThickness.html) and [ICWTopologyThicknessControl::SetMinimumMemberThicknessUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl~SetMinimumMemberThicknessUnit.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyThicknessControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl.html)

[ICWTopologyThicknessControl Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyThicknessControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0