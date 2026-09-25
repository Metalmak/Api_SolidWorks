<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~SetBulletsAndNumbering.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBulletsAndNumbering Method (IParagraphs) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html) : SetBulletsAndNumbering Method (IParagraphs) |

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

Sets the list properties of the current paragraph.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBulletsAndNumbering( _    ByVal ParagraphType As System.Integer, _    ByVal NumberingType As System.Integer, _    ByVal StartAt As System.Integer, _    ByVal Type As System.Integer, _    ByVal Format As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParagraphs Dim ParagraphType As System.Integer Dim NumberingType As System.Integer Dim StartAt As System.Integer Dim Type As System.Integer Dim Format As System.Integer Dim value As System.Boolean   value = instance.SetBulletsAndNumbering(ParagraphType, NumberingType, StartAt, Type, Format) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetBulletsAndNumbering(     System.int ParagraphType,    System.int NumberingType,    System.int StartAt,    System.int Type,    System.int Format ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetBulletsAndNumbering(  &   System.int ParagraphType, &   System.int NumberingType, &   System.int StartAt, &   System.int Type, &   System.int Format ) ``` | |

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

See Paragraphs::SetBulletsAndNumbering.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, set the current paragraph using [IParagraphs::CurrentParagraph](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~CurrentParagraph.html).

After calling this method, call [IParagraphs::UpdateParagraph](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~UpdateParagraph.html) to update the model.

# ![](dotnetimages/collapse.gif)See Also

####

[IParagraphs Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs.html)

[IParagraphs Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs_members.html)

[IParagraphs::GetBulletsAndNumbering Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParagraphs~GetBulletsAndNumbering.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0