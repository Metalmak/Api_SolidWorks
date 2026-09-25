<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~GetBulletsAndNumbering.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBulletsAndNumbering Method (IParagraphs) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html) : GetBulletsAndNumbering Method (IParagraphs) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ParagraphType*
:   List type as defined in swParagraphType\_e

*NumberingType*
:   Numbering direction as defined in swNumberedListStartType\_e; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

*StartAt*
:   Letter or number starting this numbered list, depending on Type; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

*Type*
:   Numbered list type as defined in swNumberedListType\_e; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

*Format*
:   Numbered list format as defined in swNumberingFormat\_e; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

Gets the list properties of the current paragraph.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBulletsAndNumbering( _    ByRef ParagraphType As System.Integer, _    ByRef NumberingType As System.Integer, _    ByRef StartAt As System.Integer, _    ByRef Type As System.Integer, _    ByRef Format As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParagraphs Dim ParagraphType As System.Integer Dim NumberingType As System.Integer Dim StartAt As System.Integer Dim Type As System.Integer Dim Format As System.Integer Dim value As System.Boolean   value = instance.GetBulletsAndNumbering(ParagraphType, NumberingType, StartAt, Type, Format) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetBulletsAndNumbering(     out System.int ParagraphType,    out System.int NumberingType,    out System.int StartAt,    out System.int Type,    out System.int Format ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetBulletsAndNumbering(  &   [Out] System.int ParagraphType, &   [Out] System.int NumberingType, &   [Out] System.int StartAt, &   [Out] System.int Type, &   [Out] System.int Format ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ParagraphType*
:   List type as defined in swParagraphType\_e

*NumberingType*
:   Numbering direction as defined in swNumberedListStartType\_e; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

*StartAt*
:   Letter or number starting this numbered list, depending on Type; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

*Type*
:   Numbered list type as defined in swNumberedListType\_e; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

*Format*
:   Numbered list format as defined in swNumberingFormat\_e; valid only if ParagraphType is swParagraphType\_e.swParagraphNumbered

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Paragraphs::GetBulletsAndNumbering.

# ![](dotnetimages/collapse.gif)Example

See the [IParagraphs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, set the current paragraph using [IParagraphs::CurrentParagraph](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~CurrentParagraph.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html)

[IParagraphs Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs_members.html)

[IParagraphs::SetBulletsAndNumbering Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~SetBulletsAndNumbering.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0