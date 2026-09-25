<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenFileName2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetOpenFileName2 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetOpenFileName2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DialogTitle*
:   Title of the dialog

*InitialFileName*
:   Path and file name of the file to open

*FileFilter*
:   File name extension of the file to open

*OpenOptions*
:   Open options as defined by swGetOpenFileNameOptions\_e

*ConfigName*
:   Name of configuration of InitialFileName; comma-separated list of sheet names beginning with active sheet if OpenOptions is swGetOpenFileNameOptions\_e.swGetOpenFileNameOptions\_SelectedSheets

*DisplayName*
:   Recommended name to use for opened file

*DisplayStateName*
:   Selected display state name

Prompts the user for the name of the file to open.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetOpenFileName2( _    ByVal DialogTitle As System.String, _    ByVal InitialFileName As System.String, _    ByVal FileFilter As System.String, _    ByRef OpenOptions As System.Integer, _    ByRef ConfigName As System.String, _    ByRef DisplayName As System.String, _    ByRef DisplayStateName As System.String _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DialogTitle As System.String Dim InitialFileName As System.String Dim FileFilter As System.String Dim OpenOptions As System.Integer Dim ConfigName As System.String Dim DisplayName As System.String Dim DisplayStateName As System.String Dim value As System.String   value = instance.GetOpenFileName2(DialogTitle, InitialFileName, FileFilter, OpenOptions, ConfigName, DisplayName, DisplayStateName) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetOpenFileName2(     System.string DialogTitle,    System.string InitialFileName,    System.string FileFilter,    out System.int OpenOptions,    out System.string ConfigName,    out System.string DisplayName,    out System.string DisplayStateName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetOpenFileName2(  &   System.String^ DialogTitle, &   System.String^ InitialFileName, &   System.String^ FileFilter, &   [Out] System.int OpenOptions, &   [Out] System.String^ ConfigName, &   [Out] System.String^ DisplayName, &   [Out] System.String^ DisplayStateName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DialogTitle*
:   Title of the dialog

*InitialFileName*
:   Path and file name of the file to open

*FileFilter*
:   File name extension of the file to open

*OpenOptions*
:   Open options as defined by swGetOpenFileNameOptions\_e

*ConfigName*
:   Name of configuration of InitialFileName; comma-separated list of sheet names beginning with active sheet if OpenOptions is swGetOpenFileNameOptions\_e.swGetOpenFileNameOptions\_SelectedSheets

*DisplayName*
:   Recommended name to use for opened file

*DisplayStateName*
:   Selected display state name

#### Return Value

Path and file name of the file to open

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetOpenFileName2.

# ![](dotnetimages/collapse.gif)Example

[Open File (VBA)](Open_File_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30