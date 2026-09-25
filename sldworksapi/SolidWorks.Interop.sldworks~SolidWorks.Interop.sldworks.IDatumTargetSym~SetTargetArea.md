<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetTargetArea.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetTargetArea Method (IDatumTargetSym) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html) : SetTargetArea Method (IDatumTargetSym) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Shape*
:   Target area shape or style as defined in swDatumTargetAreaShape\_e

*Size1*
:   Target area diameter or width (see **Remarks**)

*Size2*
:   Target area height (see Remarks)

Sets the datum target area style and size.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTargetArea( _    ByVal Shape As System.Integer, _    ByVal Size1 As System.String, _    ByVal Size2 As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDatumTargetSym Dim Shape As System.Integer Dim Size1 As System.String Dim Size2 As System.String Dim value As System.Boolean   value = instance.SetTargetArea(Shape, Size1, Size2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetTargetArea(     System.int Shape,    System.string Size1,    System.string Size2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetTargetArea(  &   System.int Shape, &   System.String^ Size1, &   System.String^ Size2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Shape*
:   Target area shape or style as defined in swDatumTargetAreaShape\_e

*Size1*
:   Target area diameter or width (see **Remarks**)

*Size2*
:   Target area height (see Remarks)

#### Return Value

True if the target area parameters were set successfully, false if they were not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DatumTargetSym::SetTargetArea.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If the target area style for this symbol is...** | **Then...** |
| Point | There is one size value, which might be empty. Retrieve the text using an index value of 0. SOLIDWORKS displays the text in the upper half of the symbol, preceded by a diameter character. |
| Circle | There is one size value. Retrieve the text using an index value of 0. SOLIDWORKS displays the text in the upper half of the symbol, preceded by a diameter character. |
| Rectangle | There are two size values. Retrieve the text using an index value of 0 and 1. SOLIDWORKS displays the texts in the upper half of the symbol, separated by an x character. |

If the specified target area style is not one of the values in swDatumTargetAreaShape\_e, SOLIDWORKS does not modify the symbol, and the returns false.

Use [IDatumTargetSym::GetTargetShape](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTargetSym~GetTargetShape.html) to get the target area style. Use [IDatumTargetSym::GetTargetAreaSize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTargetSym~GetTargetAreaSize.html) to get the target area size.

To see the model or drawing changes, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw your window.

# ![](dotnetimages/collapse.gif)See Also

####

[IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html)

[IDatumTargetSym Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0