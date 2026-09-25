<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup~SetEntityForGravityDirection2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetEntityForGravityDirection2 Method (ICWDropTestSetup) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDropTestSetup Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup.html) : SetEntityForGravityDirection2 Method (ICWDropTestSetup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Face, edge, or plane geometry reference (see **Remarks**)

Sets the face, edge, or plane reference to determine the direction of gravity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetEntityForGravityDirection2( _    ByVal DispEntity As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDropTestSetup Dim DispEntity As System.Object Dim value As System.Boolean   value = instance.SetEntityForGravityDirection2(DispEntity) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetEntityForGravityDirection2(     System.object DispEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetEntityForGravityDirection2(  &   System.Object^ DispEntity ) ``` | |

#### Parameters

*DispEntity*
:   Face, edge, or plane geometry reference (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

If the reference entity is a plane or planar face, the velocity is applied in the direction normal to the reference entity.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDropTestSetup Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup.html)

[ICWDropTestSetup Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30