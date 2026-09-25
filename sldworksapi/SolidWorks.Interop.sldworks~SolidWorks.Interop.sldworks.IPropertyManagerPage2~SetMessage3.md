<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2~SetMessage3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetMessage3 Method (IPropertyManagerPage2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html) : SetMessage3 Method (IPropertyManagerPage2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Message*
:   Message text

*Visibility*
:   Visibility state of this message as defined by swPropertyManagerPageMessageVisibility

*Expanded*
:   Expand, compress, or leave the state of the message as is, as defined by swPropertyManagerPageMessageExpanded

*Caption*
:   Caption for message

Sets the message in this PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetMessage3( _    ByVal Message As System.String, _    ByVal Visibility As System.Integer, _    ByVal Expanded As System.Integer, _    ByVal Caption As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2 Dim Message As System.String Dim Visibility As System.Integer Dim Expanded As System.Integer Dim Caption As System.String Dim value As System.Boolean   value = instance.SetMessage3(Message, Visibility, Expanded, Caption) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetMessage3(     System.string Message,    System.int Visibility,    System.int Expanded,    System.string Caption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetMessage3(  &   System.String^ Message, &   System.int Visibility, &   System.int Expanded, &   System.String^ Caption ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Message*
:   Message text

*Visibility*
:   Visibility state of this message as defined by swPropertyManagerPageMessageVisibility

*Expanded*
:   Expand, compress, or leave the state of the message as is, as defined by swPropertyManagerPageMessageExpanded

*Caption*
:   Caption for message

#### Return Value

True if the message is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2::SetMessage3.

# ![](dotnetimages/collapse.gif)Remarks

If Caption is empty, then the current caption is not changed.

This method should be useful when creating multi-page PropertyManager pages where you want different informational messages on each page.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html)

[IPropertyManagerPage2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0