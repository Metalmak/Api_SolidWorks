<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup~CornerTreatmentType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CornerTreatmentType Property (IStructuralMemberGroup) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html) : CornerTreatmentType Property (IStructuralMemberGroup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the type of corner treatment for this structural-member group.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CornerTreatmentType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IStructuralMemberGroup Dim value As System.Integer   instance.CornerTreatmentType = value   value = instance.CornerTreatmentType ``` | |

| C# |  |
| --- | --- |
| ``` System.int CornerTreatmentType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int CornerTreatmentType {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Type of corner treatment as defined in swSolidworksWeldmentEndCondOptions\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See StructuralMemberGroup::CornerTreatmentType.

# ![](dotnetimages/collapse.gif)Example

[Insert Structural Weldment (C#)](Insert_Structural_Weldment_Example_CSharp.htm)

[Insert Structural Weldment (VB.NET)](Insert_Structural_Weldment_Example_VBNET.htm)

[Insert Structural Weldment (VBA)](Insert_Structural_Weldment_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is only available when [IStructuralMemberGroup::ApplyCornerTreatment](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup~ApplyCornerTreatment.html) is true.

# ![](dotnetimages/collapse.gif)See Also

####

[IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html)

[IStructuralMemberGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup_members.html)

[IStructuralMemberGroup::MiterMergeCondition Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup~MiterMergeCondition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0