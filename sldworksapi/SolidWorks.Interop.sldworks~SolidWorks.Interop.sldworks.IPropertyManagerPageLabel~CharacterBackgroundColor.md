<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel~CharacterBackgroundColor.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CharacterBackgroundColor Property (IPropertyManagerPageLabel) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageLabel Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel.html) : CharacterBackgroundColor Property (IPropertyManagerPageLabel) |

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

Gets or sets the background color for the specified range of characters in this PropertyManager label.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CharacterBackgroundColor( _    ByVal StartChar As System.Short, _    ByVal EndChar As System.Short _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageLabel Dim StartChar As System.Short Dim EndChar As System.Short Dim value As System.Integer   instance.CharacterBackgroundColor(StartChar, EndChar) = value   value = instance.CharacterBackgroundColor(StartChar, EndChar) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CharacterBackgroundColor(     System.short StartChar,    System.short EndChar ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int CharacterBackgroundColor {    System.int get(System.short StartChar, System.short EndChar);    void set (System.short StartChar, System.short EndChar, System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StartChar*
:   0-based index value of start character

*EndChar*
:   0-based index value of end character

#### Property Value

RGB value for the text background color for the specified characters; if not specified, then the background color for this control is used

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageLabel::CharacterBackgroundColor.

# ![](dotnetimages/collapse.gif)Remarks

You can use a [group box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageGroup.html) with just a [label](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageLabel.html) to look like a [message box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~SetMessage3.html) on a PropertyManager page. Set the [background of the group box](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageGroup~BackgroundColor.html) and the background of the label to the same color and the [label text](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageLabel~CharacterColor.html) to a different color. You can also position the group box anywhere on the PropertyManager page.

NOTE: If you want to set the background color of the message box to be the same as the color typically used by SOLIDWORKS for a message box, use [ISldWorks::GetUserPreferenceIntegerValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceIntegerValue.html) swPropertyManagerColorImportantMessage to get the COLORREF value.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageLabel Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel.html)

[IPropertyManagerPageLabel Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageLabel_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0