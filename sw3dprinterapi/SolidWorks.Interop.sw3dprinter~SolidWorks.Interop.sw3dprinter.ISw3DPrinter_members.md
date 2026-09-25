<!-- source: sw3dprinterapi/SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS 3D Printer API Help | Send comments on this topic. |
| ISw3DPrinter Interface Members | |
| [See Also](#seealsobookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sw3dprinter Namespace](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter_namespace.html) : ISw3DPrinter Interface |

The following tables list the members exposed by [ISw3DPrinter](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html).

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetAvailableMaterials](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetAvailableMaterials.html) | Gets an array of strings that contain available material names, such as plastic, composite, etc., that the device can use. |
| ![ Method](dotnetimages/Method.gif) | [GetBuildEnvelope](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetBuildEnvelope.html) | Gets the dimensions of the printer envelope. |
| ![ Method](dotnetimages/Method.gif) | [GetBuildOrientation](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetBuildOrientation.html) | Gets the selected build orientation. |
| ![ Method](dotnetimages/Method.gif) | [GetCalculatedBoundingVolume](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedBoundingVolume.html) | Gets the dimension of the calculated bounding volume in document units. |
| ![ Method](dotnetimages/Method.gif) | [GetCalculatedBuildTime](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedBuildTime.html) | Gets the estimated time in minutes to build the current document. |
| ![ Method](dotnetimages/Method.gif) | [GetCalculatedCost](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedCost.html) | Gets the calculated cost in vendor-defined units, e.g., dollars, euros, liters of material, etc. |
| ![ Method](dotnetimages/Method.gif) | [GetCalculatedSurfaceArea](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedSurfaceArea.html) | Gets the calculated surface area of the current document in current document units, taking into account scale and other parameters. |
| ![ Method](dotnetimages/Method.gif) | [GetCalculatedVolume](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCalculatedVolume.html) | Gets the calculated volume of the current document in current document units, taking into account scale and other parameters. |
| ![ Method](dotnetimages/Method.gif) | [GetCurrentMaterial](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCurrentMaterial.html) | Gets the name of the selected material. |
| ![ Method](dotnetimages/Method.gif) | [GetCurrentOrientationTransform](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCurrentOrientationTransform.html) | Gets the current orientation transform. |
| ![ Method](dotnetimages/Method.gif) | [GetCurrentPrinterName](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetCurrentPrinterName.html) | Gets the name of current printer. |
| ![ Method](dotnetimages/Method.gif) | [GetDefaultBuildOrientation](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetDefaultBuildOrientation.html) | Gets the default build orientation. |
| ![ Method](dotnetimages/Method.gif) | [GetDefaultPrintQuality](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetDefaultPrintQuality.html) | Gets the default setting for print quality. |
| ![ Method](dotnetimages/Method.gif) | [GetDialogConfiguration](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetDialogConfiguration.html) | Gets a collection of bits that represent which controls SOLIDWORKS hides or changes in the Print dialog for a given print driver. |
| ![ Method](dotnetimages/Method.gif) | [GetEnvelopeOrigin](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetEnvelopeOrigin.html) | Gets the default starting location for the item to be built in the build envelope, e.g. x-min, y-min, z-min. |
| ![ Method](dotnetimages/Method.gif) | [GetOutputOption](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetOutputOption.html) | Gets the currently selected output option. |
| ![ Method](dotnetimages/Method.gif) | [GetOutputOptions](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetOutputOptions.html) | Gets an array of strings that specify how to create the rapid prototype, e.g. "Print directly to machine", "Print to queue", "Create data file", etc. |
| ![ Method](dotnetimages/Method.gif) | [GetPrinterComment](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterComment.html) | Gets a general-purpose string, possibly one that the user specified during installation. |
| ![ Method](dotnetimages/Method.gif) | [GetPrinterImageBitmap](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterImageBitmap.html) | Gets the name of the a file of a 24-bit color .bmp of dimensions 100x100 pixels that is typically an image of the printer or a corporate logo. |
| ![ Method](dotnetimages/Method.gif) | [GetPrinterLocation](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterLocation.html) | Gets the string that the user specified during installation to indicate where the printer is located (e.g., 2nd floor office). |
| ![ Method](dotnetimages/Method.gif) | [GetPrinterNames](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterNames.html) | Gets the user-specified printer names, e.g., Speedy3d\_1stfloor, speed3d\_2ndfloor, etc. |
| ![ Method](dotnetimages/Method.gif) | [GetPrinterStatus](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterStatus.html) | Gets the current state of the printer. |
| ![ Method](dotnetimages/Method.gif) | [GetPrinterType](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrinterType.html) | Gets the printer model, e.g., Speedy3D 2800. |
| ![ Method](dotnetimages/Method.gif) | [GetPrintQuality](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetPrintQuality.html) | Gets the current print quality setting of the printer. |
| ![ Method](dotnetimages/Method.gif) | [GetQuantity](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetQuantity.html) | Gets the number of copies to print. |
| ![ Method](dotnetimages/Method.gif) | [GetScale](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetScale.html) | Gets the value by which to scale the document. |
| ![ Method](dotnetimages/Method.gif) | [GetScaleParametersForActiveDocument](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~GetScaleParametersForActiveDocument.html) | Gets the values by which the document can be scaled. The values appear in the Scale box. |
| ![ Method](dotnetimages/Method.gif) | [OnAdvancedSettings](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~OnAdvancedSettings.html) | Called when a user clicks the Advanced Settings button on the 3D Printer tab. |
| ![ Method](dotnetimages/Method.gif) | [OnCancel](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~OnCancel.html) | Called when a user clicks the **Cancel** button, cancels printing the document, and closes the dialog. |
| ![ Method](dotnetimages/Method.gif) | [OnOk](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~OnOk.html) | Called when a user clicks the OK button on the dialog and sends the document to the 3D printer. |
| ![ Method](dotnetimages/Method.gif) | [OnStartup](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~OnStartup.html) | Called when the user selects the vendor's printer from the Name box on the 3D Printer tab. |
| ![ Method](dotnetimages/Method.gif) | [OnUpdateStatistics](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~OnUpdateStatistics.html) | Called when a user clicks the Update Statistics button on the 3D Printer tab and changes the build statistics. |
| ![ Method](dotnetimages/Method.gif) | [SetBuildOrientation](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetBuildOrientation.html) | Called when a user changes a build orientation on the Build Orientation tab. |
| ![ Method](dotnetimages/Method.gif) | [SetCurrentMaterial](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetCurrentMaterial.html) | Called when a user selects the name of a material in the Material box on the 3D Printer tab. |
| ![ Method](dotnetimages/Method.gif) | [SetCurrentPrinterName](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetCurrentPrinterName.html) | Sets the name of the current printer. |
| ![ Method](dotnetimages/Method.gif) | [SetOrientationTransform](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetOrientationTransform.html) | Called when a user changes a preset orthogonal orientation or Z rotation value on the Build Orientation tab. |
| ![ Method](dotnetimages/Method.gif) | [SetOutputOption](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetOutputOption.html) | Called when a user specifies how to create the rapid prototype by making a selection in the **Output** box on the 3D Printer tab. |
| ![ Method](dotnetimages/Method.gif) | [SetPrintQuality](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetPrintQuality.html) | Called when a user selects a print quality setting on the 3D Printer tab. |
| ![ Method](dotnetimages/Method.gif) | [SetQuantity](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetQuantity.html) | Called when a user sets the number of copies to print in the **Number** of copies box on the 3D Printer tab. |
| ![ Method](dotnetimages/Method.gif) | [SetScale](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter~SetScale.html) | Called when a user sets the value by which to scale the document in the Scale box on the 3D Printer tab. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISw3DPrinter Interface](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter.ISw3DPrinter.html)

[SolidWorks.Interop.sw3dprinter Namespace](SolidWorks.Interop.sw3dprinter~SolidWorks.Interop.sw3dprinter_namespace.html)