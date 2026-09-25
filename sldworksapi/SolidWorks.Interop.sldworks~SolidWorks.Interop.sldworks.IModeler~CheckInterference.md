<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CheckInterference.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CheckInterference Method (IModeler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : CheckInterference Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Body1*
:   First [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to check for interference

*Body2*
:   Second [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to check for interference

*CoincidentInterference*
:   True to check for coincident interference, false to not

*Body1InterferedFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that have interfered from the first body with the second body

*Body2InterferedFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that have interfered from the second body with the first body

*IntersectedBodyArray*
:   Array of the interfering [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

Obsolete. Superseded by [IModeler::CheckInterference3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~CheckInterference3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CheckInterference( _    ByVal Body1 As System.Object, _    ByVal Body2 As System.Object, _    ByVal CoincidentInterference As System.Boolean, _    ByRef Body1InterferedFaceArray As System.Object, _    ByRef Body2InterferedFaceArray As System.Object, _    ByRef IntersectedBodyArray As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Body1 As System.Object Dim Body2 As System.Object Dim CoincidentInterference As System.Boolean Dim Body1InterferedFaceArray As System.Object Dim Body2InterferedFaceArray As System.Object Dim IntersectedBodyArray As System.Object Dim value As System.Boolean   value = instance.CheckInterference(Body1, Body2, CoincidentInterference, Body1InterferedFaceArray, Body2InterferedFaceArray, IntersectedBodyArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CheckInterference(     System.object Body1,    System.object Body2,    System.bool CoincidentInterference,    out System.object Body1InterferedFaceArray,    out System.object Body2InterferedFaceArray,    out System.object IntersectedBodyArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CheckInterference(  &   System.Object^ Body1, &   System.Object^ Body2, &   System.bool CoincidentInterference, &   [Out] System.Object^ Body1InterferedFaceArray, &   [Out] System.Object^ Body2InterferedFaceArray, &   [Out] System.Object^ IntersectedBodyArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Body1*
:   First [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to check for interference

*Body2*
:   Second [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to check for interference

*CoincidentInterference*
:   True to check for coincident interference, false to not

*Body1InterferedFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that have interfered from the first body with the second body

*Body2InterferedFaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that have interfered from the second body with the first body

*IntersectedBodyArray*
:   Array of the interfering [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::CheckInterference.

# ![](dotnetimages/collapse.gif)Example

[Check Interference Using IModeler::CheckInterference (VBA)](Check_Interference_using_Modeler_CheckInterference_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Each body must be transformed in the coordinate space of the top-level assembly so that it is positioned the same with respect to the other bodies as it is in assembly space.

To align the two bodies, apply the transformation from [IComponent2::Transform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Transform2.html) using [IBody2::ApplyTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ApplyTransform.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::ICheckInterferenceCount2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICheckInterferenceCount2.html)

[IAssemblyDoc::IToolsCheckInterference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IToolsCheckInterference3.html)

[IAssemblyDoc::ToolsCheckInterference2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ToolsCheckInterference2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0