<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| eDrawings.Interop.EModelViewControl Namespace | |
| [See Also](#seealsobookmark)  [Inheritance Hierarchy](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace_hierarchy.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

eDrawings API

# ![](dotnetimages/collapse.gif)Interfaces

| Interface | Description |
| --- | --- |
| [IEModelViewControl](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) | Encapsulates the functionality of the eDrawings Viewer. |

# ![](dotnetimages/collapse.gif)Delegates

| Delegate | Description |
| --- | --- |
| [\_IEModelViewControlEvents\_OnAnimationsChangedEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnAnimationsChangedEventHandler.html) | Fired when an animation has changed. |
| [\_IEModelViewControlEvents\_OnCameraChangeEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnCameraChangeEventHandler.html) | Fired when changing the camera, including changing a scene orbit and selecting a named view. |
| [\_IEModelViewControlEvents\_OnCameraChangeFinishedEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnCameraChangeFinishedEventHandler.html) | Fired when changes to the camera have finished, including changing a scene orbit and selecting a named view. |
| [\_IEModelViewControlEvents\_OnComponentMouseOverNotify2EventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentMouseOverNotify2EventHandler.html) | Fired when the cursor is over a component. |
| [\_IEModelViewControlEvents\_OnComponentMouseOverNotifyEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentMouseOverNotifyEventHandler.html) | Obsolete. Superseded by [IEModelViewControlEvents::OnComponentMouseOverNotify2](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentMouseOverNotify2EventHandler.html) |
| [\_IEModelViewControlEvents\_OnComponentSelectionNotify2EventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentSelectionNotify2EventHandler.html) | Fired when a component is selected. |
| [\_IEModelViewControlEvents\_OnComponentSelectionNotifyEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentSelectionNotifyEventHandler.html) | Obsolete. Superseded by [IEModelViewControlEvent OnComponentSelectionNotify2](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnComponentSelectionNotify2EventHandler.html). |
| [\_IEModelViewControlEvents\_OnConfigChangeEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnConfigChangeEventHandler.html) | Fired when the specified configuration changes. |
| [\_IEModelViewControlEvents\_OnFailedLoadingDocumentEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedLoadingDocumentEventHandler.html) | Fired when the specified eDrawings document fails to load. |
| [\_IEModelViewControlEvents\_OnFailedPrintingDocumentEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler.html) | Fired if the printer name specified in the [IEModelViewControl::SetPageSetupOptions](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~SetPageSetupOptions.html) was invalid or if an eDrawings-related error exists that prevents data from being sent to a printer queue. |
| [\_IEModelViewControlEvents\_OnFailedSavingDocumentEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedSavingDocumentEventHandler.html) | Fired when saving an eDrawings document fails. |
| [\_IEModelViewControlEvents\_OnFinishedAnimationEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedAnimationEventHandler.html) | Fired when an animation has finished. |
| [\_IEModelViewControlEvents\_OnFinishedLoadingDocumentEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedLoadingDocumentEventHandler.html) | Fired when the eDrawings file has finished loading. |
| [\_IEModelViewControlEvents\_OnFinishedPrintingDocumentEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedPrintingDocumentEventHandler.html) | Fired when an eDrawings document finishes printing. |
| [\_IEModelViewControlEvents\_OnFinishedSavingDocumentEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedSavingDocumentEventHandler.html) | Fired when an eDrawings file finishes saving. |
| [\_IEModelViewControlEvents\_OnModifySceneEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnModifySceneEventHandler.html) | Fired when a scene is modified. |
| [\_IEModelViewControlEvents\_OnNamedViewEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnNamedViewEventHandler.html) | Fired when a named view has been selected. |
| [\_IEModelViewControlEvents\_OnPrevNextPlayStartEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnPrevNextPlayStartEventHandler.html) | Fired when the animation starts when associated with the **Preview**, **Next**, or **Play** button. |
| [\_IEModelViewControlEvents\_OnPrevNextPlayStopEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnPrevNextPlayStopEventHandler.html) | Fired when the animation stops when associated with the **Preview**, **Next**, or **Play** button. |
| [\_IEModelViewControlEvents\_OnStartedAnimationEventHandler](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnStartedAnimationEventHandler.html) | Fired when an animation has started. |

# ![](dotnetimages/collapse.gif)Enumerations

| Enumeration | Description |
| --- | --- |
| [EMVAnimateAction](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVAnimateAction.html) | Animation actions. |
| [EMVComponentState](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVComponentState.html) | Component states. Bitmask. |
| [EMVEnableFeatures](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVEnableFeatures.html) | Enable features. Bitmask. |
| [EMVMassProperty](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVMassProperty.html) | Mass properties. |
| [EMVOperators](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVOperators.html) | Select and view tools. |
| [EMVPrintOrientation](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVPrintOrientation.html) | Print orientations. |
| [EMVPrintType](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVPrintType.html) | Print types. |
| [EMVViewOrientation](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVViewOrientation.html) | View orientations. |
| [EMVViewState](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVViewState.html) | View states. Bitmask. |

# ![](dotnetimages/collapse.gif)See Also

####

[eDrawings.Interop.EModelViewControl Assembly](eDrawings.Interop.EModelViewControl.html)