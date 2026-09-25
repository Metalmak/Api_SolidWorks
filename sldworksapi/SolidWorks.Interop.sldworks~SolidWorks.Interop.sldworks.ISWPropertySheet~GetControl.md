<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet~GetControl.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetControl Method (ISWPropertySheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISWPropertySheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet.html) : GetControl Method (ISWPropertySheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PageIndex*
:   Index of property sheet

Gets the ActiveX control on the property sheet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetControl( _    ByVal PageIndex As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISWPropertySheet Dim PageIndex As System.Integer Dim value As System.Object   value = instance.GetControl(PageIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetControl(     System.int PageIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetControl(  &   System.int PageIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PageIndex*
:   Index of property sheet

#### Return Value

ActiveX control

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SWPropertySheet::GetControl.

# ![](dotnetimages/collapse.gif)Remarks

Typically, you would call this method from the ISWPropertySheet [OnOKNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSWPropertySheetEvents_OnOKNotifyEventHandler.html) event handler to retrieve data from your ActiveX control.

# ![](dotnetimages/collapse.gif)See Also

####

[ISWPropertySheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet.html)

[ISWPropertySheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP4, Revision Number 12.4