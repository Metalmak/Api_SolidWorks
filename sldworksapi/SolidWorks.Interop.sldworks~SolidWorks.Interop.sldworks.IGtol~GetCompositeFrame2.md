<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetCompositeFrame2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCompositeFrame2 Method (IGtol) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html) : GetCompositeFrame2 Method (IGtol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FrameNum*
:   Index of GTol frame

Gets whether the GTol frame with the specified index is part of a composite frame.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCompositeFrame2( _    ByVal FrameNum As System.Short _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGtol Dim FrameNum As System.Short Dim value As System.Boolean   value = instance.GetCompositeFrame2(FrameNum) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetCompositeFrame2(     System.short FrameNum ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetCompositeFrame2(  &   System.short FrameNum ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FrameNum*
:   Index of GTol frame

#### Return Value

True if GTol frame is part of a composite frame, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Gtol::GetCompositeFrame2.

# ![](dotnetimages/collapse.gif)Example

[Create GTol Composite Frame (VBA)](Create_Gtol_Composite_Frame_Example_VB.htm)

[Create GTol Composite Frame (VB.NET)](Create_Gtol_Composite_Frame_Example_VBNET.htm)

[Create GTol Composite Frame (C#)](Create_Gtol_Composite_Frame_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html)

[IGtol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol_members.html)

[IGtol::SetCompositeFrame2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetCompositeFrame2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0