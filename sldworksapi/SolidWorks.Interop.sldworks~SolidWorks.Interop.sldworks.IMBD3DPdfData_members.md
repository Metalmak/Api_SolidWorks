<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMBD3DPdfData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IMBD3DPdfData Interface |

The following tables list the members exposed by [IMBD3DPdfData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Accuracy](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~Accuracy.html) | Gets or sets the level of accuracy for lossy compression when publishing to SOLIDWORKS MBD 3D PDF. |
| ![ Property](dotnetimages/Property.gif) | [CompressLossyTessellation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~CompressLossyTessellation.html) | Gets or sets whether to apply lossy compression to polygons in the model when publishing to SOLIDWORKS MBD 3D PDF. |
| ![ Property](dotnetimages/Property.gif) | [CreateAttachSTEP242](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~CreateAttachSTEP242.html) | Gets or sets whether to export SOLIDWORKS parts and assemblies to STEP 242 format and attach the STEP 242 file to the SOLIDWORKS MBD 3D PDF. |
| ![ Property](dotnetimages/Property.gif) | [ExcludeFromAnnotationView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ExcludeFromAnnotationView.html) | Gets or sets whether to exclude BOM tables from annotation views for this SOLIDWORKS MBD 3D PDF. |
| ![ Property](dotnetimages/Property.gif) | [FilePath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~FilePath.html) | Gets or sets the path and file name to which to save this SOLIDWORKS MBD 3D PDF. |
| ![ Property](dotnetimages/Property.gif) | [ThemeName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ThemeName.html) | Gets or sets the path and file name of the theme for this SOLIDWORKS MBD 3D PDF. |
| ![ Property](dotnetimages/Property.gif) | [ViewPdfAfterSaving](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ViewPdfAfterSaving.html) | Gets or sets whether to display this SOLIDWORKS MBD 3D PDF after [publishing it](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~PublishTo3DPDF.html). |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetAttachments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~GetAttachments.html) | Gets the fully qualified paths of the files to include as attachments when publishing to SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [GetBomAreaCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~GetBomAreaCount.html) | Gets the number of BOM Table Areas defined in the [theme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ThemeName.html) for this SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [GetImportedNotes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~GetImportedNotes.html) | Gets the imported note names from the theme of this MBD3DPdfData. |
| ![ Method](dotnetimages/Method.gif) | [GetMoreViews](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~GetMoreViews.html) | Gets the names of the custom views (i.e., [named views](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~NameView.html) and [3D views](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D.html)) in the model for this SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [GetStandardViews](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~GetStandardViews.html) | Gets the types of standard views in the model for this SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [GetTextAndCustomProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~GetTextAndCustomProperties.html) | Gets the text and custom properties in the [theme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ThemeName.html) for this SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [SetAttachments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetAttachments.html) | Sets the fully qualified paths of the files to include as attachments when publishing to SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [SetBomTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetBomTable.html) | Maps a BOM Table Area in the [theme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~ThemeName.html) with a BOM table in the model and sets the columns in the BOM table to export to the BOM Table Area in a SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [SetImportedNote](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetImportedNote.html) | Sets the specified imported note. |
| ![ Method](dotnetimages/Method.gif) | [SetIndependentViewPort](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetIndependentViewPort.html) | Sets the specified view for an independent viewport for the SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [SetMoreViews](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetMoreViews.html) | Sets the names of the custom views (i.e., [named views](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~NameView.html) and [3D views](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D.html)) in the model for this SOLIDWORKS MBD 3D PDF. |
| ![ Method](dotnetimages/Method.gif) | [SetStandardViews](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~SetStandardViews.html) | Sets the types of standard views in the model for this SOLIDWORKS MBD 3D PDF. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IMBD3DPdfData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IModelDocExtension::PublishTo3DPDF Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~PublishTo3DPDF.html)

[IView3D Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D.html)