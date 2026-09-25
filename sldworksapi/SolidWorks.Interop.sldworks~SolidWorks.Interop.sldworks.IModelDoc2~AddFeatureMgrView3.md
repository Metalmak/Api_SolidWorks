<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AddFeatureMgrView3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddFeatureMgrView3 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : AddFeatureMgrView3 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Bitmap*
:   Pointer to the bitmap that you want to use for the FeatureManager design tree tab; the bitmap should be no larger than 16x18; this standard pointer is created by performing a New on Cbitmap

*AppView*
:   Pointer to an existing view that you want to use as your FeatureManager design tree view. If you do not have an existing view, then use [IModelViewMgr::CreateFeatureMgrView2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~CreateFeatureMgrView2.html), which returns a view handle

*ToolTip*
:   ToolTip string

*WhichPane*
:   Pane in which to add the view as defined in swFeatMgrPane\_e

Adds the specified tab to the FeatureManager design tree view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddFeatureMgrView3( _    ByRef Bitmap As System.Integer, _    ByRef AppView As System.Integer, _    ByVal ToolTip As System.String, _    ByVal WhichPane As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Bitmap As System.Integer Dim AppView As System.Integer Dim ToolTip As System.String Dim WhichPane As System.Integer Dim value As System.Boolean   value = instance.AddFeatureMgrView3(Bitmap, AppView, ToolTip, WhichPane) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddFeatureMgrView3(     ref System.int Bitmap,    ref System.int AppView,    System.string ToolTip,    System.int WhichPane ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddFeatureMgrView3(  &   System.int% Bitmap, &   System.int% AppView, &   System.String^ ToolTip, &   System.int WhichPane ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Bitmap*
:   Pointer to the bitmap that you want to use for the FeatureManager design tree tab; the bitmap should be no larger than 16x18; this standard pointer is created by performing a New on Cbitmap

*AppView*
:   Pointer to an existing view that you want to use as your FeatureManager design tree view. If you do not have an existing view, then use [IModelViewMgr::CreateFeatureMgrView2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~CreateFeatureMgrView2.html), which returns a view handle

*ToolTip*
:   ToolTip string

*WhichPane*
:   Pane in which to add the view as defined in swFeatMgrPane\_e

#### Return Value

True if the FeatureManager design tree view tab is added successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::AddFeatureMgrView3.

# ![](dotnetimages/collapse.gif)Remarks

This method is not valid in the context of the Microsoft .NET Framework; it is only valid for old-style add-ins, which are now obsolete. Instead, use [IModelViewManager::CreateFeatureMgrControl3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~CreateFeatureMgrControl3.html), which allows you to provide the ProgID or CLSID of an ActiveX control to use in the new tab for the FeatureManager design tree.

This method is identical to the earlier version, IModelDoc2::AddFeatureMgrView2, except that this method provides the ability to place the new tab on either the top or bottom pane. The pane may or may not be visible. However, the tab is added to the specified pane. Only the values swFeatMgrPaneTop and swFeatMgrPaneBottom from swFeatMgrPane\_e should be used as inputs in the whichPane argument.

Under certain conditions, for example while the Surface, Extend command is active in the user interface, SOLIDWORKS locks the bottom pane and does not allow the activation of any other tab. If your application needs the ability to activate your new tab at all times, consider adding it either to the top pane or to both panes. If you add it to the top pane only, it may not be apparent to the user until the top pane is made visible.

If you have an existing CView, this method adds that view as a new FeatureManager design tree view. This method also provides a parameter for adding a tab, which the user clicks to activate your view.

The FeatureManager design tree view added to this document is not persistent. In other words, the FeatureManager design tree view is not stored with this document and must be recreated upon reloading the document.

This method does not receive [IFeatMgrView::ActivateNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatMgrView~ActivateView.html) and [IFeatMgrView::DeactivateNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatMgrView~DeActivateView.html) events.

This view is generated by you and can be drawn into as you desire. However, because you generated this view, you are responsible for deleting it. See [IModelDoc2::DeleteFeatureMgrView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~DeleteFeatureMgrView.html) and [IModelDocExtension::DeleteFeatureMgrViewx64](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~DeleteFeatureMgrViewx64.html) for details on how to delete your Feature Manager view.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0