<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData~GetSketchSegments.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSketchSegments Method (IStructuralMemberFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IStructuralMemberFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html) : GetSketchSegments Method (IStructuralMemberFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PBodyIn*
:   [IBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) whose path sketch segments to get

Gets the sketch segments that define the path of the specified structural member body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSketchSegments( _    ByVal PBodyIn As Body2 _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IStructuralMemberFeatureData Dim PBodyIn As Body2 Dim value As System.Object   value = instance.GetSketchSegments(PBodyIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSketchSegments(     Body2 PBodyIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSketchSegments(  &   Body2^ PBodyIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PBodyIn*
:   [IBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) whose path sketch segments to get

#### Return Value

Array of [ISketchSegment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html)s

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See StructuralMemberFeatureData::GetSketchSegments.

# ![](dotnetimages/collapse.gif)Example

[Get Structural Member Body Sketch Segments (VBA)](Get_Structural_Member_Body_Sketch_Segments_Example_VB.htm)

[Get Structural Member Body Sketch Segments (VB.NET)](Get_Structural_Member_Body_Sketch_Segments_Example_VBNET.htm)

[Get Structural Member Body Sketch Segments (C#)](Get_Structural_Member_Body_Sketch_Segments_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IStructuralMemberFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html)

[IStructuralMemberFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0