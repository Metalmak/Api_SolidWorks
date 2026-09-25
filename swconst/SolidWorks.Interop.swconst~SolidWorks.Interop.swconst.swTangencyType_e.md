<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swTangencyType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swTangencyType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swTangencyType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Tangency options for lofts and profile twist options for sweeps.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swTangencyType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swTangencyType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swTangencyType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swTangencyType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swMinimumTwist** | 10 = Prevents the profile from becoming self-intersecting as it follows the sweep or loft path; valid only for 3D paths; corresponds to **Profile Twist > Minimum Twist** in the Sweep PropertyManager |
| **swTangencyAllFaces** | 3 = Makes the adjacent faces tangent at the profile; valid only if swTwistControlType\_e is set to swTwistControlFollowPath and only when attaching a sweep or loft to existing geometry; corresponds to **Profile Twist > Tangent to Adjacent Faces** in the Sweep PropertyManager |
| **swTangencyDirectionVector** | 2 = Sets a direction plane, planar face, line, edge, cylinder, axis, or a pair of vertices; valid only if swTwistControlType\_e is set to swTwistControlFollowPath; corresponds to **Profile Twist > Specify Direction Vector** in the Sweep PropertyManager |
| **swTangencyNone** | 0 |
| **swTangencyNormalToProfile** | 1 = Aligns the profile normal to the sweep or loft path; valid only for 2D paths; corresponds to **Profile Twist > None** in the Sweep PropertyManager |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)