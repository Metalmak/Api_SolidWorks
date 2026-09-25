<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart~SetCostingMethod.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| SetCostingMethod Method (ICostPart) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostPart Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart.html) : SetCostingMethod Method (ICostPart) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodyName*
:   Name of the Costing body (see **Remarks**)

*MethodType*
:   Manufacturing type as defined in [swcMethodType\_e](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.swcMethodType_e.html)

Sets the manufacturing method for this Costing part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetCostingMethod( _    ByVal BodyName As System.String, _    ByVal MethodType As System.Integer _ ) As CostBody ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostPart Dim BodyName As System.String Dim MethodType As System.Integer Dim value As CostBody   value = instance.SetCostingMethod(BodyName, MethodType) ``` | |

| C# |  |
| --- | --- |
| ``` CostBody SetCostingMethod(     System.string BodyName,    System.int MethodType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CostBody^ SetCostingMethod(  &   System.String^ BodyName, &   System.int MethodType ) ``` | |

#### Parameters

*BodyName*
:   Name of the Costing body (see **Remarks**)

*MethodType*
:   Manufacturing type as defined in [swcMethodType\_e](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.swcMethodType_e.html)

#### Return Value

[Costing body](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostBody.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostPart::SetCostingMethod.

# ![](dotnetimages/collapse.gif)Example

[Create 3D Printing Costing Analysis (C#)](Create_3D_Printing_Costing_Analysis_Example_CSharp.htm)

[Create 3D Printing Costing Analysis (VB.NET)](Create_3D_Printing_Costing_Analysis_Example_VBNET.htm)

[Create 3D Printing Costing Analysis (VBA)](Create_3D_Printing_Costing_Analysis_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you specify:

* a name for BodyName, then the current body is deleted and a new body of the type that you specified in MethodType is created. This method returns the newly created body and invalidates any previously selected bodies.* an empty string for BodyName, then the body in a single body part or the currently selected body in a multibody part is used. This method returns this body.

For a [structural Costing analysis](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html), specify the name of the cut-list item for BodyName to use for the manufacturing method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostPart Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart.html)

[ICostPart Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart_members.html)

[ICostPart::GetCostingMethod Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart~GetCostingMethod.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0