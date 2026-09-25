<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration16~GetCutListItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetCutListItems Method (ISwDMConfiguration16) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMConfiguration16 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration16.html) : GetCutListItems Method (ISwDMConfiguration16) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the cut-list items for this configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCutListItems() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMConfiguration16 Dim value As System.Object   value = instance.GetCutListItems() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetCutListItems() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetCutListItems(); ``` | |

#### Return Value

Array of [cut-list items](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMCutListItem3.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMConfiguration16::GetCutListItems.

# ![](dotnetimages/collapse.gif)Example

[Get, Add, Change, and Delete Cut-List Custom Properties (VB.NET)](Get%2C_Add%2C_Change%2C_and_Delete_Cut-List_Custom_Properties_Example_VBNET.htm)

[Get, Add, Change, and Delete Cut-List Custom Properties (C#)](Get%2C_Add%2C_Change%2C_and_Delete_Cut-List_Custom_Properties_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only works with documents saved in SOLIDWORKS 2019 or later for:

* the active configuration

    - or -

* those configurations for which **Add Rebuild on Save Mark** was selected in the SOLIDWORKS ConfigurationManager before the document was saved.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMConfiguration16 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration16.html)

[ISwDMConfiguration16 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration16_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2019 SP0