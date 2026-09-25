<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMinimizeMaximumDisplacementGoal~SetCoordinateSystemPreference.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetCoordinateSystemPreference Method (ICWTopologyMinimizeMaximumDisplacementGoal) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyMinimizeMaximumDisplacementGoal Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMinimizeMaximumDisplacementGoal.html) : SetCoordinateSystemPreference Method (ICWTopologyMinimizeMaximumDisplacementGoal) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NCSPreference*
:   Coodinate system preference as defined in [swsTopologyStudyDisplacementCoordinateSysOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementCoordinateSysOption_e.html)

Sets the coordinate system preference for this minimize maximum displacement goal.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetCoordinateSystemPreference( _    ByVal NCSPreference As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyMinimizeMaximumDisplacementGoal Dim NCSPreference As System.Integer Dim value As System.Integer   value = instance.SetCoordinateSystemPreference(NCSPreference) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetCoordinateSystemPreference(     System.int NCSPreference ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetCoordinateSystemPreference(  &   System.int NCSPreference ) ``` | |

#### Parameters

*NCSPreference*
:   Coodinate system preference as defined in [swsTopologyStudyDisplacementCoordinateSysOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementCoordinateSysOption_e.html)

#### Return Value

Result code as defined in [swsTopologyStudy\_MinMaxDisplacementGoalErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_MinMaxDisplacementGoalErrors_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyMinimizeMaximumDisplacementGoal::SetCoordinateSystemPreference.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyMinimizeMaximumDisplacementGoal](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMinimizeMaximumDisplacementGoal.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid for all displacement components except [swsTopologyStudyDisplacementComponentType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementComponentType_e.html).swsTopologyStudyDisplacementCompType\_URES (URES: Resultant Displacement (Absolute)).

If NCSPreference is set to swsTopologyStudyDisplacementCoordinateSysOption\_e.swsTopologyDisplacementCoordinateSysOption\_UserDefine, then use [ICWTopologyMinimizeMaximumDisplacementGoal::SetCoordinateSystem](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMinimizeMaximumDisplacementGoal~SetCoordinateSystem.html) to set the coordinate system.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyMinimizeMaximumDisplacementGoal Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMinimizeMaximumDisplacementGoal.html)

[ICWTopologyMinimizeMaximumDisplacementGoal Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMinimizeMaximumDisplacementGoal_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0