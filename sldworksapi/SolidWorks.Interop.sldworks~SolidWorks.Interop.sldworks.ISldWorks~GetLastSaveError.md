<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetLastSaveError.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetLastSaveError Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetLastSaveError Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePath*
:   Path name of the document causing the save error

*ErrorCode*
:   :   Error code of the save

Gets the last save error issued by Microsoft in the current session.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetLastSaveError( _    ByRef FilePath As System.Object, _    ByRef ErrorCode As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FilePath As System.Object Dim ErrorCode As System.Object Dim value As System.Object   value = instance.GetLastSaveError(FilePath, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetLastSaveError(     out System.object FilePath,    out System.object ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetLastSaveError(  &   [Out] System.Object^ FilePath, &   [Out] System.Object^ ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePath*
:   Path name of the document causing the save error

*ErrorCode*
:   :   Error code of the save

#### Return Value

Text message of the save error

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetLastSaveError.

# ![](dotnetimages/collapse.gif)Example

[Get Last Save Error (VBA)](Get_Last_Save_Error_Example_VB.htm)

[Get Last Save Error (VB.NET)](Get_Last_Save_Error_Example_VBNET.htm)

[Get Last Save Error (C#)](Get_Last_Save_Error_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetErrorMessages Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetErrorMessages.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0