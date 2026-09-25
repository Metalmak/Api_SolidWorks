<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertCenterMark3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCenterMark3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertCenterMark3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Style*
:   Style as defined in swCenterMarkStyle\_e

*Propagate*
:   True if the center mark should propagate throughout the pattern, false if not

*Slot*
:   True if this is slot-style center mark, false if not

Inserts a center mark in a drawing document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCenterMark3( _    ByVal Style As System.Integer, _    ByVal Propagate As System.Boolean, _    ByVal Slot As System.Boolean _ ) As CenterMark ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Style As System.Integer Dim Propagate As System.Boolean Dim Slot As System.Boolean Dim value As CenterMark   value = instance.InsertCenterMark3(Style, Propagate, Slot) ``` | |

| C# |  |
| --- | --- |
| ``` CenterMark InsertCenterMark3(     System.int Style,    System.bool Propagate,    System.bool Slot ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CenterMark^ InsertCenterMark3(  &   System.int Style, &   System.bool Propagate, &   System.bool Slot ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*
:   Style as defined in swCenterMarkStyle\_e

*Propagate*
:   True if the center mark should propagate throughout the pattern, false if not

*Slot*
:   True if this is slot-style center mark, false if not

#### Return Value

[Center mark](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterMark.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertCenterMark3.

# ![](dotnetimages/collapse.gif)Remarks

Call [IView::AutoInsertCenterMarks](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~AutoInsertCenterMarks.html) to automatically insert center marks in multiple drawing views.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0