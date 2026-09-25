<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertTitleBlockTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertTitleBlockTable Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertTitleBlockTable Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplateName*
:   Fully qualified path and name of the title block table template

*X*
:   x coordinate for upper-left corner of title block table

*Y*
:   y coordinate for upper-left corner of title block table

Inserts a title block table in a part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertTitleBlockTable( _    ByVal TemplateName As System.String, _    ByVal X As System.Integer, _    ByVal Y As System.Integer _ ) As TitleBlockTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim TemplateName As System.String Dim X As System.Integer Dim Y As System.Integer Dim value As TitleBlockTableAnnotation   value = instance.InsertTitleBlockTable(TemplateName, X, Y) ``` | |

| C# |  |
| --- | --- |
| ``` TitleBlockTableAnnotation InsertTitleBlockTable(     System.string TemplateName,    System.int X,    System.int Y ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` TitleBlockTableAnnotation^ InsertTitleBlockTable(  &   System.String^ TemplateName, &   System.int X, &   System.int Y ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TemplateName*
:   Fully qualified path and name of the title block table template

*X*
:   x coordinate for upper-left corner of title block table

*Y*
:   y coordinate for upper-left corner of title block table

#### Return Value

[Title block table annotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITitleBlockTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertTitleBlockTable.

# ![](dotnetimages/collapse.gif)Example

[Get Title Block Tables (VBA)](Get_Title_Block_Tables_Example_VB6.htm)

[Get Title Block Tables (VB.NET)](Get_Title_Block_Tables_Example_VBNET.htm)

[Get Title Block Tables (C#)](Get_Title_Block_Tables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Title block table templates have a filename extension of .sldtbt.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::InsertGeneralTableAnnotation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertGeneralTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0