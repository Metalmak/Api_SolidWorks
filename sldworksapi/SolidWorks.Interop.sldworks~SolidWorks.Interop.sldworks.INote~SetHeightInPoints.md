<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~SetHeightInPoints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetHeightInPoints Method (INote) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html) : SetHeightInPoints Method (INote) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*HeightIn*
:   Height for this note in points

Sets the height of this note in points (for example, 8, 10, 12, and so on).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetHeightInPoints( _    ByVal HeightIn As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As INote Dim HeightIn As System.Integer   instance.SetHeightInPoints(HeightIn) ``` | |

| C# |  |
| --- | --- |
| ``` void SetHeightInPoints(     System.int HeightIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetHeightInPoints(  &   System.int HeightIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*HeightIn*
:   Height for this note in points

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Note::SetHeightInPoints.

# ![](dotnetimages/collapse.gif)See Also

####

[INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)

[INote Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote_members.html)

[INote::GetHeight Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetHeight.html)

[INote::GetHeightAtIndex Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetHeightAtIndex.html)

[INote::GetHeightInPoints Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetHeightInPoints.html)

[INote::SetHeight Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~SetHeight.html)