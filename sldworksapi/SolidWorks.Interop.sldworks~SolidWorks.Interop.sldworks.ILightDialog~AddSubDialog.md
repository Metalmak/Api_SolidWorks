<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog~AddSubDialog.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddSubDialog Method (ILightDialog) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILightDialog Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog.html) : AddSubDialog Method (ILightDialog) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Page*
:   Pointer to a CDialog object cast to a long

Adds a sub-dialog to the lighting dialog.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddSubDialog( _    ByVal Page As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILightDialog Dim Page As System.Integer Dim value As System.Boolean   value = instance.AddSubDialog(Page) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddSubDialog(     System.int Page ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddSubDialog(  &   System.int Page ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Page*
:   Pointer to a CDialog object cast to a long

#### Return Value

True if the dialog was successfully added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LightDialog::AddSubDialog.

# ![](dotnetimages/collapse.gif)Remarks

Currently only one sub-dialog can be added to each dialog.

# ![](dotnetimages/collapse.gif)See Also

####

[ILightDialog Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog.html)

[ILightDialog Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207