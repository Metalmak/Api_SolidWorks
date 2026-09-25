<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSWPropertySheetEvents_HelpNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSWPropertySheetEvents\_HelpNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSWPropertySheetEvents\_HelpNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PageIndex*
:   Page index of the add-in's Help

Fired when the Help button is clicked on a property sheet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSWPropertySheetEvents_HelpNotifyEventHandler( _    ByVal PageIndex As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSWPropertySheetEvents_HelpNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSWPropertySheetEvents_HelpNotifyEventHandler(     System.int PageIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSWPropertySheetEvents_HelpNotifyEventHandler(  &   System.int PageIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PageIndex*
:   Page index of the add-in's Help

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HelpNotify Event (SWPropertySheet).

# ![](dotnetimages/collapse.gif)Remarks

Your application should only display Help if you have added a Help page.

For add-ins, if PageIndex is the same as the value returned by [ISWPropertySheet::AddActivePage](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISWPropertySheet~AddActivePage.html), then the add-in can display its Help.

If developing a C++ application, use swPropertySheetHelpNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0