<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~CreateFeatureMgrControl4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFeatureMgrControl4 Method (IModelViewManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html) : CreateFeatureMgrControl4 Method (IModelViewManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BitMapFileNames*
:   Array of fully qualified paths to three bitmap files, one for each size (small, medium, and large), to be used for the tab icon in different screen resolutions

*Class*
:   CLSID or ProgID for the ActiveX control (see **Remarks**)

*LicKey*
:   License key for the ActiveX control; empty string if unknown

*ToolTip*
:   Text to display when hovering over the tab icon

*WhichPane*
:   Pane where to add the tab as defined in swFeatMgrPane\_e (see **Remarks**)

Creates a new FeatureManager design tree view containing the specified ActiveX control with a tab that displays the specified scaleable icon.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFeatureMgrControl4( _    ByVal BitMapFileNames As System.Object, _    ByVal Class As System.String, _    ByVal LicKey As System.String, _    ByVal ToolTip As System.String, _    ByVal WhichPane As System.Integer _ ) As FeatMgrView ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelViewManager Dim BitMapFileNames As System.Object Dim Class As System.String Dim LicKey As System.String Dim ToolTip As System.String Dim WhichPane As System.Integer Dim value As FeatMgrView   value = instance.CreateFeatureMgrControl4(BitMapFileNames, Class, LicKey, ToolTip, WhichPane) ``` | |

| C# |  |
| --- | --- |
| ``` FeatMgrView CreateFeatureMgrControl4(     System.object BitMapFileNames,    System.string Class,    System.string LicKey,    System.string ToolTip,    System.int WhichPane ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` FeatMgrView^ CreateFeatureMgrControl4(  &   System.Object^ BitMapFileNames, &   System.String^ Class, &   System.String^ LicKey, &   System.String^ ToolTip, &   System.int WhichPane ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BitMapFileNames*
:   Array of fully qualified paths to three bitmap files, one for each size (small, medium, and large), to be used for the tab icon in different screen resolutions

*Class*
:   CLSID or ProgID for the ActiveX control (see **Remarks**)

*LicKey*
:   License key for the ActiveX control; empty string if unknown

*ToolTip*
:   Text to display when hovering over the tab icon

*WhichPane*
:   Pane where to add the tab as defined in swFeatMgrPane\_e (see **Remarks**)

#### Return Value

Pointer to the new [tab](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatMgrView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelViewManager::CreateFeatureMgrControl4.

# ![](dotnetimages/collapse.gif)Example

[Add ActiveX Tab to FeatureManager Design Tree (VBA)](Add_ActiveX_Tab_to_FeatureManager_Design_Tree_Example_VB.htm)

[Add ActiveX Tab to FeatureManager Design Tree (VB.NET)](Add_ActiveX_Tab_to_FeatureManager_Design_Tree_Example_VBNET.htm)

[Add ActiveX Tab to FeatureManager Design Tree (C#)](Add_ActiveX_Tab_to_FeatureManager_Design_Tree_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To:

* Add a tab to the FeatureManager design tree, specify WhichPane with swFeatMgrPane\_e.FeatMgrPaneBottom.* Add a tab to a split FeatureManager design tree, specify WhichPane with either swFeatMgrPane\_e.swFeatMgrPaneTop or swFeatMgrPane\_e.swFeatMgrPaneBottom. See [IModelDoc2::FeatureManagerSplitterPosition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~FeatureManagerSplitterPosition.html) for details on splitting and positioning the split panel bar in the FeatureManager design tree.* Delete the tab created by this method, use [IFeatMgrView::DeleteView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatMgrView~DeleteView.html).

Specify Class with either the ProgID or the CLSID of the registered ActiveX control. You can obtain these strings by searching for the registered ActiveX control in the registry editor.

For example, **RichEditCtrol.ocx** resides in **c:\Program files\SOLIDWORKS Corp\SOLIDWORKS\sldUtils**. It is registered during the SOLIDWORKS installation. When you search for **RichEditCtrl.ocx** in the registry, you find ProgID = GTSWRICHEDITCTRL.RichEditCtrlCtrl.1 and CLSID = {7632C33C-A935-48FF-84D9-F0F173EF543D}. Use either the registry's ActiveX ProgID or CLSID to specify Class. The ActiveX control library names displayed in the Object Browser may not be the same as the ActiveX control names in the registry. Do not use the Object Browser to specify Class.

See also Keystrokes and Accelerator Keys in ActiveX Modeless Dialogs and PropertyManager Pages.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html)

[IModelViewManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager_members.html)

[IModelViewManager::CreateFeatureMgrView2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~CreateFeatureMgrView2.html)

[IModelViewManager::AddControl3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~AddControl3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0