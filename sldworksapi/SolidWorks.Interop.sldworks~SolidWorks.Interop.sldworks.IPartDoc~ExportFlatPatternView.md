<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ExportFlatPatternView.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ExportFlatPatternView Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : ExportFlatPatternView Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePath*
:   Path and filename to which to save the sheet metal part in its flattened state to a DXF/DWG file

*Options*
:   Option as described in swExportFlatPatternViewOptions\_e

Obsolete. Superseded by [IPartDoc::ExportToDWG2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ExportToDWG2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExportFlatPatternView( _    ByVal FilePath As System.String, _    ByVal Options As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim FilePath As System.String Dim Options As System.Integer Dim value As System.Boolean   value = instance.ExportFlatPatternView(FilePath, Options) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ExportFlatPatternView(     System.string FilePath,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ExportFlatPatternView(  &   System.String^ FilePath, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePath*
:   Path and filename to which to save the sheet metal part in its flattened state to a DXF/DWG file

*Options*
:   Option as described in swExportFlatPatternViewOptions\_e

#### Return Value

True if the sheet metal part is enabled to be saved in its flattened state to a DXF/DWG file at the specified path and filename, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::ExportFlatPatternView.

# ![](dotnetimages/collapse.gif)Example

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim swModel As SldWorks.ModelDoc2

Dim swModelDocExt As SldWorks.ModelDocExtension

Dim boolstatus As Boolean

Dim longstatus As Long, longwarnings As Long

Sub main()

Set swApp = Application.SldWorks

Set swModel = swApp.ActiveDoc

Set swModelDocExt = swModel.Extension

boolstatus = swModel.ExportFlatPatternView("F:\Test\Flat pattern - sheet\_metal\_cover.DXF", swExportFlatPatternOption\_None)

swModelDocExt.SaveAs "F:\Test\Flat pattern - sheet\_metal\_cover.DXF", 0, 0, Nothing, longstatus, longwarnings

End Sub

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IModelDocExtension::SaveAs](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SaveAs.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::ExportToDWG2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ExportToDWG2.html)

[IPartDoc::IExportToDWG2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~IExportToDWG2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0