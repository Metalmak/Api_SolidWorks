<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup~MergeArcSegmentBodies.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MergeArcSegmentBodies Property (IStructuralMemberGroup) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html) : MergeArcSegmentBodies Property (IStructuralMemberGroup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to merge arc segment bodies with adjacent bodies in this structural-member group.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MergeArcSegmentBodies As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IStructuralMemberGroup Dim value As System.Boolean   instance.MergeArcSegmentBodies = value   value = instance.MergeArcSegmentBodies ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MergeArcSegmentBodies {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool MergeArcSegmentBodies {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to merge arc segment bodies with adjacent bodies, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See StructuralMemberGroup::MergeArcSegmentBodies.

# ![](dotnetimages/collapse.gif)Example

[Merge Arc Segment Bodies With Adjacent Bodies (C#)](Merge_Arc_Segment_Bodies_With_Adjacent_Bodies_Example_CSharp.htm)

[Merge Arc Segment Bodies With Adjacent Bodies (VB.NET)](Merge_Arc_Segment_Bodies_With_Adjacent_Bodies_Example_VBNET.htm)

[Merge Arc Segment Bodies With Adjacent Bodies (VBA)](Merge_Arc_Segment_Bodies_With_Adjacent_Bodies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is valid for curved entities only. The arc segment and adjacent bodies must be tangent to merge.

# ![](dotnetimages/collapse.gif)See Also

####

[IStructuralMemberGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup.html)

[IStructuralMemberGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberGroup_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0