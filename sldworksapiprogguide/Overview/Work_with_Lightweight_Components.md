<!-- source: sldworksapiprogguide/Overview/Work_with_Lightweight_Components.htm -->

# SOLIDWORKS API Help

# Work with Lightweight Components

SOLIDWORKS supports a mode for assembly components called lightweight.
A lightweight component contains only a small subset of its data for display
purposes, which increases system performance when loading assemblies.
The extra data is not loaded until it is needed.

Because lightweight components contain only a small subset of the data,
applications cannot query for all the information that is available to
a fully resolved component. To avoid problems in this area, IComponent2::IsHidden
and IComponent2::IsSuppressed
return true if a component is flagged as lightweight. IComponent2::IGetBody
returns a special HRESULT value if a component is lightweight.

To take advantage of lightweight components, use IComponent2::GetSuppression,
IComponent2::SetSuppression,
IAssemblyDoc::ResolveAllLightWeightComponents,
and IAssemblyDoc::GetLightWeightComponentCount.

To find or control whether SOLIDWORKS is using lightweight components
see:

* ISldWorks::SetUserPreferenceToggle -
  swAutoLoadPartsLightweight controls whether assemblies are loaded
  with lightweight components
* ISldWorks::SetUserPreferenceIntegerValue -
  swResolveLightweight controls how lightweight components are resolved