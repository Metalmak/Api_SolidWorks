<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup~SetEntityForTargetOrientation2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetEntityForTargetOrientation2 Method (ICWDropTestSetup) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDropTestSetup Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup.html) : SetEntityForTargetOrientation2 Method (ICWDropTestSetup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Reference plane

Sets the orientation reference for the impact plane.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetEntityForTargetOrientation2( _    ByVal DispEntity As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDropTestSetup Dim DispEntity As System.Object Dim value As System.Boolean   value = instance.SetEntityForTargetOrientation2(DispEntity) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetEntityForTargetOrientation2(     System.object DispEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetEntityForTargetOrientation2(  &   System.Object^ DispEntity ) ``` | |

#### Parameters

*DispEntity*
:   Reference plane

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWDropTestSetup::TargetOrientationType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDropTestSetup~TargetOrientationType.html) = swsDropTargetOrientationType\_e.swsDropTargetOrientationType\_ParallelToRefPlane.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDropTestSetup Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup.html)

[ICWDropTestSetup Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestSetup_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30