<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~ImportScheme.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| ImportScheme Method (IDimXpertPart) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html) : ImportScheme Method (IDimXpertPart) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Filename*
:   Full path name of the file whose tolerance scheme to import to ConfigurationName

*ConfigurationName*
:   Name of the configuration in the open model document to which to import the tolerance scheme

Imports the tolerance scheme of the specified file to the specified configuration of this open model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ImportScheme( _    ByVal Filename As System.String, _    ByVal ConfigurationName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertPart Dim Filename As System.String Dim ConfigurationName As System.String Dim value As System.Boolean   value = instance.ImportScheme(Filename, ConfigurationName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ImportScheme(     System.string Filename,    System.string ConfigurationName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ImportScheme(  &   System.String^ Filename, &   System.String^ ConfigurationName ) ``` | |

#### Parameters

*Filename*
:   Full path name of the file whose tolerance scheme to import to ConfigurationName

*ConfigurationName*
:   Name of the configuration in the open model document to which to import the tolerance scheme

#### Return Value

True if tolerance scheme successfully imported, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertPart::ImportScheme.

# ![](dotnetimages/collapse.gif)Example

'VBA

'1. Open a model document with a Default configuration.

'2. Edit the ImportScheme command to point to a model document with the tolerance scheme to import.

'3. Run the macro.

Option Explicit
Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim swModelDocExt As SldWorks.ModelDocExtension
Dim swSchema As SldWorks.DimXpertManager
Dim swDXPart As DimXpertPart
Dim status As Boolean
Sub main()

    Set swApp = Application.SldWorks
    Set swModel = swApp.ActiveDoc
    Set swModelDocExt = swModel.Extension
    Set swSchema = swModelDocExt.DimXpertManager("Default", True)
    Set swDXPart = swSchema.DimXpertPart

    status = swDXPart.**ImportScheme**("*Path\_name*\*model\_name*.SLDPRT", "Default")

End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html)

[IDimXpertPart Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0