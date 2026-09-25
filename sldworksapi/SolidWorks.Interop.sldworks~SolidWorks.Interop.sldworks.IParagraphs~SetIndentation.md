<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~SetIndentation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetIndentation Method (IParagraphs) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html) : SetIndentation Method (IParagraphs) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstlineIndent*
:   Indentation of first line

*Indent*
:   Indentation of lines other than the first line

*IndentIncrement*
:   Amount by which to increment the current indents

Sets the indentation of the current paragraph.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetIndentation( _    ByVal FirstlineIndent As System.Double, _    ByVal Indent As System.Double, _    ByVal IndentIncrement As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParagraphs Dim FirstlineIndent As System.Double Dim Indent As System.Double Dim IndentIncrement As System.Double Dim value As System.Boolean   value = instance.SetIndentation(FirstlineIndent, Indent, IndentIncrement) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetIndentation(     System.double FirstlineIndent,    System.double Indent,    System.double IndentIncrement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetIndentation(  &   System.double FirstlineIndent, &   System.double Indent, &   System.double IndentIncrement ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FirstlineIndent*
:   Indentation of first line

*Indent*
:   Indentation of lines other than the first line

*IndentIncrement*
:   Amount by which to increment the current indents

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Paragraphs::SetIndentation.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, set the current paragraph using [IParagraphs::CurrentParagraph](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~CurrentParagraph.html).

After calling this method, call [IParagraphs::UpdateParagraph](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~UpdateParagraph.html) to update the model.

# ![](dotnetimages/collapse.gif)See Also

####

[IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html)

[IParagraphs Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs_members.html)

[IParagraphs::GetIndentation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~GetIndentation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0