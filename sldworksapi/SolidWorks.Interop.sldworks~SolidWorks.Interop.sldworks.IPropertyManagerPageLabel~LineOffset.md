<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel~LineOffset.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LineOffset Property (IPropertyManagerPageLabel) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageLabel Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel.html) : LineOffset Property (IPropertyManagerPageLabel) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StartChar*
:   0-based index value of start character

*EndChar*
:   0-based index value of end character

Gets or sets whether to raise or lower the specified characters above or below their baselines, relative to their heights, in this PropertyManager label.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property LineOffset( _    ByVal StartChar As System.Short, _    ByVal EndChar As System.Short _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageLabel Dim StartChar As System.Short Dim EndChar As System.Short Dim value As System.Double   instance.LineOffset(StartChar, EndChar) = value   value = instance.LineOffset(StartChar, EndChar) ``` | |

| C# |  |
| --- | --- |
| ``` System.double LineOffset(     System.short StartChar,    System.short EndChar ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double LineOffset {    System.double get(System.short StartChar, System.short EndChar);    void set (System.short StartChar, System.short EndChar, System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StartChar*
:   0-based index value of start character

*EndChar*
:   0-based index value of end character

#### Property Value

Specify:

* 0.0 to show the character on its baseline

  * -1.0 to show the character 1 character below its baseline

    * +1.0 to show the character 1 character above its baseline

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageLabel::LineOffset.

# ![](dotnetimages/collapse.gif)Remarks

Offsetting (i.e., raising or lowering a character above or below its baseline, relative to its height) a character allows you to show that character as a subscript or exponent in an equation.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageLabel Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel.html)

[IPropertyManagerPageLabel Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0