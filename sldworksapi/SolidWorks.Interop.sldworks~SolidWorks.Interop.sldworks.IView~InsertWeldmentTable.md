<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertWeldmentTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertWeldmentTable Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : InsertWeldmentTable Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   If true and the appropriate sheet format anchor point exists, then insert table at this point; if false, then use the values specified for the X and Y arguments as the insertion point

*X*
:   X coordinate for the placement of the weldment cut-list table; valid only if UserAnchorPoint = False

*Y*
:   Y coordinate for the placement of the weldment cut-list table; valid only if UseAnchorPoint = False

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*Configuration*
:   Name of the "As Welded" configuration for the weldment cut-list table

*TableTemplate*
:   Path and filename of the template that corresponds to this type of table (see Remarks)

Inserts a weldment cut-list table into this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertWeldmentTable( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal Configuration As System.String, _    ByVal TableTemplate As System.String _ ) As WeldmentCutListAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim Configuration As System.String Dim TableTemplate As System.String Dim value As WeldmentCutListAnnotation   value = instance.InsertWeldmentTable(UseAnchorPoint, X, Y, AnchorType, Configuration, TableTemplate) ``` | |

| C# |  |
| --- | --- |
| ``` WeldmentCutListAnnotation InsertWeldmentTable(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.string Configuration,    System.string TableTemplate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` WeldmentCutListAnnotation^ InsertWeldmentTable(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ Configuration, &   System.String^ TableTemplate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   If true and the appropriate sheet format anchor point exists, then insert table at this point; if false, then use the values specified for the X and Y arguments as the insertion point

*X*
:   X coordinate for the placement of the weldment cut-list table; valid only if UserAnchorPoint = False

*Y*
:   Y coordinate for the placement of the weldment cut-list table; valid only if UseAnchorPoint = False

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*Configuration*
:   Name of the "As Welded" configuration for the weldment cut-list table

*TableTemplate*
:   Path and filename of the template that corresponds to this type of table (see Remarks)

#### Return Value

[Weldment cut-list annotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldmentCutListAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::InsertWeldmentTable.

# ![](dotnetimages/collapse.gif)Example

[Insert Weldment Cut List Table (VBA)](Insert_Weldment_Cut_List_Table_Example_VB.htm)

[Insert Weldment Cut List Table (VB.NET)](Insert_Weldment_Cut_List_Table_Example_VBNET.htm)

[Insert Weldment Cut List Table (C#)](Insert_Weldment_Cut_List_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The weldment cut-list table template installed with SOLIDWORKS is <*SOLIDWORKS\_*install\_dir>\lang\<language>\**cut list.sldwldtbt**.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetKeepLinkedToBOM Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetKeepLinkedToBOM.html)

[IView::GetKeepLinkedToBOMName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetKeepLinkedToBOMName.html)

[IView::SetKeepLinkedToBOM Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetKeepLinkedToBOM.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0