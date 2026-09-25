<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBendTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBendTable Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : InsertBendTable Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   True to insert the bend table at the sheet format anchor point, false to insert it at the point specified by the X and Y parameters of this method

*X*
:   X-coordinate for placement of the bend table; valid only when UseAnchorPoint is false

*Y*
:   Y-coordinate for placement of the bend table; valid only when UseAnchorPoint is false

*AnchorType*
:   Anchor type as defined in swBomConfigurationAnchorType\_e

*StartValue*
:   Starting datum tag; a value from A to Z for letter tags; a positive integer for number tags

*TableTemplate*
:   Full pathname of the template (e.g., *install\_dir*\**lang\***language**\*****bendtable-standard.sldbndtbt**)

Inserts a bend table for this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBendTable( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal StartValue As System.String, _    ByVal TableTemplate As System.String _ ) As BendTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim StartValue As System.String Dim TableTemplate As System.String Dim value As BendTableAnnotation   value = instance.InsertBendTable(UseAnchorPoint, X, Y, AnchorType, StartValue, TableTemplate) ``` | |

| C# |  |
| --- | --- |
| ``` BendTableAnnotation InsertBendTable(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.string StartValue,    System.string TableTemplate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` BendTableAnnotation^ InsertBendTable(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ StartValue, &   System.String^ TableTemplate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   True to insert the bend table at the sheet format anchor point, false to insert it at the point specified by the X and Y parameters of this method

*X*
:   X-coordinate for placement of the bend table; valid only when UseAnchorPoint is false

*Y*
:   Y-coordinate for placement of the bend table; valid only when UseAnchorPoint is false

*AnchorType*
:   Anchor type as defined in swBomConfigurationAnchorType\_e

*StartValue*
:   Starting datum tag; a value from A to Z for letter tags; a positive integer for number tags

*TableTemplate*
:   Full pathname of the template (e.g., *install\_dir*\**lang\***language**\*****bendtable-standard.sldbndtbt**)

#### Return Value

[IBendTableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBendTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::InsertBendTable.

# ![](dotnetimages/collapse.gif)Example

[Insert Bend Table (VBA)](Insert_Bend_Table_Example_VB.htm)

[Insert Bend Table (VB.NET)](Insert_Bend_Table_Example_VBNET.htm)

[Insert Bend Table (C#)](Insert_Bend_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IBendTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendTable.html)

[IPartDoc::InsertBendTable Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertBendTable.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0