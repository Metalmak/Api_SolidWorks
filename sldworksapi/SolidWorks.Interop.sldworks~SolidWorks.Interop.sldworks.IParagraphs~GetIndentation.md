<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~GetIndentation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetIndentation Method (IParagraphs) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html) : GetIndentation Method (IParagraphs) |

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

Gets the indentation of the current paragraph.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetIndentation( _    ByRef FirstlineIndent As System.Double, _    ByRef Indent As System.Double, _    ByRef IndentIncrement As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParagraphs Dim FirstlineIndent As System.Double Dim Indent As System.Double Dim IndentIncrement As System.Double Dim value As System.Boolean   value = instance.GetIndentation(FirstlineIndent, Indent, IndentIncrement) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetIndentation(     out System.double FirstlineIndent,    out System.double Indent,    out System.double IndentIncrement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetIndentation(  &   [Out] System.double FirstlineIndent, &   [Out] System.double Indent, &   [Out] System.double IndentIncrement ) ``` | |

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

See Paragraphs::GetIndentation.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, set the current paragraph using [IParagraphs::CurrentParagraph](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~CurrentParagraph.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html)

[IParagraphs Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs_members.html)

[IParagraphs::SetIndentation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~SetIndentation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0