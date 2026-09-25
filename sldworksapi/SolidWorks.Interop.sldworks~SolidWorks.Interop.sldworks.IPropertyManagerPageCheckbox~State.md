<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageCheckbox~State.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| State Property (IPropertyManagerPageCheckbox) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageCheckbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageCheckbox.html) : State Property (IPropertyManagerPageCheckbox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the state of this check box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property State As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageCheckbox Dim value As System.Integer   instance.State = value   value = instance.State ``` | |

| C# |  |
| --- | --- |
| ``` System.int State {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int State {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

State of this check box as defined in swPropertyManagerCheckboxState\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageCheckbox::State.

# ![](dotnetimages/collapse.gif)Example

[Set Focus on PropertyManager Page Control (C#)](Set_Focus_on_PropertyManager_Page_Control_Example_CSharp.htm)

[Set Focus on PropertyManager Page Control (VB.NET)](Set_Focus_on_PropertyManager_Page_Control_Example_VBNET.htm)

[Set Focus on PropertyManager Page Control (VBA)](Set_Focus_on_PropertyManager_Page_Control_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you use this property to set the state of a check box, then you must use this property to modify the state of the check box.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageCheckbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageCheckbox.html)

[IPropertyManagerPageCheckbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageCheckbox_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0