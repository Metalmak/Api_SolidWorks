<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13~GetLastUpdateTimeStamp.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetLastUpdateTimeStamp Method (ISwDMDocument13) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument13 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13.html) : GetLastUpdateTimeStamp Method (ISwDMDocument13) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the last update stamp for this document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetLastUpdateTimeStamp() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument13 Dim value As System.Integer   value = instance.GetLastUpdateTimeStamp() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetLastUpdateTimeStamp() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetLastUpdateTimeStamp(); ``` | |

#### Return Value

Last update stamp in time\_t format

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument13::GetLastUpdateTimeStamp.

# ![](dotnetimages/collapse.gif)Example

[Get, Add, Change, and Delete Cut-List Custom Properties (C#)](Get%2C_Add%2C_Change%2C_and_Delete_Cut-List_Custom_Properties_Example_CSharp.htm)

[Get, Add, Change, and Delete Cut-List Custom Properties (VB.NET)](Get%2C_Add%2C_Change%2C_and_Delete_Cut-List_Custom_Properties_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The return value is in time\_t format, which Microsoft defines "as time as seconds elapsed since midnight, January 1, 1970 or -1 in the case of error". You must either have built-in functions to convert this value to something more accessible or write your own functions.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument13 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13.html)

[ISwDMDocument13 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2009 SP0