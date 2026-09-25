<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CheckInterferenceBetweenTwoBodies.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CheckInterferenceBetweenTwoBodies Method (IModeler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : CheckInterferenceBetweenTwoBodies Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Body1*
:   First body in interference detection (see **Remarks**)

*Body2*
:   Second body in interference detection (see **Remarks**)

*CoincidentInterference*
:   True to treat coincidence as interference, false to not

*Body1InterferedFaceArray*
:   Array of faces in the first body that interfered with the second body

*Body2InterferedFaceArray*
:   Array of faces in the second body that interfered with the first body

*IntersectedBodyArray*
:   Array of interfering bodies

Checks for interference between the specified bodies in an assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CheckInterferenceBetweenTwoBodies( _    ByVal Body1 As System.Object, _    ByVal Body2 As System.Object, _    ByVal CoincidentInterference As System.Boolean, _    ByRef Body1InterferedFaceArray As System.Object, _    ByRef Body2InterferedFaceArray As System.Object, _    ByRef IntersectedBodyArray As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Body1 As System.Object Dim Body2 As System.Object Dim CoincidentInterference As System.Boolean Dim Body1InterferedFaceArray As System.Object Dim Body2InterferedFaceArray As System.Object Dim IntersectedBodyArray As System.Object Dim value As System.Boolean   value = instance.CheckInterferenceBetweenTwoBodies(Body1, Body2, CoincidentInterference, Body1InterferedFaceArray, Body2InterferedFaceArray, IntersectedBodyArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CheckInterferenceBetweenTwoBodies(     System.object Body1,    System.object Body2,    System.bool CoincidentInterference,    out System.object Body1InterferedFaceArray,    out System.object Body2InterferedFaceArray,    out System.object IntersectedBodyArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CheckInterferenceBetweenTwoBodies(  &   System.Object^ Body1, &   System.Object^ Body2, &   System.bool CoincidentInterference, &   [Out] System.Object^ Body1InterferedFaceArray, &   [Out] System.Object^ Body2InterferedFaceArray, &   [Out] System.Object^ IntersectedBodyArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Body1*
:   First body in interference detection (see **Remarks**)

*Body2*
:   Second body in interference detection (see **Remarks**)

*CoincidentInterference*
:   True to treat coincidence as interference, false to not

*Body1InterferedFaceArray*
:   Array of faces in the first body that interfered with the second body

*Body2InterferedFaceArray*
:   Array of faces in the second body that interfered with the first body

*IntersectedBodyArray*
:   Array of interfering bodies

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::CheckInterferenceBetweenTwoBodies.

# ![](dotnetimages/collapse.gif)Example

[Check for Interference Between Two Bodies (VBA)](Check_Interference_Between_Two_Bodies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, transform Body1 and Body2 to their proper positions in the coordinate space of the top-level assembly:

1. Select the assembly components.- Use [IComponent2::Transform2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Transform2.html) to get the transform of each component.- Call IComponent2::GetBodies2 for each component.- Use [IBody2::ApplyTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ApplyTransform.html) on each body using the transforms in step 2.- Specify Body1 and Body1 with the bodies that have been transformed to their correct positions in the assembly.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IInterferenceDetectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html)

[IModeler::CheckInterference3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CheckInterference3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0