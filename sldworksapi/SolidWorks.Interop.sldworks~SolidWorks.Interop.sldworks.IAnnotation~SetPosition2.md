<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetPosition2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPosition2 Method (IAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : SetPosition2 Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X coordinate of the origin of the annotation

*Y*
:   Y coordinate of the origin of the annotation

*Z*
:   Z coordinate of the origin of the annotation

Sets the position of this annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPosition2( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As System.Boolean   value = instance.SetPosition2(X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetPosition2(     System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetPosition2(  &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X coordinate of the origin of the annotation

*Y*
:   Y coordinate of the origin of the annotation

*Z*
:   Z coordinate of the origin of the annotation

#### Return Value

True if the position of the annotation is successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::SetPosition2.

# ![](dotnetimages/collapse.gif)Example

[Insert a Note (VBA)](Insert_a_Note_Example_VB.htm)

[Insert a Note (VB.NET)](Insert_a_Note_Example_VBNET.htm)

[Insert a Note (C#)](Insert_a_Note_Example_CSharp.htm)

[Traverse Annotations (C#)](Traverse_Annotations_Example_CSharp.htm)

[Traverse Annotations (VB.NET)](Traverse_Annotations_Example_VBNET.htm)

[Traverse Annotations (VBA)](Traverse_Annotations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The following table lists the types of annotations that this method supports and the position of the x, y, z origin. In a drawing, the x, y, z origin is relative to the origin of the drawing sheet (the lower-left corner of the sheet).

|  |  |
| --- | --- |
| **Type of Annotation** | **Position of XYZ Origin** |
| [Datum Feature Symbols](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTag.html) | Point where leader hits symbol |
| [Datum Target Symbols](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTargetSym.html) | Center point of the circle that is attached to the leader |
| [Display dimensions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension.html) | Point of leader attachment centered on a text box border / center point of bottom border of text box |
| [Geometric Tolerances](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol.html) | Upper-left corner of the symbol |
| [Notes](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html) | Upper-left corner of the text box |
| [Revision Clouds](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud.html) | Position of x,y,z determined by [IRevisionCloud::Shape](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~Shape.html) |
| [Surface Finish Symbols](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol.html) | Lower-left point of symbol |
| [Table Annotations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html) | Position of x,y,z determined by [ITableAnnotation::AnchorType](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~AnchorType.html) |
| [Weld Symbols](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol.html) | Left endpoint of the main horizontal line in the symbol |

If you use this method on any other types of annotations, SOLIDWORKS takes no action and returns false.

The position of an annotation can be subject to certain restrictions. These restrictions apply to setting the position through the user interface and using this method. One example of a restriction is a surface-finish symbol that is inserted directly on a face (that is, no leaders). It can only be moved within the borders of that face. If it is inserted directly on an edge, it can only be moved along that edge or extensions of that edge. Datum feature symbols have similar restrictions. If this method attempts to set a position of an annotation that violates any restrictions, the annotation is placed as near as possible to the specified position.

The position of table annotations cannot be set if the table is anchored. Use [ITableAnnotation::Anchored](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~Anchored.html) to determine if the table is anchored.

|  |  |
| --- | --- |
| **If a dimension has [offset text](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~OffsetText.html), and you want to move...** | **Then...** |
| Dimension text, dimension line, and extension lines | 1. Turn offset text off.- Use this method to move the dimension text, dimension line, and extension lines.- Turn offset text back on. |
| Dimension text only | Use this method to move the dimension text. The dimension line and extension lines will not move. |

Because radial and diametric dimensions are already attached to the end of a leader, this property is not available for these types of dimensions.

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

[IAnnotation::GetPosition Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetPosition.html)

[INote::LockPosition Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~LockPosition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 SP3, Revision Number 22.3