<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddCyclicSymmetryRestraint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddCyclicSymmetryRestraint Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddCyclicSymmetryRestraint Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstFace*
:   First face (see **Remarks**)

*SecondFace*
:   Second face (see **Remarks**)

*Axis*
:   Axis of revolution (see **Remarks**)

*ErrorCode*
:   Error code as defined in [swsCyclicRestraintError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCyclicRestraintError_e.html)

Adds a cyclic symmetry restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCyclicSymmetryRestraint( _    ByVal FirstFace As System.Object, _    ByVal SecondFace As System.Object, _    ByVal Axis As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWRestraint ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim FirstFace As System.Object Dim SecondFace As System.Object Dim Axis As System.Object Dim ErrorCode As System.Integer Dim value As CWRestraint   value = instance.AddCyclicSymmetryRestraint(FirstFace, SecondFace, Axis, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWRestraint AddCyclicSymmetryRestraint(     System.object FirstFace,    System.object SecondFace,    System.object Axis,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWRestraint^ AddCyclicSymmetryRestraint(  &   System.Object^ FirstFace, &   System.Object^ SecondFace, &   System.Object^ Axis, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*FirstFace*
:   First face (see **Remarks**)

*SecondFace*
:   Second face (see **Remarks**)

*Axis*
:   Axis of revolution (see **Remarks**)

*ErrorCode*
:   Error code as defined in [swsCyclicRestraintError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCyclicRestraintError_e.html)

#### Return Value

[ICWRestraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddCyclicSymmetryRestraint.

# ![](dotnetimages/collapse.gif)Example

[Add Cyclic Symmetry Restraint (VBA)](Add_Cyclic_Symmetry_Restraint_Example_VB.htm)

[Add Cyclic Symmetry Restraint (VB.NET)](Add_Cyclic_Symmetry_Restraint_Example_VBNET.htm)

[Add Cyclic Symmetry Restraint (C#)](Add_Cyclic_Symmetry_Restraint_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The cyclic symmetry fixture is appropriate for turbines, fans, flywheels, and motor rotors. FirstFace and SecondFace are the faces of a cut section of a model that can be repeated in a cyclical pattern about Axis. The angle between FirstFace and SecondFace should be evenly divisible by 360. You cannot apply a cyclic symmetry restraint to an invalid section. See the **Creating Valid Sections for Cyclic Symmetry** topic in the SOLIDWORKS Simulation Helps for more information.

This method is valid only for static and nonlinear studies.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0