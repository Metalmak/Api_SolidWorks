<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsRemoteLoadType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsRemoteLoadType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Remote restraint or load types

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsRemoteLoadType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsRemoteLoadType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsRemoteLoadType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsRemoteLoadType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsRemoteLoadType\_DirectDisplacement** | 3 = Connects with rigid bars the remote location, at which translations and rotations are applied, to the center of the selected faces; Available for nonlinear studies only |
| **swsRemoteLoadType\_DirectLoad** | 0 = Transfers the specified remote forces and moments to the selected faces |
| **swsRemoteLoadType\_RigidDisplacement** | 2 = Connects with rigid bars the remote location, at which translations and rotations are applied, to the selected faces, edges, or vertices |
| **swsRemoteLoadType\_RigidLoadOrMass** | 1 = Connects with rigid bars the remote location, at which forces, moments, and/or masses are applied, to the selected faces, edges, or vertices |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)