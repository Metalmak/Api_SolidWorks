<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~CreateFeatureMgrControl.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFeatureMgrControl Method (IModelViewManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html) : CreateFeatureMgrControl Method (IModelViewManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PPicture*
:   Pointer to the bitmap that you want to use for the tab

*Class*
:   Class ID for the ActiveX control

*LicKey*
:   License key for the ActiveX control

*ToolTip*
:   Text for the ToolTip

*WhichPane*
:   Pane to use as defined in swFeatMgrPane\_e

Obsolete. Superseded by [IModelViewManager::CreateFeatureMgrControl2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~CreateFeatureMgrControl2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFeatureMgrControl( _    ByVal PPicture As System.Object, _    ByVal Class As System.String, _    ByVal LicKey As System.String, _    ByVal ToolTip As System.String, _    ByVal WhichPane As System.Integer _ ) As FeatMgrView ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelViewManager Dim PPicture As System.Object Dim Class As System.String Dim LicKey As System.String Dim ToolTip As System.String Dim WhichPane As System.Integer Dim value As FeatMgrView   value = instance.CreateFeatureMgrControl(PPicture, Class, LicKey, ToolTip, WhichPane) ``` | |

| C# |  |
| --- | --- |
| ``` FeatMgrView CreateFeatureMgrControl(     System.object PPicture,    System.string Class,    System.string LicKey,    System.string ToolTip,    System.int WhichPane ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` FeatMgrView^ CreateFeatureMgrControl(  &   System.Object^ PPicture, &   System.String^ Class, &   System.String^ LicKey, &   System.String^ ToolTip, &   System.int WhichPane ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PPicture*
:   Pointer to the bitmap that you want to use for the tab

*Class*
:   Class ID for the ActiveX control

*LicKey*
:   License key for the ActiveX control

*ToolTip*
:   Text for the ToolTip

*WhichPane*
:   Pane to use as defined in swFeatMgrPane\_e

#### Return Value

Pointer to the new [tab](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatMgrView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelViewManager::CreateFeatureMgrControl.

# ![](dotnetimages/collapse.gif)Remarks

This method is not supported in applications written in .NET languages.

The user can click the tab to activate an ActiveX control.

This method references the IPictureDisp interface. Use [IModelViewManager::CreateFeatureMgrControl2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~CreateFeatureMgrControl2.html) to specify the fully qualified path to the bitmap file on disk. Use [IModelViewManager::CreateFeatureMgrControl3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~CreateFeatureMgrControl3.html) if tab traversal support is needed and specify a fully qualified path to the bitmap file on disk.

This method sets the class ID and license key information for the ActiveX control when the API PropertyManager page is shown and the ActiveX control is created. The Class argument can be either the name of the control (ProgID) or the class ID (CLSID), for example, "MSCAL.calendar" or "{8E27C92B-1264-101C-8A2F-040224009C02}". Both provide the calendar protocol. You can obtain these strings using a combination of the Microsoft OLE/COM Object Viewer and the registry editor.

For example:

' ProgID

bRet = m\_pActiveXControl.SetClass("MSCAL.Calendar", "")

bRet = m\_pActiveXControl2.SetClass("MSComctlLib.ListViewCtrl", "")

' CLSID

bRet = m\_pActiveXControl.SetClass("{8E27C92B-1264-101C-8A2F-040224009C02}", "")

bRet = m\_pActiveXControl2.SetClass("{BDD1F04B-858B-11D1-B16A-00C0F0283628}", "")

See also Keystrokes and Accelerator Keys in ActiveX Modeless Dialogs and PropertyManager Pages.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html)

[IModelViewManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 SP1, Revision Number 11.1