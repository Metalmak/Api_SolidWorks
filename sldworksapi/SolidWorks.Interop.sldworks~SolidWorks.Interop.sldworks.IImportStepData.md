<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportStepData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IImportStepData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportStepData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IImportStepData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to specify values when importing STEP data.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IImportStepData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportStepData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IImportStepData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IImportStepData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportStepData.

# ![](dotnetimages/collapse.gif)Example

[Import STEP File (C#)](Import_STEP_File_Example_CSharp.htm)

[Import STEP File (VB.NET)](Import_STEP_File_Example_VBNET.htm)

[Import STEP File (VBA)](Import_STEP_File_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

1. Use [ISldWorks::GetImportFileData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetExportFileData.html) to get an IImportStepData interface pointer.- Use [IImportStepData::MapConfigurationData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IImportStepData~MapConfigurationData.html) to specify how to map configuration data.- Use [ISldWorks::LoadFile4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~LoadFile4.html) to load the file.

When IImportStepData is initialized, the current default environment setting, swImportStepConfigData, initializes IImportStepData::MapConfigurationData unless you explicitly set IImportStepData::MapConfigurationData. Then the IImportStepData::MapConfigurationData setting overrides swImportStepConfigData for this import only.

# ![](dotnetimages/collapse.gif)Accessors

[ISldWorks::GetImportFileData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetImportFileData.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[ImportStepData](SWObjectModel.pdf#ImportStepData)

# ![](dotnetimages/collapse.gif)See Also

####

[IImportStepData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportStepData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)