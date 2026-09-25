<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swTwistControlType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swTwistControlType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swTwistControlType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sweep twist control options.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swTwistControlType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swTwistControlType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swTwistControlType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swTwistControlType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swTwistControlConstantTwistAlongPath** | 8 = Defines the twist of the profile along the sweep path; corresponds to **Profile Twist > Specify Twist Value** in the Sweep PropertyManager |
| **swTwistControlFollowFirstSecondGuideCurves** | 3 = The twist of the intermediate sections is determined by the vector from the first guide cruve to the second guide curve; the angle between the horizontal plane and the vector remains constant in the sketch planes of all of the intermediate sections; corresponds to **Profile Twist > Follow First and Second Guide Curves** in the Sweep PropertyManager (only valid if two guide curves are present) |
| **swTwistControlFollowPath** | 0 = Corresponds to **Profile orientation > Follow Path** in the Sweep PropertyManager; after specifying this option, use ISweepFeatureData::PathAlignmentType to specify path alignment options as defined in [swTangencyType\_e](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swTangencyType_e.html) |
| **swTwistControlFollowPathFirstGuideCurve** | 2 = The twist of the intermediate sections is determined by the vector from the path to the first guide curve; the angle between the horizontal plane and the vector remains constant in the sketch planes of all of the intermediate sections; corresponds to **Profile Twist > Follow Path and First Guide Curve** in the Sweep PropertyManager (only valid if at least one guide curve is present) |
| **swTwistControlKeepNormalConstant** | 1 = Twists the section along the sweep path, keeping the section parallel to the beginning section as it twists along the path; corresponds to **Profile orientation > Keep Normal Constant** in the Sweep PropertyManager |
| **swTwistControlNormalConstantTwistAlongPath** | 9 = Defines the twist of the profile along the sweep path, keeping the section parallel to the beginning section as it twists along the path; corresponds to **Profile orientation > Keep Normal Constant** and **Profile Twist > Specify Twist Value** in the Sweep PropertyManager |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)