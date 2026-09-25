<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ITemplateOverrides~DefaultMachiningOperationTool.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| DefaultMachiningOperationTool Property (ITemplateOverrides) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ITemplateOverrides Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ITemplateOverrides.html) : DefaultMachiningOperationTool Property (ITemplateOverrides) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the tool for the default machining operation for machined parts.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DefaultMachiningOperationTool As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITemplateOverrides Dim value As System.Integer   instance.DefaultMachiningOperationTool = value   value = instance.DefaultMachiningOperationTool ``` | |

| C# |  |
| --- | --- |
| ``` System.int DefaultMachiningOperationTool {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int DefaultMachiningOperationTool {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Tool for the default machining operation as defined in [swcDefaultMachiningTool\_e](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.swcDefaultMachiningTool_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TemplateOverrides::DefaultMachiningOperationTool.

# ![](dotnetimages/collapse.gif)Remarks

Setting this property is only applied if:

* [ICostPart::GetCostingMethod](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart~GetCostingMethod.html) is either swcMethodType\_e.swcMethodType\_Machining or swcMethodType\_e.swcMethodType\_MachinedPlate.* [ITemplateOverrides::VolumeFeatureCalculationType](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ITemplateOverrides~VolumeFeatureCalculationType.html) is swcVolumeFeatureCalculationType\_e.swcVolumeFeatureCalculationType\_MachiningOperation.

# ![](dotnetimages/collapse.gif)See Also

####

[ITemplateOverrides Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ITemplateOverrides.html)

[ITemplateOverrides Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ITemplateOverrides_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0