<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ExportToolboxItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ExportToolboxItem Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ExportToolboxItem Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StdToExport*
:   Standard to export (see **Remarks**)

*DestinationFolderPath*
:   Path where to export the data (see **Remarks**)

Exports data for the specified Toolbox standard.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExportToolboxItem( _    ByVal StdToExport As System.String, _    ByVal DestinationFolderPath As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim StdToExport As System.String Dim DestinationFolderPath As System.String Dim value As System.Integer   value = instance.ExportToolboxItem(StdToExport, DestinationFolderPath) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ExportToolboxItem(     System.string StdToExport,    System.string DestinationFolderPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ExportToolboxItem(  &   System.String^ StdToExport, &   System.String^ DestinationFolderPath ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StdToExport*
:   Standard to export (see **Remarks**)

*DestinationFolderPath*
:   Path where to export the data (see **Remarks**)

#### Return Value

0 if successful, 1 if errors

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ExportToolboxItem.

# ![](dotnetimages/collapse.gif)Example

```
'VBA Preconditions'
```

```
'Open a part.
```

```
'Ensure that c:\temp exists.
```

```
Dim swApp As SldWorks.SldWorks
Dim SourceHWItem As String
Dim DestinationFoldeName As String
Dim longstatus As Long
```

```
Option Explicit
```

```
Sub Main()
```

```
    Set swApp = Application.SldWorks

    SourceHWItem = "ansi inch\bolts and screws\hex head\heavy hex bolt_ai.sldprt"

    DestinationFolderName = "C:\temp"

    longstatus = swApp.ExportToolboxItem(SourceHWItem, DestinationFolderName)

    Exit Sub

```

```
End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

Specify StdToImport with the path and file name beneath **C:\SOLIDWORKS Data\browser**, e.g., "**ansi inch\bolts and screws\hex head\heavy hex bolt\_ai.sldprt**".

Specify DestinationFolderPath with the path where to export the Excel Workbook (**\*.xslx**). The data is exported to a file whose name is formatted as follows:

> *standard***\_***hole class***\_***hole type***.xslx**

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::ImportToolboxItem Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ImportToolboxItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0