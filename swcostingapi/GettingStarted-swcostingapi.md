<!-- source: swcostingapi/GettingStarted-swcostingapi.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help |  |
| Getting Started |
| Send Feedback | |

Glossary Item Box

Writing a SOLIDWORKS Costing API application typically involves:

1. Adding a reference to either the SOLIDWORKS Costing API type library or primary interop assembly:
   * VBA: **SldCostingAPI** *version* **Type Library** or *install\_dir*\**sldcostingapi.tlb**.* C# or VB.NET: **SolidWorks.Interop.sldcostingapi** or *install\_dir*\**api\redist\SolidWorks.Interop.sldcostingapi.dll**.

       **NOTE**: *install\_dir* is usually **C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS**.- Opening the part for the Costing analysis.- Getting or setting the Costing template folders and Costing Report template folders using ISldWorks::GetUserPreferenceStringValue or ISldWorks::SetUserPreferenceStringValue (see **Templates**).- Getting the model document, IModelDoc2 object.- Getting the CostingManager, [ICostManager](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostManager.html) object, and getting the Costing templates.- Getting the Costing model, [ICostPart](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostPart.html) object.- Getting the Costing bodies, [ICostBody](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostBody.html) objects.- Creating or getting the common Costing analysis, [ICostAnalysis](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis.html) object, and getting and setting its analysis data.- Creating or getting each Costing body's specific Costing analysis.- Getting each Costing feature or subfeature, [ICostFeature](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostFeature.html) object, and getting or setting its analysis data.

## Templates

The SOLIDWORKS Costing tool provides templates that associate manufacturing features with their costs. The templates include information about material, machining, and labor costs. After the manufacturing features are recognized, Costing categorizes each manufacturing feature and applies the correct information from the template to cost out the specific manufacturing features. A total cost for all of the features is tabulated and a final unit cost is returned. You can also create reports of Costing results using the SOLIDWORKS Costing tool. The detailed line items in the report help you determine the impact of design decisions on cost.

To get or set the file locations for Costing templates and Costing report templates, you can use the SOLIDWORKS API and call ISldWorks::GetUserPreferenceStringValue or ISldWorks::SetUserPreferenceStringValue with:

* swUserPreferenceStringValue\_e.swFileLocationsCostingTemplates for Costing templates.* swUserPreferenceStringValue\_e.swFileLocationsCostingReportTemplateFolder for Costing report templates.

For more information about SOLIDWORKS Costing and its templates, see the SOLIDWORKS Help.