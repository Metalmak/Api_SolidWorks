<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetImportLayerVisibility.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetImportLayerVisibility Method (IImportDxfDwgData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html) : SetImportLayerVisibility Method (IImportDxfDwgData) |

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

*Visibility*
:   Visibility of the layers as defined in swImportDxfDwg\_LayerVisibility\_e

Sets whether the specified layers are imported hidden or visible.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetImportLayerVisibility( _    ByVal Layers As System.Object, _    ByVal Visibility As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportDxfDwgData Dim Layers As System.Object Dim Visibility As System.Integer Dim value As System.Boolean   value = instance.SetImportLayerVisibility(Layers, Visibility) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetImportLayerVisibility(     System.object Layers,    System.int Visibility ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetImportLayerVisibility(  &   System.Object^ Layers, &   System.int Visibility ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Layers*
:   Array of strings of the names of the layers (see **Remarks**)

*Visibility*
:   Visibility of the layers as defined in swImportDxfDwg\_LayerVisibility\_e

#### Return Value

True if setting the visibility of these layers is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportDxfDwgData::SetImportLayerVisibility.

# ![](dotnetimages/collapse.gif)Remarks

This method only supports importing to a drawing; it does not support importing to a part sketch.

The Layers argument can contain either a string or an array of strings, where the strings are the layer names with which to work. You can also specify the argument as empty, which indicates all layers. If this method is not used, the default behavior is to import all layers with the same visibility as they have in the DXF/DWG file.

The layer visibility is the same for all sheets that are imported; you cannot specify the layer visibility on a sheet-by-sheet basis.

Hidden layers are always imported to the drawing sheet.

You should first specify the behavior that applies to all layers, using an empty VARIANT, because this overrides any information you have previously entered for specific layers. Then, you should use this method with layer names in the VARIANT, to override that default behavior on a layer-by-layer basis.

#### Visual Basic for Applications (VBA) Example

To import all layers with the same visibility as in the DXF/DWG file (this is the default behavior):

boolstatus = ImportDxfDwgData.SetImportLayerVisibility (emptyVariant, swImportDxfDwg\_LayerMaintain)

To import layer "A" hidden and the remaining layers visible:

boolstatus = ImportDxfDwgData.SetImportLayerVisibility (emptyVariant, swImportDxfDwg\_LayerVisible)

layerName = "A"

layerVariant = layerName

boolstatus = ImportDxfDwgData.SetImportLayerVisibility ((layerVariant), swImportDxfDwg\_LayerHidden)

# ![](dotnetimages/collapse.gif)See Also

####

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)

[IImportDxfDwgData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData_members.html)

[IImportDxfDwgData::GetImportLayerToSheetFormat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetImportLayerToSheetFormat.html)

[IImportDxfDwgData::GetImportLayerVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetImportLayerVisibility.html)

[IImportDxfDwgData::SetImportLayerToSheetFormat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetImportLayerToSheetFormat.html)

[IImportDxfDwgData::ImportMethod Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~ImportMethod.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0