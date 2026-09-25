<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl~ShowBubbleTooltip.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowBubbleTooltip Method (IPropertyManagerPageControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageControl Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl.html) : ShowBubbleTooltip Method (IPropertyManagerPageControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Title*
:   Title to display in bubble ToolTip

*Message*
:   Message to display in bubble ToolTip

*BmpFile*
:   Path and filename of bitmap to display in bubble ToolTip

Displays a bubble ToolTip containing the specified title, message, and bitmap.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowBubbleTooltip( _    ByVal Title As System.String, _    ByVal Message As System.String, _    ByVal BmpFile As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageControl Dim Title As System.String Dim Message As System.String Dim BmpFile As System.String   instance.ShowBubbleTooltip(Title, Message, BmpFile) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowBubbleTooltip(     System.string Title,    System.string Message,    System.string BmpFile ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowBubbleTooltip(  &   System.String^ Title, &   System.String^ Message, &   System.String^ BmpFile ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Title*
:   Title to display in bubble ToolTip

*Message*
:   Message to display in bubble ToolTip

*BmpFile*
:   Path and filename of bitmap to display in bubble ToolTip

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageControl::ShowBubbleTooltip.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPageControl](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

A bubble ToolTip is useful for validating data typed or selected by users in controls on a PropertyManager page.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageControl Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl.html)

[IPropertyManagerPageControl Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0