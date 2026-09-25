<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ImportToolboxItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImportToolboxItem Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ImportToolboxItem Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StdToImport*
:   Standard to import (see **Remarks**)

*DestinationFilePath*
:   Path and name of file to import (see **Remarks**)

Imports data for the specified Toolbox standard.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ImportToolboxItem( _    ByVal StdToImport As System.String, _    ByVal DestinationFilePath As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim StdToImport As System.String Dim DestinationFilePath As System.String Dim value As System.Integer   value = instance.ImportToolboxItem(StdToImport, DestinationFilePath) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ImportToolboxItem(     System.string StdToImport,    System.string DestinationFilePath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ImportToolboxItem(  &   System.String^ StdToImport, &   System.String^ DestinationFilePath ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StdToImport*
:   Standard to import (see **Remarks**)

*DestinationFilePath*
:   Path and name of file to import (see **Remarks**)

#### Return Value

0 if the Toolbox standard imported successfully, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ImportToolboxItem.

# ![](dotnetimages/collapse.gif)Example

```
'VBA Preconditions'
```

```
'Open a part.
```

```
'Ensure the *.xlsx file exists.
```

```
Dim swApp As SldWorks.SldWorks
Dim SourceHWItem As String
Dim DestinationFoldeName As String
Dim longstatus As Long
Option Explicit
```

```
Sub Main()
```

```
    Set swApp = Application.SldWorks

    SourceHWItem = "ansi inch\bolts and screws\hex head\heavy hex bolt_ai.sldprt"

    DestinationFolderName = "C:\temp\AI_Heavy Hex Bolt.xlsx"

    longstatus = swApp.ImportToolboxItem(SourceHWItem, DestinationFolderName)

    Exit Sub

```

```
End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

Specify StdToImport with the path and file name beneath **C:\SOLIDWORKS Data\browser**, e.g., "**ansi inch\bolts and screws\hex head\heavy hex bolt\_ai.sldprt**".

Specify DestinationFilePath with the path and file name of the Excel Workbook (**\*.xslx**) you want to import. The Excel file name is formatted as follows:

> *standard***\_***hole class***\_***hole type***.xslx**

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::ExportToolboxItem Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ExportToolboxItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0