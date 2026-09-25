<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13~GetSheetFormatPath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetSheetFormatPath Method (ISwDMDocument13) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument13 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13.html) : GetSheetFormatPath Method (ISwDMDocument13) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SheetName*
:   Sheet name

*FormatPath*
:   Path and filename of the sheet format

Gets the path and filename of the sheet format used for the specified sheet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSheetFormatPath( _    ByVal SheetName As System.String, _    ByRef FormatPath As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument13 Dim SheetName As System.String Dim FormatPath As System.String Dim value As System.Integer   value = instance.GetSheetFormatPath(SheetName, FormatPath) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSheetFormatPath(     System.string SheetName,    out System.string FormatPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSheetFormatPath(  &   System.String^ SheetName, &   [Out] System.String^ FormatPath ) ``` | |

#### Parameters

*SheetName*
:   Sheet name

*FormatPath*
:   Path and filename of the sheet format

#### Return Value

Result as defined in [swSheetFormatPathResult](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.swSheetFormatPathResult.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument13::GetSheetFormatPath.

# ![](dotnetimages/collapse.gif)Example

[Get Drawing Sheets' Properties (C#)](Get_Drawing_Sheets_Properties_Example_CSharp.htm)

[Get Drawing Sheets' Properties (VB.NET)](Get_Drawing_Sheets_Properties_Example_vbnet.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only supports documents saved in SOLIDWORKS 2009 and later. An empty string is returned for documents saved in earlier versions of SOLIDWORKS.

Before calling this method, call [ISwDMDocument4::GetActiveSheetName](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument4~GetActiveSheetName.html) or [ISwDMDocument6::GetSheetNames](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument6~GetSheetNames.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument13 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13.html)

[ISwDMDocument13 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13_members.html)

[ISwDMDocument13::GetSheetProperties Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13~GetSheetProperties.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager 2009 SP0