<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ImportHoleWizardItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImportHoleWizardItem Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ImportHoleWizardItem Method (ISldWorks) |

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

*ReplaceData*
:   True to replace data, false to not

*ErrorFile*
:   True to create an error file, false to not

Imports data for the specified Hole Wizard standard.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ImportHoleWizardItem( _    ByVal StdToImport As System.String, _    ByVal DestinationFilePath As System.String, _    ByVal ReplaceData As System.Boolean, _    ByVal ErrorFile As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim StdToImport As System.String Dim DestinationFilePath As System.String Dim ReplaceData As System.Boolean Dim ErrorFile As System.Boolean Dim value As System.Integer   value = instance.ImportHoleWizardItem(StdToImport, DestinationFilePath, ReplaceData, ErrorFile) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ImportHoleWizardItem(     System.string StdToImport,    System.string DestinationFilePath,    System.bool ReplaceData,    System.bool ErrorFile ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ImportHoleWizardItem(  &   System.String^ StdToImport, &   System.String^ DestinationFilePath, &   System.bool ReplaceData, &   System.bool ErrorFile ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StdToImport*
:   Standard to import (see **Remarks**)

*DestinationFilePath*
:   Path and name of file to import (see **Remarks**)

*ReplaceData*
:   True to replace data, false to not

*ErrorFile*
:   True to create an error file, false to not

#### Return Value

0 if the Hole Wizard standard imported successfully, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ImportHoleWizardItem.

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
```

```
Option Explicit
```

```
Sub Main()
```

```
    Set swApp = Application.SldWorks

    SourceHWItem = "ansi inch\Counterbore Holes\Hex Bolt"

    DestinationFolderName = "C:\temp\ANSI Inch_Counterbore Holes_Hex Bolt.xlsx"

    longstatus = swApp.ImportHoleWizardItem(SourceHWItem, DestinationFolderName, True, True)

    Exit Sub
```

```
End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

Specify StdToImport with the path and file name as shown on the Hole Wizard tab of the Toolbox, e.g., "**ansi inch\Counterbore Holes\Hex Bolt**".

Specify DestinationFilePath with the path and file name of the Excel Workbook (**\*.xslx**) you want to import. The Excel file name is formatted as follows:

> *standard***\_***hole class***\_***hole type***.xslx**

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::ExportHoleWizardItem Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ExportHoleWizardItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0