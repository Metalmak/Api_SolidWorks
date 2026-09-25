<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertWeldTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertWeldTable Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : InsertWeldTable Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   If true and the appropriate sheet format anchor point exists, then insert the table at the anchor point; if false, then use the values specified for the X and Y arguments as the insertion point

*IncludeAnnotations*
:   True to include weld symbols not attached to cosmetic weld features, false to not

*CombineSameType*
:   True to group welds having the same weld symbol and weld size, false to not

*X*
:   X coordinate in meters for the placement of the weld table; valid only if UseAnchorPoint = False

*Y*
:   Y coordinate in meters for the placement of the weld table; valid only if UseAnchorPoint = False

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*Configuration*
:   Name of the part configuration for which to insert the weld table

*TableTemplate*
:   Path and filename of the template that corresponds to this type of table (see Remarks)

Inserts a weld table into this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertWeldTable( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal IncludeAnnotations As System.Boolean, _    ByVal CombineSameType As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal Configuration As System.String, _    ByVal TableTemplate As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim UseAnchorPoint As System.Boolean Dim IncludeAnnotations As System.Boolean Dim CombineSameType As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim Configuration As System.String Dim TableTemplate As System.String Dim value As System.Boolean   value = instance.InsertWeldTable(UseAnchorPoint, IncludeAnnotations, CombineSameType, X, Y, AnchorType, Configuration, TableTemplate) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertWeldTable(     System.bool UseAnchorPoint,    System.bool IncludeAnnotations,    System.bool CombineSameType,    System.double X,    System.double Y,    System.int AnchorType,    System.string Configuration,    System.string TableTemplate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertWeldTable(  &   System.bool UseAnchorPoint, &   System.bool IncludeAnnotations, &   System.bool CombineSameType, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ Configuration, &   System.String^ TableTemplate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   If true and the appropriate sheet format anchor point exists, then insert the table at the anchor point; if false, then use the values specified for the X and Y arguments as the insertion point

*IncludeAnnotations*
:   True to include weld symbols not attached to cosmetic weld features, false to not

*CombineSameType*
:   True to group welds having the same weld symbol and weld size, false to not

*X*
:   X coordinate in meters for the placement of the weld table; valid only if UseAnchorPoint = False

*Y*
:   Y coordinate in meters for the placement of the weld table; valid only if UseAnchorPoint = False

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*Configuration*
:   Name of the part configuration for which to insert the weld table

*TableTemplate*
:   Path and filename of the template that corresponds to this type of table (see Remarks)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::InsertWeldTable.

# ![](dotnetimages/collapse.gif)Example

[Insert Weld Table (VBA)](Insert_Weld_Table_Example_VB.htm)

[Insert Weld Table (VB.NET)](Insert_Weld_Table_Example_VBNET.htm)

[Insert Weld Table (C#)](Insert_Weld_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The weld table template installed with SOLIDWORKS is <*SOLIDWORKS\_*install\_dir>\lang\<language>\**weldtable-standard.sldwldtbt**.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0