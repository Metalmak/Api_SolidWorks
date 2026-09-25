<!-- source: obsoleteapi/WizardHoleFeatureData/WizardHoleFeatureData__TapDrillDiameter.htm -->

# WizardHoleFeatureData::TapDrillDiameter

This
property is obsolete and has been superseded by WizardHoleFeatureData2::TapDrillDiameter.

Description

This property gets or sets the hole wizard
feature tap drill diameter.

Syntax (OLE Automation)

tapdrillDia = WizardHoleFeatureData.TapDrillDiameter  (VB
Get property)

WizardHoleFeatureData.TapDrillDiameter= tapdrillDia   (VB Set property)

tapdrillDia = WizardHoleFeatureData.GetTapDrillDiameter
( ) (C++ Get property)

WizardHoleFeatureData.SetTapDrillDiameter ( tapdrillDia )  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) tapdrillDia | Tap drill diameter |

Syntax (COM)

status = WizardHoleFeatureData ->get\_TapDrillDiameter
( &tapdrillDia )

status = WizardHoleFeatureData ->put\_TapDrillDiameter
( tapdrillDia )

|  |  |  |
| --- | --- | --- |
| Property: | (double) tapdrillDia | Tap drill diameter |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is relevant only for tapped holes.