<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__ThruTapDrillDiameter.htm -->

# WizardHoleFeatureData::ThruTapDrillDiameter

This
property is obsolete and has been superseded by WizardHoleFeatureData2::ThruTapDrillDiameter.

Description

This property gets or sets the hole wizard feature through tap drill
diameter.

Syntax (OLE Automation)

tapdrillDia = WizardHoleFeatureData.ThruTapDrillDiameter
  (VB Get property)

WizardHoleFeatureData.ThruTapDrillDiameter = tapdrillDia   (VB Set property)

tapdrillDia = WizardHoleFeatureData.GetThruTapDrillDiameter
( ) (C++ Get property)

WizardHoleFeatureData.SetThruTapDrillDiameter ( tapdrillDia )  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) tapdrillDia | Through tap drill diameter |

Syntax (COM)

status = WizardHoleFeatureData ->get\_ThruTapDrillDiameter
( &tapdrillDia )

status = WizardHoleFeatureData ->put\_ThruTapDrillDiameter
( tapdrillDia )

|  |  |  |
| --- | --- | --- |
| Property: | (double) tapdrillDia | Through tap drill diameter |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is relevant only for tapped holes.