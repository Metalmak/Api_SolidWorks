<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~Compare3DPMI.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Compare3DPMI Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : Compare3DPMI Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ReferenceDocument*
:   Path and file name of the open part document

*ModifiedDocument*
:   Path and file name of a different and open version of ReferenceDocument

*ReportName*
:   Name for the report and name of the folder to which to save the report and bitmap image files

*ReportFolderPath*
:   Path to the folder specified in ReportName in which to save the report and bitmap image files

*ReportSaveOptions*
:   Save options for the report as defined in sw3DPMISaveOptions\_e

Compare DimXpert annotations, reference dimensions, and other annotations between different versions of the same part document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Compare3DPMI( _    ByVal ReferenceDocument As System.String, _    ByVal ModifiedDocument As System.String, _    ByVal ReportName As System.String, _    ByVal ReportFolderPath As System.String, _    ByVal ReportSaveOptions As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim ReferenceDocument As System.String Dim ModifiedDocument As System.String Dim ReportName As System.String Dim ReportFolderPath As System.String Dim ReportSaveOptions As System.Integer Dim value As System.Boolean   value = instance.Compare3DPMI(ReferenceDocument, ModifiedDocument, ReportName, ReportFolderPath, ReportSaveOptions) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Compare3DPMI(     System.string ReferenceDocument,    System.string ModifiedDocument,    System.string ReportName,    System.string ReportFolderPath,    System.int ReportSaveOptions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Compare3DPMI(  &   System.String^ ReferenceDocument, &   System.String^ ModifiedDocument, &   System.String^ ReportName, &   System.String^ ReportFolderPath, &   System.int ReportSaveOptions ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReferenceDocument*
:   Path and file name of the open part document

*ModifiedDocument*
:   Path and file name of a different and open version of ReferenceDocument

*ReportName*
:   Name for the report and name of the folder to which to save the report and bitmap image files

*ReportFolderPath*
:   Path to the folder specified in ReportName in which to save the report and bitmap image files

*ReportSaveOptions*
:   Save options for the report as defined in sw3DPMISaveOptions\_e

#### Return Value

True if the method executed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::Compare3DPMI.

# ![](dotnetimages/collapse.gif)Example

[Compare DimXpert Annotations in Different Versions of Same Part (C#)](Compare_DimXpert_Annotations_in_Different_Versions_of_Same_Part_Example_CSharp.htm)

[Compare DimXpert Annotations in Different Versions of Same Part (VB.NET)](Compare_DimXpert_Annotations_in_Different_Versions_of_Same_Part_Example_VBNET.htm)

[Compare DimXpert Annotations in Different Versions of Same Part (VBA)](Compare_DimXpert_Annotations_in_Different_Versions_of_Same_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0