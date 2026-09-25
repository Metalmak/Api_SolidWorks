<!-- source: swconst/FileOpenOptionsGeneral.htm -->

# SOLIDWORKS API Help

# System Options > Import > General

This topic contains two tables. The information in the table:

* appearing immediately after the dialog corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on
  the dialog but are now obsolete.

To display the dialog:

Select **Tools > Options > System Options > Import
> File Format > General**.

- or -

1. Select  **File > Open.**
2. In **Files of type**, select:

> * Parasolid
> * IGES
> * STEP AP203/214/242
> * IFC 2x3
> * ACIS
> * VDAFS
> * Unigraphics/NX
> * Inventor Part
> * Inventor Assembly

1. Click Options.

![](FileOpenOptionsGeneral.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Enable 3D Interconnect | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMultiCAD\_Enable3DInterconnect)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMultiCAD\_Enable3DInterconnect, <OnFlag>) | Boolean value |  |
| Create 3D Interconnect feature link in parts only | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMultiCAD\_ApplyOnlyToParts)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMultiCAD\_ApplyOnlyToParts, <OnFlag>) | Boolean value | Valid only if swUserPreferenceToggle\_e.swMultiCAD\_Enable3DInterconnect is true. |
| Break or dissolve components as external files | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMultiCAD\_CreateNewComponentsAsExternalFiles)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMultiCAD\_CreateNewComponentsAsExternalFiles, <OnFlag>) | Boolean value | Valid only if swUserPreferenceToggle\_e.swMultiCAD\_Enable3DInterconnect is true. |
| Automatically run Import Diagnostics (Healing) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportAutoRunImportDiagnostics)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportAutoRunImportDiagnostics, <OnFlag>)  and  ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportAutoRunImportDiagnosticsPersist)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportAutoRunImportDiagnosticsPersist, <OnFlag>) | Boolean value  and  Boolean value | Specifies whether import diagnostics (healing) are run automatically. If TRUE, they are; if FALSE, they are not  and  Specifies whether users are presented with a dialog asking them if the import diagnostics (healing) should run; if True, then users are not asked and automatic healing is done depending on the value of swUserPreferenceToggle\_e.swImportAutoRunImportDiagnostics; if False, then users are asked |
| Perform full entity check and repair errors | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportCheckAndRepair)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportCheckAndRepair, <Value>) | * 0 = Do not check and repair * 1 = Check and repair |  |
| Unit - File specified unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportUnitPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportUnitPreference, swGeneralImportUnitsOptions\_e.swGeneralImportFileSpecifiedUnit) | swGeneralImportUnitsOptions\_e.swGeneralImportFileSpecifiedUnit | See swGeneralImportUnitsOptions\_e for all valid options |
| Unit - Document template specified unit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportUnitPreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportUnitPreference, swGeneralImportUnitsOptions\_e.swGeneralImportDocumentTemplateSpecifiedUnit) | swGeneralImportUnitsOptions\_e.swGeneralImportDocumentTemplateSpecifiedUnit) | See swGeneralImportUnitsOptions\_e for all valid options |
| Solid and Surface | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSolidSurface)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSolidSurface, <OnFlag>) | Boolean value | Specifies whether to import surface and solid entities; you must also set ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption, swGeneralImportSurfaceSolidEntityOptions\_e.<Value>) |
| Try forming solid(s) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption, swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportTryFormingSolids) | swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportTryFormingSolids | See swGeneralImportSurfaceSolidEntityOptions\_e for all valid options |
| B-Rep mapping | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportUseBrep)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption, swGeneralImportSurfaceSolidEntityOptions\_e.swImportUseBrep)  and  ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption, swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportByBrep) | * 0 = Import the model by directly mapping topologies   using BREP data * 1 = Do not import the model by directly mapping   topologies using BREP data   NOTE: You must set ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption, swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportByBrep) for  swGeneralImportSurfaceSolidEntityOptions\_e.swImportUseBrep to have an affect.  and  swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportByBrep | See swGeneralImportSurfaceSolidEntityOptions\_e for all valid options |
| Knit surface(s) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption, swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportKnitSurfaces) | swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportKnitSurfaces | See swGeneralImportSurfaceSolidEntityOptions\_e for all valid options |
| Do not knit | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swCreateBodyFromSurfacesOption, swGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportDoNotKnit) | wGeneralImportSurfaceSolidEntityOptions\_e.swGeneralImportDoNotKnit | See swGeneralImportSurfaceSolidEntityOptions\_e for all valid options |
| Merge Entities | See Comment | See Comment | Not currently available in SOLIDWORKS API |
| Free Curves/points entities | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportFreeCurves)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportFreeCurves, <OnFlag>) | Boolean value | Specifies whether to import free points and free curve entities; must also specify an ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportCurvePreference, swGeneralImportFreePointCurveEntityOptions\_e.<Value>) |
| Import as sketch(es) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportCurvePreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportCurvePreference, swGeneralImportFreePointCurveEntityOptions\_e.swGeneralImportAsSketches) | swGeneralImportFreePointCurveEntityOptions\_e.swGeneralImportAsSketches | See swGeneralImportFreePointCurveEntityOptions\_e for all valid options |
| Import as 3D curves | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportCurvePreference)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swImportCurvePreference, swGeneralImportFreePointCurveEntityOptions\_e.swGeneralImportAs3dCurves) | swGeneralImportFreePointCurveEntityOptions\_e.swGeneralImportAs3dCurves | See swGeneralImportFreePointCurveEntityOptions\_e for all valid options |
| Import multiple bodies as parts | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportMultBodyAsPartData)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportMultBodyAsPartData, <OnFlag>) | Boolean value | Specifies whether to import multibody part as an assembly document; for STEP and ACIS files only |
| Customize curve tolerance | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swUseCustomizedImportTolerance)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swUseCustomizedImportTolerance, <Value>) | * 0 = Do not use customized import tolerance * 1 = Use customized import tolerance | Specifies whether customized curve tolerance for imported documents is enabled |
| Customize curve tolerance <n> | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swCustomizedImportTolerance) ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swCustomizedImportTolerance, <Value>) | Double value in meters | Specifies customized curve tolerance for imported documents; swUserPreferenceIntegerValue\_e.swUseCustomizedImportTolerance must be set to 1 to enable this setting |
| IGES - Show IGES levels | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESImportShowLevel)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIGESImportShowLevel, <OnFlag>) | Boolean value | Specifies whether to displays the IGES-In Surfaces, Curves, and Levels dialog to the user where the user can specify levels and values |
| STEP - Map configuration data | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportStepConfigData)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportStepConfigData, <OnFlag>) | Boolean value | Specifies whether to import STEP file configuration data plus geometric data or geometric data only; for STEP files only |
| Force enable import diagnosis | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swForceEnableImportDiagnosis)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swForceEnableImportDiagnosis, <OnFlag>) | Boolean value | Specifies whether to force enable import diagnosis |

Obsolete Enumerators

| Enumerator | Comment |
| swImportUGToolBodies | Obsolete |