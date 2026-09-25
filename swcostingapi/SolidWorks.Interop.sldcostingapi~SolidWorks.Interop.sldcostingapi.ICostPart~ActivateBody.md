<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart~ActivateBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| ActivateBody Method (ICostPart) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostPart Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart.html) : ActivateBody Method (ICostPart) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodyName*
:   Name of Costing body to activate or an empty string to activate the common [Cost analysis](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis.html) for this Costing part (see **Remarks**)

*Errors*
:   Status as defined in [swcActivateBodyResult\_e](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.swcActivateBodyResult_e.html)

Activates the specified Costing body in the Costing part, which allows modifications to its Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ActivateBody( _    ByVal BodyName As System.String, _    ByRef Errors As System.Integer _ ) As CostBody ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostPart Dim BodyName As System.String Dim Errors As System.Integer Dim value As CostBody   value = instance.ActivateBody(BodyName, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` CostBody ActivateBody(     System.string BodyName,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CostBody^ ActivateBody(  &   System.String^ BodyName, &   [Out] System.int Errors ) ``` | |

#### Parameters

*BodyName*
:   Name of Costing body to activate or an empty string to activate the common [Cost analysis](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis.html) for this Costing part (see **Remarks**)

*Errors*
:   Status as defined in [swcActivateBodyResult\_e](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.swcActivateBodyResult_e.html)

#### Return Value

[Costing body](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostBody.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostPart::ActivateBody.

# ![](dotnetimages/collapse.gif)Remarks

To get the name of a Costing body for BodyName:

1. Get the Costing bodies in the Costing part by calling:

- [ICostPart::GetBodies](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostPart~GetBodies.html)
  - or -- [ICostPost::GetBodyCount](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostPart~GetBodyCount.html) and [ICostPart::IGetBodies](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostPart~IGetBodies.html).

2. Get the names of the Costing bodies in the Costing part by iterating through the array of returned Costing bodies and calling [ICostBody::GetName](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostBody~GetName.html).

Activating Costing bodies by their names allows you to use names directly from existing references to SOLIDWORKS bodies.

If you passed an empty string to BodyName, then **Return Value** is null and Errors is swcActivateBodyResult\_e.swcActivateBodyResult\_Success.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostPart Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart.html)

[ICostPart Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart_members.html)

[ICostPart::ActiveBody Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart~ActiveBody.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2013 SP0