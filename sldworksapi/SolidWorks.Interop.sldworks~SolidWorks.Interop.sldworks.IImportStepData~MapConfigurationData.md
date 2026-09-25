<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportStepData~MapConfigurationData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MapConfigurationData Property (IImportStepData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IImportStepData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportStepData.html) : MapConfigurationData Property (IImportStepData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to import the STEP file configuration data plus geometric data or geometric data only.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MapConfigurationData As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportStepData Dim value As System.Boolean   instance.MapConfigurationData = value   value = instance.MapConfigurationData ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MapConfigurationData {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool MapConfigurationData {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to import the STEP file configuration data plus geometric data, false to import geometric data only

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportStepData::MapConfigurationData.

# ![](dotnetimages/collapse.gif)Example

[Import STEP File (C#)](Import_STEP_File_Example_CSharp.htm)

[Import STEP File (VB.NET)](Import_STEP_File_Example_VBNET.htm)

[Import STEP File (VBA)](Import_STEP_File_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If this property is not set, then the current default environment setting, swImportStepConfigData, is used. If this property is set, its setting overrides the swImportStepConfigData setting for this import only.

# ![](dotnetimages/collapse.gif)See Also

####

[IImportStepData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportStepData.html)

[IImportStepData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportStepData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0