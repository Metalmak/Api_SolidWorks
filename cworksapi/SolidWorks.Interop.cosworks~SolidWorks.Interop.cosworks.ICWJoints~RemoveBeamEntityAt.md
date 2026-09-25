<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~RemoveBeamEntityAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RemoveBeamEntityAt Method (ICWJoints) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWJoints Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints.html) : RemoveBeamEntityAt Method (ICWJoints) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based index of the beam to remove

Removes the specified beam from the joints.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub RemoveBeamEntityAt( _    ByVal NIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWJoints Dim NIndex As System.Integer   instance.RemoveBeamEntityAt(NIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveBeamEntityAt(     System.int NIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveBeamEntityAt(  &   System.int NIndex ) ``` | |

#### Parameters

*NIndex*
:   0-based index of the beam to remove

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWJoints::RemoveBeamEntityAt.

# ![](dotnetimages/collapse.gif)Remarks

To determine a valid index for the beam to remove, call [IBeamManager::BeamCount](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBeamManager~BeamCount.html).

To remove a beam:

1. [Begin editing](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWJoints~JointsBeginEdit.html).- Remove a beam by calling this method.- [Save your modification.](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWJoints~IncludeKeepModifiedJointOnUpdate.html)- [Calculate](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWJoints~CalculateJoints.html) the joints.- [End editing](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWJoints~JointsEndEdit.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWJoints Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints.html)

[ICWJoints Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints_members.html)

[ICWJoints::InsertBeamEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~InsertBeamEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010 SP0