<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenedFileInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetOpenedFileInfo Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetOpenedFileInfo Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Full path and filename of the last model successfully opened by SOLIDWORKS

*Options*
:   Options in effect when FileName opened as defined in swOpenDocOptions\_e

Gets the name of the last model successfully opened by SOLIDWORKS and the options that were in effect when it opened.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetOpenedFileInfo( _    ByRef FileName As System.String, _    ByRef Options As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FileName As System.String Dim Options As System.Integer   instance.GetOpenedFileInfo(FileName, Options) ``` | |

| C# |  |
| --- | --- |
| ``` void GetOpenedFileInfo(     out System.string FileName,    out System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetOpenedFileInfo(  &   [Out] System.String^ FileName, &   [Out] System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Full path and filename of the last model successfully opened by SOLIDWORKS

*Options*
:   Options in effect when FileName opened as defined in swOpenDocOptions\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetOpenedFileInfo.

# ![](dotnetimages/collapse.gif)Example

```
'VBA
```

```
Dim swApp As SldWorks.SldWorks
Dim path As String
Dim docspec As SldWorks.DocumentSpecification
Dim opened As String
Dim Options As Long
Dim Part As SldWorks.ModelDoc2
Dim boolstatus As Boolean
Dim longstatus As Long, longwarnings As Long
Option Explicit
Sub main()
```

```
    Set swApp = Application.SldWorks
    swApp.CloseAllDocuments True
    path = "C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\tutorial\api\bagel.sldprt"
    Set docspec = swApp.GetOpenDocSpec(path)
    Set Part = swApp.OpenDoc7(docspec)
    Set Part = swApp.OpenDoc6("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\tutorial\api\coffeecup.sldprt", 1, 0, "", longstatus, longwarnings)
    Set Part = swApp.OpenDoc6("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\tutorial\api\toaster.sldprt", 1, 0, "", longstatus, longwarnings)

    ' None of the above documents successfully opened through the API get returned by GetOpenedFileInfo
    swApp.GetOpenedFileInfo opened, Options
    Debug.Print "Last successfully opened file: " & opened
    Debug.Print "Options as defined in swOpenDocOptions_e: " & Options

End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

This method considers only models opened through the SOLIDWORKS user interface. This method does not consider models successfully opened through the API, unless the API opens an assembly. In that case, each assembly component is opened by SOLIDWORKS, and this method determines which of those assembly's components was successfully opened last.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetOpenDocument Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenDocument.html)

[ISldWorks::GetOpenDocumentByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenDocumentByName.html)

[ISldWorks::GetOpenFileName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetOpenFileName.html)

[ISldWorks::IGetOpenDocumentByName2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetOpenDocumentByName2.html)

[ISldWorks::EnumDocuments2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~EnumDocuments2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0