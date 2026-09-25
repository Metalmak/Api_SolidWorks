<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetImportLayerToSheetFormat.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetImportLayerToSheetFormat Method (IImportDxfDwgData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html) : SetImportLayerToSheetFormat Method (IImportDxfDwgData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Layers*
:   Array of strings of the names of the layers (see **Remarks**)

*SheetFormat*
:   True to import the specified visible layers to the sheet format, false to import them to the drawing sheet

Sets whether the specified visible layers are imported to the sheet format or drawing sheet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetImportLayerToSheetFormat( _    ByVal Layers As System.Object, _    ByVal SheetFormat As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportDxfDwgData Dim Layers As System.Object Dim SheetFormat As System.Boolean Dim value As System.Boolean   value = instance.SetImportLayerToSheetFormat(Layers, SheetFormat) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetImportLayerToSheetFormat(     System.object Layers,    System.bool SheetFormat ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetImportLayerToSheetFormat(  &   System.Object^ Layers, &   System.bool SheetFormat ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Layers*
:   Array of strings of the names of the layers (see **Remarks**)

*SheetFormat*
:   True to import the specified visible layers to the sheet format, false to import them to the drawing sheet

#### Return Value

True of importing the specified visible  layers was successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportDxfDwgData::SetImportLayerToSheetFormat.

# ![](dotnetimages/collapse.gif)Remarks

This method only supports importing to a drawing; it does not support importing to a part sketch.

The Layers argument can contain either a string or an array of strings, where the strings are the layer names with which to work. You can also specify the argument as empty, which indicates all layers. If this method is not used, the default behavior is to import all layers to the drawing sheet.

The import to sheet or sheet format Boolean is the same for all sheets that are imported; you cannot specify it on a sheet-by-sheet basis.

#### Visual Basic for Applications (VBA) Example

To import all layers on all sheets to drawings sheets in SOLIDWORKS (this is the default behavior):

boolstatus = ImportDxfDwgData.SetImportLayerToSheetFormat (emptyVariant, false)

To import layers "A" and "B" to the drawing sheet and the remaining layers to the sheet format:

boolstatus = ImportDxfDwgData.SetImportLayerToSheetFormat (emptyVariant, True)

layerName(0) = "A"

layerName(1) = "B"

layerVariant = layerName

boolstatus = ImportDxfDwgData.SetImportLayerToSheetFormat ((layerVariant), false)

# ![](dotnetimages/collapse.gif)See Also

####

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)

[IImportDxfDwgData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData_members.html)

[IImportDxfDwgData::GetImportLayerToSheetFormat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetImportLayerToSheetFormat.html)

[IImportDxfDwgData::GetImportLayerVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetImportLayerVisibility.html)

[IImportDxfDwgData::SetImportLayerVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetImportLayerVisibility.html)

[IImportDxfDwgData::ImportMethod Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~ImportMethod.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0