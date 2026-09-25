<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX~IGetControl.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetControl Method (IPropertyManagerPageActiveX) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageActiveX Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX.html) : IGetControl Method (IPropertyManagerPageActiveX) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the interface to this ActiveX control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetControl() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageActiveX Dim value As System.Object   value = instance.IGetControl() ``` | |

| C# |  |
| --- | --- |
| ``` System.object IGetControl() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ IGetControl(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

ActiveX control

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageActiveX::IGetControl.

# ![](dotnetimages/collapse.gif)Remarks

Do not call this method until the PropertyManager page is displayed. If you call this method before the PropertyManager page is displayed, then the method will fails and retval is NULL.

When the ActiveX control is created, the program creating the PropertyManager page should receive notification from the IPropertyManagerPage2Handler5::OnActiveXControlCreated method. Your program should not call [IPropertyManagerPageActiveX::GetControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageActiveX~GetControl.html) or IPropertyManagerPageActiveX::IGetControl to get the interface object for this ActiveX control, because the PropertyManager page is not displayed when this notification is sent.

When the page is displayed, your program can now initialize the control properties so that the control looks how you want it to appear when it the PropertyManager page is initially displayed. You can set up the event sink for the control so that you receive notification when certain events happen to the control.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageActiveX Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX.html)

[IPropertyManagerPageActiveX Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0