<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInterferenceDetectionMgr Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IInterferenceDetectionMgr Interface |

The following tables list the members exposed by [IInterferenceDetectionMgr](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CreateFastenersFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~CreateFastenersFolder.html) | Gets or sets whether to create the Fasteners folders to segregate interferences involving fasteners. |
| ![ Property](dotnetimages/Property.gif) | [IgnoreHiddenBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~IgnoreHiddenBodies.html) | Gets or sets whether to ignore hidden bodies during interference detection. |
| ![ Property](dotnetimages/Property.gif) | [IncludeMultibodyPartInterferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~IncludeMultibodyPartInterferences.html) | Gets or sets whether to report interferences between bodies within multibody parts. |
| ![ Property](dotnetimages/Property.gif) | [MakeInterferingPartsTransparent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~MakeInterferingPartsTransparent.html) | Gets or sets whether to display the components of the selected interference in transparent mode. |
| ![ Property](dotnetimages/Property.gif) | [NonInterferingComponentDisplay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~NonInterferingComponentDisplay.html) | Gets or sets the mode to display non-interfering components. |
| ![ Property](dotnetimages/Property.gif) | [ShowIgnoredInterferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~ShowIgnoredInterferences.html) | Gets or sets whether to show ignored interferences. |
| ![ Property](dotnetimages/Property.gif) | [TreatCoincidenceAsInterference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~TreatCoincidenceAsInterference.html) | Gets or sets whether to treat coincident entities as interference. |
| ![ Property](dotnetimages/Property.gif) | [TreatSubAssembliesAsComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~TreatSubAssembliesAsComponents.html) | Gets or sets whether to treat subassemblies as single components so that interferences between a sub-assembly's components are not reported. |
| ![ Property](dotnetimages/Property.gif) | [UseTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~UseTransform.html) | Gets or sets whether to use transforms in interference detection. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [Done](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~Done.html) | Stops the interference detection. |
| ![ Method](dotnetimages/Method.gif) | [ExportResults](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~ExportResults.html) | Saves interference detection results to a file. |
| ![ Method](dotnetimages/Method.gif) | [GetComponentsAndTransforms](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetComponentsAndTransforms.html) | Gets the interfering components and their transforms. |
| ![ Method](dotnetimages/Method.gif) | [GetComponentsTransformInterference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetComponentsTransformInterference.html) | Calculates and gets the interfering components for the specified components and math transform. |
| ![ Method](dotnetimages/Method.gif) | [GetComponentsTransformInterferenceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetComponentsTransformInterferenceCount.html) | Calculates and gets the number of interfering components for the specified components and math transform. |
| ![ Method](dotnetimages/Method.gif) | [GetInterferenceComponentCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetInterferenceComponentCount.html) | Calculates and gets the number of interfering components. |
| ![ Method](dotnetimages/Method.gif) | [GetInterferenceComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetInterferenceComponents.html) | Calculates and gets the interfering components. |
| ![ Method](dotnetimages/Method.gif) | [GetInterferenceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetInterferenceCount.html) | Calculates and gets the number of interferences. |
| ![ Method](dotnetimages/Method.gif) | [GetInterferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetInterferences.html) | Calculates and gets the interferences. |
| ![ Method](dotnetimages/Method.gif) | [IGetComponentsTransformInterference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~IGetComponentsTransformInterference.html) | Calculates and gets the interfering components for the specified components and math transform. |
| ![ Method](dotnetimages/Method.gif) | [IGetInterferenceComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~IGetInterferenceComponents.html) | Calculates and gets the interfering components. |
| ![ Method](dotnetimages/Method.gif) | [IGetInterferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~IGetInterferences.html) | Calculates and gets the interferences. |
| ![ Method](dotnetimages/Method.gif) | [SetComponentsAndTransforms](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~SetComponentsAndTransforms.html) | Sets the interfering components and their transforms. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IInterferenceDetectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IInterference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterference.html)

[IModeler::CheckInterferenceBetweenTwoBodies Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CheckInterferenceBetweenTwoBodies.html)