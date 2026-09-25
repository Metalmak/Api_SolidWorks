<!-- source: swconst/SO_Selection.htm -->

# SOLIDWORKS API Help

# System Options > Selection

![](SO_Selection2.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Default bulk selection method - Lasso or Box | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesDefaultBulkSelection)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesDefaultBulkSelection, <OnFlag>) | Boolean value | True to use a lasso for bulk selection, false to use a box |
| Selection of hidden edges - Allow selection in wireframe and HLV modes | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesHiddenEdgeSelectionInWireframe)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesHiddenEdgeSelectionInWireframe, <OnFlag>) | Boolean value | Specifies whether to allow selection of hidden edges or vertices in Wireframe and Hidden Lines Visible modes |
| Selection of hidden edges - Allow selection in HLR and shaded modes | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesHiddenEdgeSelectionInHLR)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEdgesHiddenEdgeSelectionInHLR, <OnFlag>) | Boolean value | Specifies whether to allow selection of hidden edges or vertices in Wireframe and Hidden Lines Visible modes |
| Enable selection through transparency | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayEnableSelectionThroughTransparency)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayEnableSelectionThroughTransparency, <OnFlag>) | Boolean value | Specifies whether to enable selection of opaque objects behind transparent objects in graphics area or selection of nearest object regardless of transparency |
| Enhance small face selection precision | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnhanceSmallFaceSelectionPrecision)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swEnhanceSmallFaceSelectionPrecision, <OnFlag>) | Boolean value | Specifies whether to enable selecting small entities more easily |