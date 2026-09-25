<!-- source: swconst/FileOpenOptionsInventorCatiaCreoNXSE.htm -->

# SOLIDWORKS API Help

# System Options > Import > Inventor/Catia V5/Creo/NX/Solid Edge

To display the dialog:

Select **Tools > Options > System Options > Import > File Format
> Inventor/Catia V5/Creo/NX/Solid Edge**.

- or -

1. Click **File > Open**.
2. In **Files of type**, select
   **Inventor** (**Part** or **Assembly**), **Catia V5**, **ProE/Creo**(**Part** or **Assembly**), **Unigraphics/NX**, or **Solid
   Edge** (**Part** or **Assembly**).
3. Click **Options**.

![](FileOpenOptionsInventorCatiaCreoNXSE.gif)

| Setting | Get/Set Methods | Return Value  or   <Value>  or  <OnFlag> | Comment |
| Entities to Read From 3rd Party CAD Files - Solid Body | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSolidBody)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSolidBody, <OnFlag>) | Boolean value |  |
| Entities to Read From 3rd Party CAD Files - Surface Body | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSurfaceBody)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportSurfaceBody, <OnFlag>) | Boolean value |  |
| Entities to Read From 3rd Party CAD Files - Reference Plane | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportReferencePlane)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportReferencePlane, <OnFlag>) | Boolean value |  |
| Entities to Read From 3rd Party CAD Files - Reference Axis | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportReferenceAxis)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportReferenceAxis, <OnFlag>) | Boolean value |  |
| Entities to Read From 3rd Party CAD Files - Unconsumed Sketch(es) and Curves | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportUnconsumedSketchesAndCurves)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportUnconsumedSketchesAndCurves, <OnFlag>) | Boolean value |  |
| Entities to Read From 3rd Party CAD Files - Custom Properties | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportCustomProperties)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportCustomProperties, <OnFlag>) | Boolean value |  |
| Entities to Read From 3rd Party CAD Files - Material Properties | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportMaterialProperties)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportMaterialProperties, <OnFlag>) | Boolean value |  |
| Options - Dissolve top level assembly on open (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportDissolveTopLevelAssemblyOnOpen)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportDissolveTopLevelAssemblyOnOpen, <OnFlag>) | Boolean value |  |
| Options - Ignore Hidden Entities | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportIgnoreHiddenEntities)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportIgnoreHiddenEntities, <OnFlag>) | Boolean value |  |
| Options - Import tool bodies from UG NX | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportToolBodiesFromUGNX)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportToolBodiesFromUGNX, <OnFlag>) | Boolean value |  |