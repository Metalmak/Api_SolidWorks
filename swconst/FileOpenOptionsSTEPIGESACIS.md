<!-- source: swconst/FileOpenOptionsSTEPIGESACIS.htm -->

# SOLIDWORKS API Help

# System Options > Import > STEP/IGES/ACIS

To display the dialog:

Select **Tools > Options > System Options > Import > File Format
> STEP/IGES/ACIS**.

- or -

1. Select **File > Open**.
2. In **Files of type**, select
   **IGES**, **ACIS**,or **STEP AP203/214/242**.
3. Click **Options**.

![](FileOpenOptionsSTEPIGESACIS.gif)

| Setting | Get/Set Methods | Return Value  or   <Value>  or  <OnFlag> | Comment |
| Entities to Import - Solids and Surfaces | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutral\_SolidandSurface)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutral\_SolidandSurface, <OnFlag>) | Boolean value |  |
| Entities to Import - Try forming solid(s) or Do not knit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportNeutral\_KnitOption) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportNeutral\_KnitOption, swImportNeutralKnitOption\_e.<*Value*>) | Integer value as defined in swImportNeutralKnitOption\_e | Valid only if **Entities to Import - Solids and Surfaces** is set to true |
| Entities to Import - Free Curves and Points as Sketch | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutral\_FreeCurvesAndPoints)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutral\_FreeCurvesAndPoints, <OnFlag>) | Boolean value |  |
| Entities to Import - Reference Planes | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutralReferencePlane)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutralReferencePlane, <OnFlag>) | Boolean value |  |
| Entities to Import - User Define Attributes | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutral\_AttributesAndProperties)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutral\_AttributesAndProperties, <OnFlag>) | Boolean value |  |
| Options - Assembly Structure Mapping | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportNeutralAssemblyStructureMapping)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportNeutralAssemblyStructureMapping, swImportNeutralAssemblyStructureMapping\_e.<*Value*>) | Integer value as defined in swImportNeutralAssemblyStructureMapping\_e |  |
| Options - Automatically run Import Diagnostics (Healing) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutralRunDiagnostics)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutralRunDiagnostics, <OnFlag>) | Boolean value |  |
| Options - Create analytic faces (slower) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutralAnalyticalConversion)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportNeutralAnalyticalConversion, <OnFlag>) | Boolean value |  |
| Options - Unit of Import | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportNeutralUnits)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportNeutralUnits, swImportNeutralUnits\_e.<*Value*>) | Integer value as defined in swImportNeutralUnits\_e |  |