<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup~MiterMergeCondition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MiterMergeCondition Property (IStructuralMemberGroup) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html) : MiterMergeCondition Property (IStructuralMemberGroup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Get or set whether to merge miter trimmed bodies in this structural-member group.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MiterMergeCondition As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IStructuralMemberGroup Dim value As System.Boolean   instance.MiterMergeCondition = value   value = instance.MiterMergeCondition ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MiterMergeCondition {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool MiterMergeCondition {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to merge miter trimmed bodies, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See StructuralMemberGroup::MiterMergeCondition.

# ![](dotnetimages/collapse.gif)Example

[Merge Miter Trimmed Bodies (C#)](Merge_Miter_Trimmed_Bodies_Example_CSharp.htm)

[Merge Miter Trimmed Bodies (VB.NET)](Merge_Miter_Trimmed_Bodies_Example_VBNET.htm)

[Merge Miter Trimmed Bodies (VBA)](Merge_Miter_Trimmed_Bodies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is only available when [IStructuralMemberGroup::CornerTreatmentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup~CornerTreatmentType.html) is swSolidworksWeldmentEndCondOptions\_e.swEndConditionMiter.

# ![](dotnetimages/collapse.gif)See Also

####

[IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html)

[IStructuralMemberGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup_members.html)

[IStructuralMemberGroup::ApplyCornerTreatment Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup~ApplyCornerTreatment.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0