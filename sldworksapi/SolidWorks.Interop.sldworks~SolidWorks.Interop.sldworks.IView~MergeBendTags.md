<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~MergeBendTags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MergeBendTags Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : MergeBendTags Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Merge*
:   True to merge bend tags, false to unmerge a merged bend tag

*BendNotes*
:   Array of two or more bend [tags](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html) to merge or an array of one merged bend tag to unmerge

Merges or unmerges bend tags in drawings of sheet metal parts.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MergeBendTags( _    ByVal Merge As System.Boolean, _    ByVal BendNotes As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Merge As System.Boolean Dim BendNotes As System.Object Dim value As System.Boolean   value = instance.MergeBendTags(Merge, BendNotes) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MergeBendTags(     System.bool Merge,    System.object BendNotes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool MergeBendTags(  &   System.bool Merge, &   System.Object^ BendNotes ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Merge*
:   True to merge bend tags, false to unmerge a merged bend tag

*BendNotes*
:   Array of two or more bend [tags](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html) to merge or an array of one merged bend tag to unmerge

#### Return Value

True if the bend tags are merged or a merged bend tag is unmerged, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::MergeBendTags.

# ![](dotnetimages/collapse.gif)Example

[Merge and Unmerge Bend Tags (C#)](Merge_and_Unmerge_Bend_Tags_Example_CSharp.htm)

[Merge and Unmerge Bend Tags (VB.NET)](Merge_and_Unmerge_Bend_Tags_Example_VBNET.htm)

[Merge and Unmerge Bend Tags (VBA)](Merge_and_Unmerge_Bend_Tags_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **To...** | **Do...** |
| Merge two or more bend tags | 1. Select the bend tags to merge.- Select the drawing view in which the bend tags exist.- Call this method with the Merge parameter set to true.- Rebuild the drawing. |
| Unmerge a merged bend tag | 1. Select the drawing view in which the merged bend tag exists.- Activate the drawing view in which the merged bend tag exists.- Select the merged bend tag to unmerge.- Call this method with the Merge parameter set to false. |

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[INote::IsBendLineNote Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~IsBendLineNote.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0