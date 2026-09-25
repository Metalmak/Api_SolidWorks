<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2~Pinned.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Pinned Property (IPropertyManagerPage2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html) : Pinned Property (IPropertyManagerPage2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the state of the pushpin on a PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Pinned As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2 Dim value As System.Boolean   instance.Pinned = value   value = instance.Pinned ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Pinned {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool Pinned {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if pushpin is pressed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2::Pinned.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |  |
| --- | --- | --- |
| **If the user clicks...** | **And PropertyManagerPage2::GetPinned is...** | **Then...** |
| x | True or false | IPropertyManagerPage2Handler8::OnClose(swPropertyManagerPageClose\_Closed) is called, the dialog closes, and IPropertyManagerPage2Handler8::AfterClose is called. |
| check mark | True | IPropertyManagerPage2Handler8::OnClose(swPropertyManagerPageClose\_Apply) is called, the dialog is not closed, IPropertyManagerPage2Handler8::AfterClose is not called. |
|  | false | IPropertyManagerPage2Handler8::OnClose(swPropertyManagerPageClose\_Okay) is called, the dialog is closed, and IPropertyManagerPage2Handler8::AfterClose is called. |

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html)

[IPropertyManagerPage2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0