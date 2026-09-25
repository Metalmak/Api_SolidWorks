<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~SelectChain.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SelectChain Method (ISketchSegment) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html) : SelectChain Method (ISketchSegment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Append*
:   True to append to the current selection list, false to replace the selection list

*Data*
:   [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html)

Selects chains of entities attached to this sketch segment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SelectChain( _    ByVal Append As System.Boolean, _    ByVal Data As SelectData _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSegment Dim Append As System.Boolean Dim Data As SelectData Dim value As System.Boolean   value = instance.SelectChain(Append, Data) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SelectChain(     System.bool Append,    SelectData Data ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SelectChain(  &   System.bool Append, &   SelectData^ Data ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Append*
:   True to append to the current selection list, false to replace the selection list

*Data*
:   [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchSegment::SelectChain.

# ![](dotnetimages/collapse.gif)Example

[Select Chains of Entities Attached to a Sketch Segment (VBA)](Select_Chain_of_Entities_Example_VB.htm)

[Select Chains of Entities Attached to a Sketch Segment (VB.NET)](Select_Chain_of_Entities_Example_VBNET.htm)

[Select Chains of Entities Attached to a Sketch Segment (C#)](Select_Chain_of_Entities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method call [ISelectionMgr::CreateSelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~CreateSelectData.html) to specify Data.

This method is equivalent to right-clicking a sketch segment and selecting **Select Chain**. The chain of entities in each direction is selected. Selection ends when a branch in the chain is encountered.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[ISketchSegment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0